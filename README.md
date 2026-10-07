# Field Notes

A responsive English walking journal, built as a static website with Leaflet 1.9.4 and OpenStreetMap tiles.

## Run locally

Run `python3 -m http.server 8765` and open `http://localhost:8765`.

## Contents

- Three complete GPS tracks, with 15,608 original coordinate points retained.
- Route cards with seven-second drawing and three-second full-route holds.
- Individual and global pause controls, enlarged interactive maps, and reduced-motion support.
- Distances computed from GPS points. Time includes stops; pace uses elapsed time. Values may differ from Fitness.
- Region count is an approximate grouping of route midpoints within 25 km, not named administrative regions.
- GPX metadata, track names, filenames, creator/device information and extensions are excluded.
- Exact route coordinates, original dates, timing and elevation are intentionally retained. The source files are not included.

This is a snapshot of the three supplied routes, not a live HealthKit connection. Map tiles require an internet connection. Leaflet is included locally under its license in `vendor/LEAFLET-LICENSE`.

## GitHub Pages

The website files are at the repository root. All URLs are relative and support project subpaths. No build or API key is required. In Settings → Pages, choose Deploy from a branch, main, and / (root), then Save. Publishing there makes the included route data available to visitors.

## Editing

Edit `index.html`, `styles.css` and `app.js`. Route data is the explicit allowlisted object in `routes.js`. Do not add raw Health exports to the repository.

Repository: https://github.com/AlexZeng3/hiking

Expected website URL after Pages is enabled: https://AlexZeng3.github.io/hiking/
