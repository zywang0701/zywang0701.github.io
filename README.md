# Personal website — Zhenyu (Zach) Wang

Static HTML/CSS website for https://zywang0701.github.io/. No build step or JavaScript runtime is needed.

## Pages
- `index.html`: profile, recent news, and three selected research projects
- `research.html`: seven papers grouped by research theme
- `teaching.html`: existing teaching records and resource links
- `styles.css`: shared responsive layout and typography

SIHR is linked from its paper. The former paper-explanation blogs and standalone software section have been removed. A future blog can be added for ideas and work habits.

## Preview
Run `python -m http.server 8000` in this folder, then open http://localhost:8000/.

## Academic CV
The current academic CV is at assets/Zhenyu_Wang_Resume.pdf. The navigation and homepage link to this PDF. The existing URL is retained for compatibility.

## GitHub Pages
Review locally before publishing. Copy the changed HTML, `styles.css`, and `papers/PRICE_ICLR.pdf` into the existing repository, and remove the six former `blog*.html` files. Preserve unrelated files, including any separately hosted SIHR project. Commit and push to the existing Pages source branch (the supplied repository uses `master`).
