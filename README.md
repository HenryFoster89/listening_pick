# listening_pick

Bi-weekly poster of albums currently being listened to. A static HTML page — no dependencies, no build step.

## How to use

1. Open `index.html` in a browser.
2. Edit the `ALBUMS` array at the top of the script with the albums of the week:

```js
const ALBUMS = [
  { artist: "Artist Name", title: "Album Title", spotifyUrl: "https://open.spotify.com/..." },
  // ...
];
```

Cover art is fetched automatically from the iTunes API. Clicking an album opens it directly on Spotify. Hovering over an album shows a tooltip with the artist name and title.

## Print

The page is optimized for printing. Use **File → Print** from the browser (or `Ctrl+P`).

- Recommended format: **30 × 30 cm**
- Make sure to enable "Print backgrounds and colors" in the print options

## Releases

### v1.0
- Initial release
- 2×2 album grid with cover art fetched from iTunes
- Bi-weekly header with Roman numeral week and year
- Click to open album on Spotify
- Hover tooltip with artist and album title
- Print-optimized layout (30×30 cm)
