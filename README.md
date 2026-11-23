# Our Story map maker

A single-page tool for making matching map prints for our "Our Story So Far" book.
Key in a location, place a pin, add a title and date, then print, share or download.

## Features

- Search for a place (OpenStreetMap Nominatim), paste coordinates from Google Maps, or click/drag the pin
- Title in handwritten style, date, coordinates (DMS or decimal)
- Map styles: colour, light, dark, ink (Stadia Maps)
- Two outputs, both sized to Instax SQUARE film:
  - **Polaroid card**: 72 x 86 mm card with the caption in the white strip
  - **Instax print**: 62 x 62 mm square with the caption on the map (the film adds the frame)
- **Share to Instax / Photos** via the phone share sheet (Web Share API)
- **Print** at true size, or **Download PNG**
- Last settings are remembered in the browser (localStorage)

## Running locally

Just open `index.html` in a browser. No build step, no backend.

## Hosting

Any static host works: GitHub Pages, Netlify, Cloudflare Pages, or your own server.
Serve over HTTPS so the share sheet works on phones.

## Credits and limits

- Map data © OpenStreetMap contributors, © OpenMapTiles, tiles © Stadia Maps. Keep the attribution on the image.
- Tiles need no API key: add the site's domain (e.g. `petectw.github.io`) under Authentication in the Stadia Maps dashboard. `localhost` works without setup.
- Nominatim search is free but rate limited (about 1 request per second). Pasting coordinates always works.
