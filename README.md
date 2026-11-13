# DERMÉA Skin & Hair Clinic — fictional portfolio website

A static, single-page-app style website (plain HTML/CSS/JS, no build step, no dependencies). Pages are routed with URL hashes (#about, #treatments, #journal …), so no server rewrites are needed.

## Files
| File | Purpose |
|---|---|
| index.html | The whole website |
| images/ | 18 optimised WebP photos |
| favicon.svg, apple-touch-icon.png, icon-192.png, icon-512.png, site.webmanifest | Icons and app manifest |
| og-image.jpg | 1200×630 link-preview image |
| 404.html | Branded not-found page |
| robots.txt, sitemap.xml | Search-engine files |
| _headers | Security + cache headers (Netlify, Cloudflare Pages) |
| vercel.json | Same headers for Vercel |

## Before you publish
1. Replace **YOUR-DOMAIN.com** with your real domain in: index.html (canonical, og:image, og:url), robots.txt, sitemap.xml.
2. Keep the "fictional clinic" notices — the content (doctors, testimonials, contacts) is illustrative.
3. The forms are front-end demos only; they send nothing anywhere.

## Deploy (pick one)
- **Netlify:** drag the whole folder onto app.netlify.com/drop.
- **Vercel:** `npm i -g vercel`, then run `vercel` inside the folder.
- **Cloudflare Pages:** create a project → Direct Upload → upload the folder.
- **GitHub Pages:** push the files to a repo → Settings → Pages → deploy from branch (root). _headers and vercel.json are ignored there; that's fine.

## Notes
- Fonts (Cormorant Garamond, Manrope, Pinyon Script) load from Google Fonts. To self-host, download the WOFF2 files and add @font-face rules.
- Because pages use hash routes, search engines treat the site as one page. For per-page SEO, split it into real HTML files.
- The doctor and clinic photos are AI-generated; label them as such if you show the site publicly.
