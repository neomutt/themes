---
title: Live Preview
description: Interactive preview of NeoMutt colour themes
keywords: [neomutt, email, theme, color, preview]
---

# Live Preview

<img src="_static/icon-terminal-mail.png" alt="" class="page-icon">

Pick a theme from the dropdown or click a favourite to see a live preview of NeoMutt's Compose screen.

<label for="theme-picker">Theme:</label>
<select id="theme-picker" autofocus>
  <option value="dracula" selected>Dracula</option>
  <option value="solarized">Solarized</option>
  <option value="neon">Neon</option>
  <option value="gruvbox">Gruvbox</option>
  <option value="nord">Nord</option>
  <option value="monokai">Monokai</option>
  <option value="catppuccin">Catppuccin</option>
  <option value="tokyonight">Tokyo Night</option>
</select>

<label>Favourites:</label>
<button class="fav-btn" data-theme="dracula">Dracula</button>
<button class="fav-btn" data-theme="solarized">Solarized</button>
<button class="fav-btn" data-theme="neon">Neon</button>
<button class="fav-btn" id="random-btn"><i class="fa-solid fa-shuffle"></i></i> Random</button>

## Index Dialog

```{margin}
##### Colours Used
- `sidebar_background`
- `sidebar_divider`
- `sidebar_flagged`
- `sidebar_highlight`
- `sidebar_indicator`
- `sidebar_new`
- `sidebar_ordinary`
```

<div class="term-window" data-theme="dracula">
  <div class="term-titlebar">
    <span class="blob red"></span>
    <span class="blob yellow"></span>
    <span class="blob green"></span>
    <span class="title">Index</span>
  </div>
  <pre class="terminal">
<span class="sb_background sb_flagged">Inbox [2]        63</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_ordinary">Fruit           146</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_ordinary">  Apple         379</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_indicator sb_new">  Banana      3/131</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_new">  Cherry      2/168</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_highlight sb_new">  Damson       2/62</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_ordinary">  Endive        103</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_ordinary">  Fig            66</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background sb_ordinary">  Guava         138</span><span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
<span class="sb_background">                    <span class="sb_divider"> </span><span class="index">                                                                                                    </span>
</pre>
</div>

## Compose Dialog

```{margin}
##### Colours Used
- `compose_header`
- `compose_security_sign`
- `normal`
- `status`
```
```{margin}
##### Other Colours
- `compose_security_both`
- `compose_security_encrypt`
- `compose_security_none`
- `compose_security_sign`
```

<div class="term-window" data-theme="dracula">
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

<script>
function setTheme(theme) {
  var picker = document.getElementById('theme-picker');
  var options = Array.from(picker.options).map(function(o) { return o.value; });
  if (options.indexOf(theme) === -1) return;
  document.querySelector('.term-window').setAttribute('data-theme', theme);
  picker.value = theme;
  history.replaceState(null, '', '#' + theme);
}
document.getElementById('theme-picker').addEventListener('change', function() {
  setTheme(this.value);
});
document.querySelectorAll('.fav-btn').forEach(function(btn) {
  btn.addEventListener('click', function() {
    setTheme(this.getAttribute('data-theme'));
  });
});
document.getElementById('random-btn').addEventListener('click', function() {
  var options = Array.from(document.getElementById('theme-picker').options).map(function(o) { return o.value; });
  setTheme(options[Math.floor(Math.random() * options.length)]);
});
var hash = window.location.hash.replace('#', '');
if (hash) setTheme(hash);
</script>
