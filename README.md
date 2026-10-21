# Jeremiah Romagnoli — Personal Site

Plain HTML + one shared CSS file. No build step, no dependencies.

## Site map

```
index.html            Landing page: sidebar intro (photo, name, links) + About,
                      Selected Experience, Projects, Contact
style.css             All styling, shared by every page
cv.html               Separate CV page — a live preview of cv.pdf
cv.pdf                Your CV. Replace this file and cv.html updates itself.
photo.jpg             (you add this) Your portrait — see below
projects/
  congestion-pricing.html
  housing-regulation-thesis.html
  degree-saturation.html
assets/               Project preview images (SVG placeholders — swap in your
                      own screenshots/charts anytime, same filenames)
attachments/
  senior-thesis.pdf   Linked from the thesis project page
```

## How to change things

- **Your photo:** save a picture as `photo.jpg` in the site root (same folder
  as `index.html`). It appears in the sidebar automatically. No photo yet?
  A clean "JR" placeholder shows instead.
- **CV:** the front page only carries a brief Selected Experience summary.
  The full CV lives on `cv.html`, which embeds `cv.pdf` — just overwrite
  `cv.pdf` with a newer resume export.
- **Project images:** replace the files in `assets/` with real screenshots
  or charts (keep the filenames, or update the `<img src>` in `index.html`
  and the matching project page). JPG/PNG work too — just match the extension.
- **Project attachments:** drop files in `attachments/` and link them from
  the "Links & Attachments" list at the bottom of that project's page.
  Each project page has an HTML comment showing the exact line to add.
  The thesis page already links `attachments/senior-thesis.pdf`.

## Push to GitHub Pages

The repo must be named `jeremiahsamroo.github.io` for the root URL
`https://jeremiahsamroo.github.io/` (rename under repo Settings → General
if yours is still named `jromagnoli.github.io`).

```bash
cd daniel-portfolio
git add .
git commit -m "Sidebar layout, separate CV page, project pages"
git push
```

Then in the repo: **Settings → Pages → Deploy from branch → main → Save**
(if Pages isn't already on).

## Still worth verifying

- **LinkedIn URL** is `linkedin.com/in/jeremiah-r-553a62215`, taken from your
  resume PDF — double-check that's the exact slug.
