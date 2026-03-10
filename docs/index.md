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

<hr class="section-divider">

## Screenshot

<div class="term-window index-preview">
  <div class="term-titlebar">
    <span class="blob red"></span>
    <span class="blob yellow"></span>
    <span class="blob green"></span>
    <span class="title">Compose</span>
  </div>
  <pre class="terminal">
<span class="status">q:Quit  d:Del  u:Undel  m:Mail  r:Reply  ?:Help                                                     </span>
<span class="header">        From: </span><span class="normal">Ryan Reynolds &lt;ryanr@yew.com&gt;                                                         </span>
<span class="header">          To: </span><span class="normal">Diane Wiest &lt;dianew@apple.com&gt;, Glenn Close &lt;glennc@kumquat.com&gt;          </span>
<span class="header">          Cc: </span><span class="normal">Jamie Foxx &lt;jamief@olive.com&gt;                                                   </span>
<span class="header">         Bcc: </span><span class="normal">                                                                                      </span>
<span class="header">     Subject: </span><span class="normal">Party in London                                                                       </span>
<span class="header">    Reply-To: </span><span class="normal">                                                                                      </span>
<span class="header">         Fcc: </span><span class="normal">                                                                                      </span>
<span class="header">    Security: </span><span class="sign">Sign</span><span class="normal"> (PGP/MIME)                                                                       </span>
<span class="header">     Sign as: </span><span class="normal">0x54BE8DECB4041D988854E3F2EA0E60D133D46E38                                            </span>
<span class="status">-- Attachments                                                                                      </span>
<span class="normal">- I     1 /tmp/mutt/neomutt-user-12345678                         [text/plain, 7bit, us-ascii, 0.5K]</span>
<span class="normal">  A     2 ~/dress-code.md                                         [text/markdown, 8bit, utf-8, 3.6K]</span>
<span class="status">-- Preview                                                                                          </span>
<span class="normal">Hey guys!                                                                                           </span>
<span class="normal">                                                                                                    </span>
<span class="normal">I've having a small party and you're all invited.                                                   </span>
<span class="normal">Don't forget to bring your Oscars!                                                                  </span>
<span class="normal">                                                                                                    </span>
<span class="normal">RR                                                                                                  </span>
<span class="normal">                                                                                                    </span>
<span class="status">-- NeoMutt: Compose  [Approx. msg size: 4.1K   Atts: 2]---------------------------------------------</span>
<span class="normal">                                                                                                    </span>
</pre>
</div>
