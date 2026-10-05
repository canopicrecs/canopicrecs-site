# Canopic Recordings website

Static site for canopicrecordings.com, hosted on Cloudflare Pages. Bandcamp handles all sales.

- `index.html` – the whole site (styles and script inline)
- `assets/` – logos, favicon, social share image
- `_redirects` – forwards old Bandcamp URLs (/album/…, /track/…, /merch) to shop.canopicrecordings.com

Cloudflare Pages settings: no framework, no build command, output directory `/`.

To add a release: add a line to the `releases` list near the bottom of `index.html` (title, artist, year, Bandcamp URL, artwork URL).

## Demo submissions

`demos/index.html` posts to Web3Forms, which forwards each submission to the label inbox without the address appearing on the site. Set `ACCESS_KEY` near the bottom of that file to the key Web3Forms emails you.

## Merch

`merch/index.html` lists products from the `products` list near the bottom of the file. Products show in a grid with Tees / Hoodies / Bags filters (set by `cat`). Product photos live in `assets/merch/`. Leave `price` as "" to hide it; set `soldOut: true` to grey an item out.
