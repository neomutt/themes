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

<a href="preview" class="feature-card">
  <img src="_static/icon-terminal-mail.png" alt="Live preview">
  <h3>Live Preview</h3>
  <p>See exactly how each theme will look in your terminal before you install it.</p>
</a>

<a href="themes" class="feature-card">
  <img src="_static/icon-terminal-at.png" alt="Theme list">
  <h3>400+ Themes</h3>
  <p>A curated collection of TrueColor and 256-colour palettes sourced from popular terminal emulators.</p>
</a>

<a href="creating" class="feature-card">
  <img src="_static/icon-paper-plane.png" alt="Create a theme">
  <h3>Create Your Own</h3>
  <p>Learn the colour system and build a custom theme from scratch.</p>
</a>

</div>

```{toctree}
---
maxdepth: 2
hidden: true
---
preview.md
themes.md
creating.md
```

<hr class="section-divider">

## How to Install a Theme

1. Try the **[Live Preview](preview.md)** to see themes in action.
2. Visit the **[Theme List](themes.md)** and find a theme you like.
3. Click the **truecolor** or **palette** link to download the `.rc` file.
4. Save it to your NeoMutt config directory (e.g. `~/.config/neomutt/`).
5. Add a single line to your `neomuttrc`:

   ```
   source ~/.config/neomutt/dracula.rc
   ```

6. Restart NeoMutt — enjoy your new look! 🎉
