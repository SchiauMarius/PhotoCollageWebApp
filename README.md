# Photo Collage

Upload 3–7 photos; the app picks a matching template and lets you download the collage as a PNG.
Everything runs in the browser — photos never leave your machine.

## Run on localhost

Double-click `start.bat` (needs Python), or from this folder run:

    python -m http.server 5173

Then open http://localhost:5173

## Files

- `index.html` – page layout
- `style.css` – styling
- `app.js` – upload handling, templates (`TEMPLATES`), canvas drawing, download

## Adding templates

In `app.js`, add an entry to `TEMPLATES[count]`: a list of `[x, y, w, h]` rectangles (0–1 units) — one per photo.
