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

  var html = "";
  themes.forEach(function(theme) {
    var enc = encodeURIComponent(theme.d);
    html += '<div class="theme-row">';
    html += '<span class="theme-name" title="' + theme.d + '">' + theme.d + '</span>';
    html += '<span class="theme-links">';
    html += '<a href="/preview/#' + theme.w + '">preview</a>';
    html += '<a download href="/truecolor/' + enc + '.rc">truecolor</a>';
    html += '<a download href="/palette/' + enc + '.rc">palette</a>';
    html += '</span>';
    // Build gradient from packed colour string (20 colours × 6 hex chars)
    var stops = [];
    var n = 20;
    for (var i = 0; i < n; i++) {
      var col = '#' + theme.p.substr(i * 6, 6);
      var lo = (i / n * 100).toFixed(1) + '%';
      var hi = ((i + 1) / n * 100).toFixed(1) + '%';
      stops.push(col + ' ' + lo + ',' + col + ' ' + hi);
    }
    html += '<span class="palette-bar" style="background:linear-gradient(to right,' + stops.join(',') + ')"></span>';
    html += '</div>';
  });
  document.getElementById("theme-grid").innerHTML = html;
})();
</script>
