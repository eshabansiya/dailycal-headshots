# Headshot icons

Turns headshots into circular red/blue icons: background removed, photo in grayscale, placed on a colored circle. The framing matches the map's SVG pattern (7% inset, center-cropped).

## Use

1. Open `index.html` in Chrome (double-clicking it works).
2. Set the red and blue hex values to match the map's `colors`. They're saved for next time.
3. Drop in photos. Each one starts as the default color.
4. Pick red or blue for each card, or paste a list under **Paste red/blue assignments**:
   ```
   jane-doe, red
   john_smith.jpg, blue
   ```
   Names are matched against filenames, ignoring case, punctuation and extension.
5. Click **Download all (.zip)**, or download a single icon from its card.

The first photo downloads the background-removal model (about 80 MB at "Balanced"). Later runs use the browser cache. Photos are never uploaded; everything runs locally.

Background removal uses [`@imgly/background-removal`](https://github.com/imgly/background-removal-js), which is AGPL-3.0 licensed.
