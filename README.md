# RadialDeck themes

Community ring styles for [RadialDeck](https://github.com/StefanKasamakov/radialdeck-releases), the native Windows radial menu.

## Use a theme

1. Download a `.json` from `themes/`.
2. Put it in `%APPDATA%\RadialDeck\themes\` (RadialDeck Settings → the `…` button next to the style dropdown opens that folder).
3. Reopen Settings and pick it under **Style**. The ring preview and the real ring change immediately.

## Make a theme

Copy `themes/glass.json`, change `id` and `name`, edit the colours. Every colour is `#RRGGBB` or `#AARRGGBB` (alpha first). Both a `dark` and a `light` block are required; RadialDeck picks one to match Windows.

| Field | What it paints |
|---|---|
| `sliceTop`, `sliceBottom` | vertical gradient of a slice |
| `sliceStroke` | slice outline |
| `hoverTop`, `hoverBottom`, `hoverStroke` | the highlighted slice |
| `hub` | the centre disc |
| `label`, `labelDim`, `labelEmpty` | text on the highlighted slice, on the others, and on empty slices |
| `shadow` | drop-shadow colour under the ring |
| `strokeWidth` | outline width in px (0–6) |
| `shadowOpacity` | 0–1 |

A bad colour shows as magenta so you spot it at once. A theme whose `id` matches a built-in one replaces it.

## Share a theme

Open a pull request that adds `themes/<id>.json` and a 300×300 screenshot `previews/<id>.png` (Settings → the preview card, or the ring itself over a plain wallpaper). Keep `author` as you want to be credited.

Built-in themes (`glass`, `midnight`, `neon`, `paper`, `nord`, `catppuccin-mocha`, `dracula`, `terminal`, `sunset`, `mono`) ship with the app and are mirrored here as examples.
