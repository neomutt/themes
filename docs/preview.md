---
title: Live Preview
description: Interactive preview of NeoMutt colour themes
keywords: [neomutt, email, theme, color, preview]
---

# Live Preview

<img src="_static/icon-terminal-mail.png" alt="" class="page-icon">

Pick a theme from the dropdown to see a live preview of NeoMutt's Index and Compose screens.

<label for="theme-picker">Theme:</label>
<select id="theme-picker" autofocus></select>

<label>Favourites:</label>
<button class="fav-btn" data-theme="ayu">Ayu</button>
<button class="fav-btn" data-theme="dracula">Dracula</button>
<button class="fav-btn" data-theme="neon">Neon</button>
<button class="fav-btn" data-theme="solarized-dark-patched">Solarized</button>
<button class="fav-btn" data-theme="zenburn">Zenburn</button>
<button class="fav-btn" id="random-btn"><i class="fa-solid fa-shuffle"></i> Random</button>

<div id="theme-summary" class="theme-summary"></div>

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
  <pre class="terminal normal">
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
  <pre class="terminal normal">
<span class="sb_background sb_flagged">Inbox [2]        63</span><span class="sb_divider"> </span><span class="index"><span class="index_number">457 </span><span class="index_date">Jun-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">      └─&gt;Re: Use Buffers in Auto-Completion                  </span><span class="index_size">(0.4K)</span></span>
<span class="sb_background sb_ordinary">Fruit           146</span><span class="sb_divider"> </span><span class="index"><span class="index_number">458 </span><span class="index_date">Jul-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">Welcome and Thanks!                                          </span><span class="index_size">(0.5K)</span></span>
<span class="sb_background sb_ordinary">  Apple         379</span><span class="sb_divider"> </span><span class="index"><span class="index_number">459 </span><span class="index_date">Jul-25 </span><span class="index_flags">r T </span><span class="index_author">Mike Marchywka        </span><span class="index_subject">└─&gt;including modified neomutt in project(s) uploaded to githu</span><span class="index_size">(7.4K)</span></span>
<span class="sb_background sb_indicator sb_new">  Banana      3/131</span><span class="sb_divider"> </span><span class="index"><span class="index_number">460 </span><span class="index_date">Jul-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">  └─&gt;                                                        </span><span class="index_size">(0.9K)</span></span>
<span class="sb_background sb_new">  Cherry      2/168</span><span class="sb_divider"> </span><span class="index"><span class="index_number">461 </span><span class="index_date">Jul-25 </span><span class="index_flags">  L </span><span class="index_author">Mike Marchywka        </span><span class="index_subject">    └─&gt;Re: including modified neomutt in project(s) uploaded </span><span class="index_size">t(11K)</span></span>
<span class="sb_background sb_highlight sb_new">  Damson       2/62</span><span class="sb_divider"> </span><span class="index"><span class="index_number">462 </span><span class="index_date">Jul-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">Striping the Help Page                                       </span><span class="index_size">(1.6K)</span></span>
<span class="sb_background sb_ordinary">  Endive        103</span><span class="sb_divider"> </span><span class="index"><span class="index_number">463 </span><span class="index_date">Jul-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">Learning / Reviewing the Code                                </span><span class="index_size">(1.3K)</span></span>
<span class="sb_background sb_ordinary">  Fig            66</span><span class="sb_divider"> </span><span class="index new"><span class="index_number">464 </span><span class="index_date">Sep-25 </span><span class="index_flags">NsF </span><span class="index_author">Richard Russon        </span><span class="index_subject">Re: [PATCH] fix formatting of emails                         </span><span class="index_size">(4.6K)</span></span>
<span class="sb_background sb_ordinary">  Guava         138</span><span class="sb_divider"> </span><span class="index new"><span class="index_number">465 </span><span class="index_date">Sep-25 </span><span class="index_flags">NsL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">└─&gt;                                                          </span><span class="index_size">(7.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index new"><span class="index_number">466 </span><span class="index_date">Sep-25 </span><span class="index_flags">NsF </span><span class="index_author">Richard Russon        </span><span class="index_subject">  └─&gt;                                                        </span><span class="index_size">(0.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">467 </span><span class="index_date">Oct-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">NeoMutt 2025-10-06                                           </span><span class="index_size">(3.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">468 </span><span class="index_date">Oct-25 </span><span class="index_flags"> sL </span><span class="index_author">наб                   </span><span class="index_subject">└─&gt;Re: NeoMutt 2025-10-06                                    </span><span class="index_size">(4.7K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">469 </span><span class="index_date">Oct-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">NeoMutt 2025-10-25                                           </span><span class="index_size">(1.0K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">470 </span><span class="index_date">Oct-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">2025-10-25 Homebrew crash - CLI send mail                    </span><span class="index_size">(0.6K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index old"><span class="index_number">471 </span><span class="index_date">Oct-25 </span><span class="index_flags">O L </span><span class="index_author">Neomutt Developers    </span><span class="index_subject">┬─&gt;Re: Building neomutt from source                          </span><span class="index_size">(3.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index old"><span class="index_number">472 </span><span class="index_date">Oct-25 </span><span class="index_flags">OsL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">│ └─&gt;                                                        </span><span class="index_size">(5.7K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index old"><span class="index_number">473 </span><span class="index_date">Oct-25 </span><span class="index_flags">OsF </span><span class="index_author">Richard Russon        </span><span class="index_subject">└─&gt;Re: Building neomutt from source                          </span><span class="index_size">(4.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">474 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">NeoMutt 2025-11-03                                           </span><span class="index_size">(2.4K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">475 </span><span class="index_date">Nov-25 </span><span class="index_flags">rsL </span><span class="index_author">наб                   </span><span class="index_subject">└─&gt;Re: NeoMutt 2025-11-03                                    </span><span class="index_size">(6.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">476 </span><span class="index_date">Nov-25 </span><span class="index_flags">rsL </span><span class="index_author">наб                   </span><span class="index_subject">  ├─&gt;                                                        </span><span class="index_size"> (18K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">477 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">  │ └─&gt;                                                      </span><span class="index_size">(0.2K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">478 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">  └─&gt;                                                        </span><span class="index_size">(0.2K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_collapsed"><span class="index_number">479 </span><span class="index_date">Sep-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">+18) A Release is Coming!                                    </span><span class="index_size">      </span></span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">480 </span><span class="index_date">Oct-25 </span><span class="index_flags">rs* </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">Build errors in 'main'                                       </span><span class="index_size"> (10K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">481 </span><span class="index_date">Oct-25 </span><span class="index_flags"> s* </span><span class="index_author">Richard Russon        </span><span class="index_subject">├─&gt;Re: Build errors in 'main'                                </span><span class="index_size">(0.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">482 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">└─&gt;Re: Build errors in 'main'                                </span><span class="index_size"> (10K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">483 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">наб                   </span><span class="index_subject">  └─&gt;                                                        </span><span class="index_size">(5.6K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">484 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">    └─&gt;                                                      </span><span class="index_size"> (10K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">485 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">наб                   </span><span class="index_subject">      └─&gt;                                                    </span><span class="index_size"> (14K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">486 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">        └─&gt;                                                  </span><span class="index_size">(5.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index tagged"><span class="index_number">487 </span><span class="index_date">Nov-25 </span><span class="index_flags"> s* </span><span class="index_author">Carlos Henrique Lima  </span><span class="index_subject">          └─&gt;                                                </span><span class="index_size">(5.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">488 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">[PATCH] Allow crypto operations in batch mode.               </span><span class="index_size">(5.3K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">489 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">└─&gt;                                                          </span><span class="index_size">(5.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">490 </span><span class="index_date">Nov-25 </span><span class="index_flags">rsL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">[BUG] neomutt(1) refuses to send mail from stdin             </span><span class="index_size">(7.6K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">491 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">└─&gt;Re: [BUG] neomutt(1) refuses to send mail from stdin      </span><span class="index_size">(0.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_collapsed"><span class="index_number">492 </span><span class="index_date">Nov-25 </span><span class="index_flags"> sL </span><span class="index_author">Alejandro Colomar     </span><span class="index_subject">+4) [PATCH] send.c: Allow crypto operations in batch and mail</span><span class="index_size">x mode</span></span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">493 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">Aliases now support tagging                                  </span><span class="index_size">(0.9K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">494 </span><span class="index_date">Dec-25 </span><span class="index_flags">r L </span><span class="index_author">Neomutt Developers    </span><span class="index_subject">[PATCH] fix memory leak in alias_complete()                  </span><span class="index_size">(3.3K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">495 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">└─&gt;                                                          </span><span class="index_size">(0.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">496 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sF </span><span class="index_author">Richard Russon        </span><span class="index_subject">New Release next week                                        </span><span class="index_size">(0.4K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">497 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sL </span><span class="index_author">наб                   </span><span class="index_subject">└─&gt;Re: New Release next week                                 </span><span class="index_size">(5.1K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">498 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sL </span><span class="index_author">наб                   </span><span class="index_subject">  └─&gt;                                                        </span><span class="index_size">(5.5K)</span></span>
<span class="sb_background">                   </span><span class="sb_divider"> </span><span class="index"><span class="index_number">499 </span><span class="index_date">Dec-25 </span><span class="index_flags"> sL </span><span class="index_author">наб                   </span><span class="index_subject">    └─&gt;                                                      </span><span class="index_size">(9.7K)</span></span>
</pre>
</div>

<script src="/_static/theme-data.js"></script>
<script>
(function() {
  if (typeof themes === "undefined") return;

  // Unpack "p" into s (4 special) and c (16 ANSI) arrays
  function unpack(theme) {
    if (!theme._u) {
      theme.s = []; theme.c = [];
      for (var i = 0; i < 120; i += 6)
        (i < 24 ? theme.s : theme.c).push(theme.p.substr(i, 6));
      theme._u = true;
    }
  }

  // Build a lookup map for O(1) theme access
  var themeMap = {};
  themes.forEach(function(theme) { themeMap[theme.w] = theme; });

  // Populate the dropdown from theme data
  var picker = document.getElementById('theme-picker');
  themes.forEach(function(theme) {
    var opt = document.createElement('option');
    opt.value = theme.w;
    opt.textContent = theme.d;
    picker.appendChild(opt);
  });

  function buildGradient(p, start, count) {
    var stops = [];
    for (var i = 0; i < count; i++) {
      var col = '#' + p.substr((start + i) * 6, 6);
      var lo = (i / count * 100).toFixed(1) + '%';
      var hi = ((i + 1) / count * 100).toFixed(1) + '%';
      stops.push(col + ' ' + lo + ',' + col + ' ' + hi);
    }
    return 'linear-gradient(to right,' + stops.join(',') + ')';
  }

  var summary = document.getElementById('theme-summary');

  function setTheme(slug) {
    var theme = themeMap[slug];
    if (!theme) return;
    unpack(theme);
    document.querySelectorAll('.term-window').forEach(function(el) {
      theme.s.forEach(function(s, i) { el.style.setProperty('--s' + i, '#' + s); });
      theme.c.forEach(function(c, i) { el.style.setProperty('--c' + i, '#' + c); });
    });
    picker.value = slug;
    history.replaceState(null, '', '#' + slug);

    var enc = encodeURIComponent(theme.d);
    summary.innerHTML =
      '<span class="theme-summary-name">' + theme.d + '</span>' +
      '<span class="palette-special" style="background:' + buildGradient(theme.p, 0, 4) + '"></span>' +
      '<span class="palette-sep"></span>' +
      '<span class="palette-ansi" style="background:' + buildGradient(theme.p, 4, 16) + '"></span>' +
      '<div class="theme-summary-downloads">' +
        '<label>Downloads:</label>' +
        '<a download href="/truecolor/' + enc + '.rc">truecolor</a>' +
        '<a download href="/palette/' + enc + '.rc">palette</a>' +
      '</div>';
  }

  picker.addEventListener('change', function() {
    setTheme(this.value);
  });

  document.querySelectorAll('.fav-btn[data-theme]').forEach(function(btn) {
    btn.addEventListener('click', function() {
      setTheme(this.getAttribute('data-theme'));
    });
  });

  document.getElementById('random-btn').addEventListener('click', function() {
    var opts = Array.from(picker.options);
    setTheme(opts[Math.floor(Math.random() * opts.length)].value);
  });

  // Apply initial theme from hash or default to first
  var hash = window.location.hash.replace('#', '');
  setTheme(hash || 'dracula');
})();
</script>
