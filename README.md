# Personal website — zywang0701.github.io

Static site (no build step). Every page is a self-contained `.html` file; `support.js`
is the small runtime that renders them and pulls React from a CDN at load time.

## Files
- `index.html` — Home
- `blog.html`, `teaching.html`
- `blog-stablepca.html`, `blog-cgdro.html`, `blog-causal-invariance.html`,
  `blog-dro-multisource.html`, `blog-sihr.html`
- `assets/` — wedding banner + headshot
- `support.js`, `image-slot.js` — runtime (do not edit)
- `.nojekyll` — tells GitHub Pages to serve files as-is (skip Jekyll)

## Deploy to https://zywang0701.github.io/

Your repo `zywang0701/zywang0701.github.io` uses the **master** branch. These commands
replace the old Jekyll site with this one:

```bash
git clone https://github.com/zywang0701/zywang0701.github.io.git
cd zywang0701.github.io
git checkout master

# remove the old site (keeps .git), then copy this folder's contents in:
git rm -rf .
cp -R /path/to/this/dist/. .

git add -A
git commit -m "Redesign personal website"
git push origin master
```

Then in the repo on GitHub → **Settings → Pages**, make sure the source is
**Deploy from a branch → master → / (root)**. The site goes live at
`https://zywang0701.github.io/` within a minute or two.

> Prefer to preview before replacing? Push to a `preview` branch first and set Pages to
> serve from it, or just open `index.html` locally in a browser.
