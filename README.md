# Canopic Recordings website

Static site for canopicrecordings.com, hosted on Cloudflare Pages. Bandcamp handles all sales.

- `index.html` – the whole site (styles and script inline)
- `assets/` – logos, favicon, social share image
- `_redirects` – forwards old Bandcamp URLs (/album/…, /track/…, /merch) to shop.canopicrecordings.com

Cloudflare Pages settings: no framework, no build command, output directory `/`.

To add a release: add a line to the `releases` list near the bottom of `index.html` (title, artist, year, Bandcamp URL, artwork URL).
