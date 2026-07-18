# Simple Tools — website

A tiny static site (home + privacy policy). No build step, no dependencies —
just HTML and CSS.

## Files
- `index.html` — landing page
- `privacy.html` — privacy policy (use this URL in the Play Console)
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Host it on GitHub Pages

1. Create a new GitHub repo (e.g. `simpletools-site`).
2. Put these files in the repo root and push:
   ```bash
   git init
   git add .
   git commit -m "Simple Tools site"
   git branch -M main
   git remote add origin https://github.com/YOURNAME/simpletools-site.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages**.
4. Under **Build and deployment**, set **Source: Deploy from a branch**,
   **Branch: main**, folder **/ (root)**. Save.
5. Wait ~1 minute. Your site is live at:
   ```
   https://YOURNAME.github.io/simpletools-site/
   ```
   and the privacy policy at:
   ```
   https://YOURNAME.github.io/simpletools-site/privacy.html
   ```

Paste that privacy URL into the Play Console listing.

## Before you publish
- Swap the placeholder email in `privacy.html` (`hello@example.com`) for a real
  address.
- Optional: use a custom domain in **Settings → Pages → Custom domain**.

## Edit
Open the `.html` files in any editor. The internal links use root-absolute paths
(`/privacy.html`), which work on a user/organization Pages site or a custom
domain. If you host under a **project** path like
`YOURNAME.github.io/simpletools-site/`, change the links to relative
(`privacy.html` and `index.html`) or set a custom domain.
