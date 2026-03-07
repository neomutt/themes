---
title: Creating a Theme
description: How to create your own NeoMutt colour theme
keywords: [neomutt, email, theme, color, create, customize]
---

# Creating a Theme

<img src="_static/icon-paper-plane.png" alt="" class="page-icon">

Want to build your own NeoMutt colour scheme?
This guide walks you through the colour system, the configuration syntax, and the anatomy of a theme file.

## Colour Modes

NeoMutt supports three ways to specify colours, depending on what your terminal can display:

| Mode | Colours | Syntax example | Config setting |
|---|---|---|---|
| **Basic** | 16 ANSI colours | `red`, `brightblue` | *(default)* |
| **256-colour palette** | 256 indexed colours | `color141`, `color236` | *(default)* |
| **TrueColor** | 16 million colours | `#bd93f9`, `#282a36` | `set color_directcolor = yes` |

TrueColor gives the most accurate results but requires a modern terminal emulator.
The 256-colour palette is a close approximation that works almost everywhere.

## The `color` Command

Every colour rule in NeoMutt follows the same pattern:

```
color <object>  <foreground>  <background>  [<pattern>]
```

- **object** — what part of the UI to colour (see the table below).
- **foreground** — text colour.
- **background** — background colour.
- **pattern** — *(optional)* a regex that restricts the rule to matching lines.

### Colour Objects

NeoMutt has many colour objects.  Here are the most commonly themed ones:

| Object | Where it appears |
|---|---|
| `normal` | Default text everywhere |
| `error` | Error messages |
| `message` | Informational messages |
| `indicator` | The highlighted / selected line |
| `tree` | Thread-tree arrows in the index |
| `status` | The status bar |
| `index` | Rows in the message index |
| `index_number` | Message number column |
| `index_author` | Author column |
| `index_subject` | Subject column |
| `index_date` | Date column |
| `index_flags` | Flag indicators (N, D, etc.) |
| `hdrdefault` | Default header colour in the pager |
| `header` | Specific header lines (with a pattern) |
| `body` | Message body text (with a pattern) |
| `quoted0`–`quoted9` | Levels of quoted text |
| `signature` | Email signature |
| `search` | Search-match highlight |
| `compose_header` | Headers in the compose screen |
| `compose_security_encrypt` | Encryption indicator |
| `compose_security_sign` | Signature indicator |
| `compose_security_both` | Sign + encrypt indicator |

## Basic Colour Names

The 16 ANSI colours available everywhere:

```
black   red     green   yellow   blue   magenta   cyan   white
```

Prefix with `bright` for the high-intensity variant: `brightred`, `brightgreen`, etc.

Use `default` to inherit the terminal's own foreground or background.

## 256-Colour Palette

Use `color0` through `color255`.  The first 16 (`color0`–`color15`) map to the
ANSI colours above; `color16`–`color231` are a 6×6×6 colour cube; and
`color232`–`color255` are a greyscale ramp.

```
color normal  color255  color236
color status  color141  color61
```

## TrueColor (24-bit)

Enable TrueColor at the top of your theme file, then use `#RRGGBB` hex values:

```
set color_directcolor = yes

color normal  #f8f8f2  #282a36
color status  #f8f8f2  #6272a4
```

## Anatomy of a Theme File

A complete theme file is a plain-text NeoMutt config (`.rc`) with colour commands
grouped into logical sections.  Here is a minimal example:

```
# My Theme – NeoMutt colour scheme
#
# Base palette
# bg:  #1a1b26
# fg:  #c0caf5

set color_directcolor = yes

# Global defaults
color normal      #c0caf5  #1a1b26
color error       #f7768e  #1a1b26
color message     #7aa2f7  #1a1b26
color indicator   #1a1b26  #e0af68
color tree        #565f89  #1a1b26

# Status bar
color status      #c0caf5  #24283b

# Index
color index            #c0caf5  #1a1b26
color index_author     #bb9af7  #1a1b26
color index_subject    #c0caf5  #1a1b26
color index_date       #e0af68  #1a1b26
color index  #f7768e  #1a1b26  "~D"   # deleted
color index  #e0af68  #1a1b26  "~T"   # tagged

# Headers
color hdrdefault  #c0caf5  #1a1b26
color header      #bb9af7  #1a1b26  "^From:"
color header      #e0af68  #1a1b26  "^Subject:"

# Body & quoting
color body        #c0caf5  #1a1b26  ".*"
color quoted0     #73daca  #1a1b26
color quoted1     #7aa2f7  #1a1b26
color signature   #565f89  #1a1b26
color body        #7dcfff  #1a1b26  "(https?|ftp)://[^ ]+"

# Compose
color compose_header           #bb9af7  #1a1b26
color compose_security_sign    #9ece6a  #1a1b26
color compose_security_encrypt #f7768e  #1a1b26
```

## Tips for a Good Theme

- **Start from a base palette.**  Pick a background, a foreground, and an accent
  colour, then derive the rest.
- **Keep contrast high.**  The index and status bar are scanned quickly — make
  sure they are easy to read.
- **Use quoted colours to show depth.**  `quoted0` through `quoted3` is usually
  enough; alternate between warm and cool tones.
- **Highlight URLs and diffs.**  A `body` rule with a URL regex and diff markers
  (`^+`, `^-`, `^@@`) makes patches much easier to read.
- **Test both light and dark terminals.**  If your terminal has a light
  background, your theme's dark background will override it — but make sure it
  still looks intentional.

## Installing Your Theme

Save your file as `~/.config/neomutt/mytheme.rc`, then add one line to your
`neomuttrc`:

```
source ~/.config/neomutt/mytheme.rc
```

Restart NeoMutt and you're done!
