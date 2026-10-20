# Jeremiah Romagnoli — Personal Site

A single-file static site. No build step, no dependencies.

## Before you push — two placeholders to fix

1. **GitHub username.** Search `index.html` for `YOUR-USERNAME` (2 spots: hero links + contact) and replace with your real username.
2. **LinkedIn URL.** It's currently `linkedin.com/in/jeremiah-r-553a62215`, taken from your resume PDF — double-check that's the exact slug.
3. `cv.pdf` is a copy of the resume you already had on file (`Resume_J_174890_2__2___1___4.pdf`). If you update your resume, re-copy it over this file. The on-page CV section uses the "operationalized WRLURI as a proxy" wording you settled on (the PDF still says "instrumented").

## Push to GitHub Pages

**Option A — yourname.github.io (your main site):**
```bash
cd daniel-portfolio
git init
git add index.html cv.pdf
git commit -m "Personal site"
git branch -M main
git remote add origin git@github.com:YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```
Then in the repo: **Settings → Pages → Deploy from branch → main → Save.**
Your site goes live at `https://YOUR-USERNAME.github.io`.

**Option B — a project repo (e.g. `portfolio`):**

Same steps but remote is `git@github.com:YOUR-USERNAME/portfolio.git`;
site goes live at `https://YOUR-USERNAME.github.io/portfolio`.

## Updating later

Everything lives in `index.html` — edit the About/Projects/CV/Contact sections
directly, commit, push. Pages redeploys automatically.
