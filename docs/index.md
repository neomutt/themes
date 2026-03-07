---
title: NeoMutt Themes
description: NeoMutt Colour Schemes
keywords: [neomutt, email, theme, color]
---

# NeoMutt Themes

<div class="hero-banner">
  <h2>🎨 Personalise Your Terminal Email</h2>
  <p>Browse, preview and install colour schemes for NeoMutt — the command-line mail reader that makes email truly awesome.</p>
</div>

<div class="feature-grid">

<div class="feature-card">
  <img src="_static/hero-terminal.png" alt="Live preview">
  <h3>Live Preview</h3>
  <p>See exactly how each theme will look in your terminal before you install it.</p>
</div>

<div class="feature-card">
  <img src="_static/palette-icon.png" alt="Colour palette">
  <h3>200+ Themes</h3>
  <p>A curated collection of TrueColor and 256-colour palettes sourced from popular terminal emulators.</p>
</div>

<div class="feature-card">
  <img src="_static/setup-icon.png" alt="Easy setup">
  <h3>Easy Setup</h3>
  <p>Download a single <code>.rc</code> file and <code>source</code> it in your <code>neomuttrc</code> — done!</p>
</div>

</div>

```{toctree}
---
maxdepth: 2
hidden: true
---
preview.md
terminal.md
```

<hr class="section-divider">

## How to Install a Theme

1. Try the **[Live Preview](preview.md)** to see themes in action.
2. Visit the **[Theme List](terminal.md)** and find a theme you like.
3. Click the **truecolor** or **palette** link to download the `.rc` file.
4. Save it to your NeoMutt config directory (e.g. `~/.config/neomutt/`).
5. Add a single line to your `neomuttrc`:

   ```
   source ~/.config/neomutt/dracula.rc
   ```

6. Restart NeoMutt — enjoy your new look! 🎉
