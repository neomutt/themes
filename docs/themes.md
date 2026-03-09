---
title: Theme List
description: List of all NeoMutt's colour themes
keywords: [neomutt, email, terminal, theme, preview]
---

# Theme List

<img src="_static/icon-terminal-at.png" alt="" class="page-icon">

Browse the full catalogue of NeoMutt colour themes below.
Each row shows the theme name, download links for **TrueColor** and **256-colour** palette files, and a swatch preview of the foreground, background, cursor, selection, and 16 ANSI colours.

Click a **truecolor** or **palette** link to download the `.rc` file, then `source` it in your `neomuttrc`.

<div id="theme-grid" class="theme-grid"></div>

<script>
(function() {
  if (typeof themes === "undefined") return;

  // Generate CSS variables for each theme
  var cssVars = "";
  themes.forEach(function(theme) {
    cssVars += '[data-theme="' + theme.w + '"] {';
    theme.s.forEach(function(s, i) { cssVars += "--s" + i + ":#" + s + ";"; });
    theme.c.forEach(function(c, i) { cssVars += "--c" + i + ":#" + c + ";"; });
    cssVars += "}\n";
  });
  var styleEl = document.createElement("style");
  styleEl.textContent = cssVars;
  document.head.appendChild(styleEl);

  // Build the grid
  var grid = document.getElementById("theme-grid");
  themes.forEach(function(theme) {
    var row = document.createElement("div");
    row.className = "theme-row";
    row.setAttribute("data-theme", theme.w);

    // Theme name
    var name = document.createElement("span");
    name.className = "theme-name";
    name.textContent = theme.d;
    name.title = theme.d;
    row.appendChild(name);

    // Download links
    var links = document.createElement("span");
    links.className = "theme-links";
    var enc = encodeURIComponent(theme.d);
    links.innerHTML =
      '<a download href="/truecolor/' + enc + '.rc">truecolor</a>' +
      '<a download href="/palette/' + enc + '.rc">palette</a>';
    row.appendChild(links);

    // Colour swatches
    var palette = document.createElement("span");
    palette.className = "palette";

    for (var i = 0; i < 4; i++) {
      var sw = document.createElement("span");
      sw.className = "swatch special-" + i;
      palette.appendChild(sw);
    }

    var sep = document.createElement("span");
    sep.className = "palette-sep";
    palette.appendChild(sep);

    for (var i = 0; i < 16; i++) {
      var sw = document.createElement("span");
      sw.className = "swatch color-" + i;
      palette.appendChild(sw);
    }

    row.appendChild(palette);
    grid.appendChild(row);
  });
})();
</script>
