---
title: Theme List
description: List of all NeoMutt's colour themes
keywords: [neomutt, email, terminal, theme, preview]
---

# Theme List

<img src="_static/icon-terminal-at.png" alt="" class="page-icon">

Browse the full catalogue of NeoMutt colour themes below.
Each row shows the theme name, download links for **TrueColor** and **256-colour** palette files, and a swatch preview.
The first four swatches are **special colours** (foreground, background, cursor, and selection), followed by the **16 ANSI palette colours** (black through white, normal and bright).

Click a **truecolor** or **palette** link to download the `.rc` file, then `source` it in your `neomuttrc`.

<div id="theme-grid" class="theme-grid"></div>

<script src="/_static/theme-data.js"></script>
<script>
(function() {
  if (typeof themes === "undefined") return;

  var ROW_HEIGHT = 28;
  var BUFFER = 10;
  var container = document.getElementById("theme-grid");
  var totalHeight = themes.length * ROW_HEIGHT;

  // Fixed-height scrollable container with a tall spacer
  container.style.height = Math.min(totalHeight, 600) + "px";
  container.style.overflow = "auto";
  container.style.position = "relative";

  var spacer = document.createElement("div");
  spacer.style.height = totalHeight + "px";
  spacer.style.position = "relative";
  container.appendChild(spacer);

  var pool = document.createElement("div");
  pool.style.position = "absolute";
  pool.style.left = "0";
  pool.style.right = "0";
  spacer.appendChild(pool);

  // Pre-build gradient strings once
  var gradients = new Array(themes.length);
  for (var t = 0; t < themes.length; t++) {
    var stops = [];
    var p = themes[t].p;
    for (var i = 0; i < 20; i++) {
      var col = "#" + p.substr(i * 6, 6);
      var lo = (i * 5).toFixed(1) + "%";
      var hi = ((i + 1) * 5).toFixed(1) + "%";
      stops.push(col + " " + lo + "," + col + " " + hi);
    }
    gradients[t] = "linear-gradient(to right," + stops.join(",") + ")";
  }

  var lastStart = -1, lastEnd = -1;

  function render() {
    var scrollTop = container.scrollTop;
    var viewH = container.clientHeight;
    var start = Math.max(0, Math.floor(scrollTop / ROW_HEIGHT) - BUFFER);
    var end = Math.min(themes.length, Math.ceil((scrollTop + viewH) / ROW_HEIGHT) + BUFFER);

    if (start === lastStart && end === lastEnd) return;
    lastStart = start;
    lastEnd = end;

    var html = "";
    for (var i = start; i < end; i++) {
      var theme = themes[i];
      var enc = encodeURIComponent(theme.d);
      var top = i * ROW_HEIGHT;
      html += '<div class="theme-row" style="position:absolute;top:' + top + 'px;left:0;right:0;height:' + ROW_HEIGHT + 'px">';
      html += '<span class="theme-name" title="' + theme.d + '">' + theme.d + '</span>';
      html += '<span class="theme-links">';
      html += '<a href="/preview/#' + theme.w + '">preview</a>';
      html += '<a download href="/truecolor/' + enc + '.rc">truecolor</a>';
      html += '<a download href="/palette/' + enc + '.rc">palette</a>';
      html += '</span>';
      html += '<span class="palette-bar" style="background:' + gradients[i] + '"></span>';
      html += '</div>';
    }
    pool.innerHTML = html;
  }

  container.addEventListener("scroll", render);
  render();
})();
</script>
