# listening_pick

Bi-weekly poster of albums currently being listened to. A static HTML page — no dependencies, no build step.

## How to use

1. Open `index.html` in a browser.
2. Edit the `ALBUMS` array at the top of the script with the albums of the week:

```js
const ALBUMS = [
  {
    artist: "Artist Name",
    title: "Album Title",
    description: "Optional editorial note (shown in 'L'angolo del Folleggiante').",
    reviewUrl: "https://...",   // optional — shows a "La recensione →" link
    spotifyUrl: "https://open.spotify.com/...",
  },
  // ...
];
```

Cover art is fetched automatically from the iTunes API. Clicking an album opens it directly on Spotify. Hovering over an album shows a side panel with metadata and optional editorial content.

## Print

The page is optimized for printing. Use **File → Print** from the browser (or `Ctrl+P`).

- Recommended format: **30 × 30 cm**
- Make sure to enable "Print backgrounds and colors" in the print options

## Releases

### v1.1
- Side panel on hover with album metadata (year, label, producer)
- Metadata fetched automatically from iTunes + Discogs
- Panel appears left or right depending on album column, without shifting the poster
- "L'angolo del Folleggiante" editorial section (shown when `description` is set)
- "La recensione →" link (shown when `reviewUrl` is set)

### v1.0
- Initial release
- 2×2 album grid with cover art fetched from iTunes
- Bi-weekly header with Roman numeral week and year
- Click to open album on Spotify
- Hover tooltip with artist and album title
- Print-optimized layout (30×30 cm)
