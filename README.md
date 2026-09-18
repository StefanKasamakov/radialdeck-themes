# RadialDeck themes

Community ring styles for [RadialDeck](https://github.com/StefanKasamakov/radialdeck-releases), the native Windows radial menu.

## Use a theme

1. Download a `.json` from `themes/`.
2. Put it in `%APPDATA%\RadialDeck\themes\` (RadialDeck Settings → the `…` button next to the style dropdown opens that folder).
3. Reopen Settings and pick it under **Style**. The ring preview and the real ring change immediately.

## Make a theme

**The easy way:** open the [theme studio](https://stefankasamakov.github.io/radialdeck-releases/themes.html).
Pick a theme to start from, move the colours around with a live ring next to you, then either download the
file or press "Share it on GitHub", which opens this repository with your theme already filled in and ready
to commit as a pull request. Nothing to install and no account beyond GitHub.

**By hand:** copy `themes/glass.json`, change `id` and `name`, edit the colours. Every colour is `#RRGGBB` or `#AARRGGBB` (alpha first). Both a `dark` and a `light` block are required; RadialDeck picks one to match Windows.

| Field | What it paints |
|---|---|
| `sliceTop`, `sliceBottom` | vertical gradient of a slice |
| `sliceStroke` | slice outline |
| `hoverTop`, `hoverBottom`, `hoverStroke` | the highlighted slice |
| `hub` | the centre disc |
| `label`, `labelDim`, `labelEmpty` | text on the highlighted slice, on the others, and on empty slices |
| `shadow` | drop-shadow colour under the ring |
| `strokeWidth` | outline width in px (0-6) |
| `shadowOpacity` | 0-1 |
| `pattern` | overlay on every slice: `none`, `pixels` (Minecraft blocks), `gloss` (Aero shine), `stripes`, `dots`, `scanlines`, `grid` |
| `patternColor` | colour of the pattern; its alpha is the strength |
| `glow`, `glowRadius` | glow around the highlighted slice (`""` = none) |
| `font` | label font family, must be installed (`Consolas`, `Segoe UI Black`, `Georgia`...) |
| `labelSize` | label size in px, 0 = automatic |
| `labelUppercase` | `true` to shout |

A bad colour shows as magenta so you spot it at once. A theme whose `id` matches a built-in one replaces it.

## Built-in themes

| Theme | Dark | Light |
|---|---|---|
| **Blueprint** `blueprint` | ![](previews/blueprint-dark.png) | ![](previews/blueprint-light.png) |
| **Catppuccin Mocha** `catppuccin-mocha` | ![](previews/catppuccin-mocha-dark.png) | ![](previews/catppuccin-mocha-light.png) |
| **Cyberpunk** `cyberpunk` | ![](previews/cyberpunk-dark.png) | ![](previews/cyberpunk-light.png) |
| **Dracula** `dracula` | ![](previews/dracula-dark.png) | ![](previews/dracula-light.png) |
| **Frost** `frost` | ![](previews/frost-dark.png) | ![](previews/frost-light.png) |
| **Glass** `glass` | ![](previews/glass-dark.png) | ![](previews/glass-light.png) |
| **Gridline** `gridline` | ![](previews/gridline-dark.png) | ![](previews/gridline-light.png) |
| **Inferno** `inferno` | ![](previews/inferno-dark.png) | ![](previews/inferno-light.png) |
| **Midnight** `midnight` | ![](previews/midnight-dark.png) | ![](previews/midnight-light.png) |
| **Minecraft** `minecraft` | ![](previews/minecraft-dark.png) | ![](previews/minecraft-light.png) |
| **Mono** `mono` | ![](previews/mono-dark.png) | ![](previews/mono-light.png) |
| **Neon** `neon` | ![](previews/neon-dark.png) | ![](previews/neon-light.png) |
| **Nord** `nord` | ![](previews/nord-dark.png) | ![](previews/nord-light.png) |
| **Onyx & Gold** `gold` | ![](previews/gold-dark.png) | ![](previews/gold-light.png) |
| **Overworld** `overworld` | ![](previews/overworld-dark.png) | ![](previews/overworld-light.png) |
| **Paper** `paper` | ![](previews/paper-dark.png) | ![](previews/paper-light.png) |
| **Retro Handheld** `handheld` | ![](previews/handheld-dark.png) | ![](previews/handheld-light.png) |
| **Sakura** `sakura` | ![](previews/sakura-dark.png) | ![](previews/sakura-light.png) |
| **Stealth** `stealth` | ![](previews/stealth-dark.png) | ![](previews/stealth-light.png) |
| **Sunset** `sunset` | ![](previews/sunset-dark.png) | ![](previews/sunset-light.png) |
| **Synthwave** `synthwave` | ![](previews/synthwave-dark.png) | ![](previews/synthwave-light.png) |
| **Terminal** `terminal` | ![](previews/terminal-dark.png) | ![](previews/terminal-light.png) |
| **Test Chamber** `lab` | ![](previews/lab-dark.png) | ![](previews/lab-light.png) |
| **Vault** `vault` | ![](previews/vault-dark.png) | ![](previews/vault-light.png) |
| **Windows 7 Aero** `aero` | ![](previews/aero-dark.png) | ![](previews/aero-light.png) |

## Share a theme

Open a pull request that adds `themes/<id>.json` and a 300×300 screenshot `previews/<id>.png` (Settings → the preview card, or the ring itself over a plain wallpaper). Keep `author` as you want to be credited.

