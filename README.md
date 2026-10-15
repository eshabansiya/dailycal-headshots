# Headshot icons

Turns headshots into circular icons: background removed, photo in full color, placed on a circle in its group's color. Each photo is framed automatically: the head is found in the cutout, centered, and sized to fill the circle. The shoulders stop at a thin outline of the group color around the edge.

## Use

1. Open `index.html` in Chrome (double-clicking it works).
2. Set up groups: rename each one, pick its color (color picker or hex), and use **+ Add group** for more. Groups and colors are saved for next time.
3. List the people in each group's **Names** box, one per line. Downloads are named after these.
4. Drop photos onto a group, or click **Add photos** on it. A photo whose filename contains a listed name gets that name (`jane_doe.jpg` → "Jane Doe"). The remaining names go to the remaining photos in the order they appear. To fix one, type the name on its card (it suggests names from the list). The hint under the list shows names still waiting for a photo.
5. Framing: **Head size** and **Space above head** at the top apply to every photo. If one photo comes out too tight or too loose, use the **Zoom** slider on its card. **Outline** sets the width of the band of group color around the edge, which the photo stays inside (as a % of the circle; 0 lets the shoulders run to the edge).
6. To move a photo to another group, use the dropdown on its card. Changing a group's color updates all of its icons.
7. Click **Download all (.zip)** to get one folder per group, or download a single icon from its card.

The first photo downloads the background-removal model (about 80 MB at "Balanced"). Later runs use the browser cache. Photos are never uploaded; everything runs locally.

Background removal uses [`@imgly/background-removal`](https://github.com/imgly/background-removal-js), which is AGPL-3.0 licensed.
