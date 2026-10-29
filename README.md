# Nur Shamilla Selamat — 3D portfolio

A single-file site (`index.html`) built with three.js. No build step.

## Live site

https://shmllslmt.github.io/ (GitHub Pages, from the `main` branch of `shmllslmt/shmllslmt.github.io`).

`siteUrl` in the `CONFIG` block of `index.html` is set to that address, so the QR code's "Portfolio link" mode opens it. "Save contact" mode adds your name, title, email and LinkedIn to the scanner's phone.

To publish a change, commit and push to `main`; the site updates within a minute or two.

## Updating content

Everything is in the `window.DATA` block in `index.html`:

- `pubs`: papers and presentations (`type` is `journal`, `proceedings`, `seminar` or `talk`)
- `awards`: `l` is `gold`, `silver`, `bronze` or `special`; `s` is the short name shown on project cards
- `projects`: `aw` lists award keys (`k`) and `pub` is a paper key
- `certs`, `jury`

Counts in the 3D scene (papers, awards, jury roles) update on their own.

## Preview locally

```bash
python3 -m http.server 5173
```

Then open http://localhost:5173.
