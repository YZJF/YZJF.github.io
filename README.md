# Personal Homepage

GitHub Pages serves the academic CV site at the repo root. The designed portfolio stays local and is not published.

## Preview

```bash
cd personal-homepage
python -m http.server 4173
```

- Academic site: `http://localhost:4173`
- Designed portfolio (local only): `http://localhost:4173/portfolio.html`
- Gallery (local only): `http://localhost:4173/gallery.html`

## Publish to GitHub Pages (`yzjf.github.io`)

Publish only the academic files:

```bash
git add index.html README.md assets/avatar.png assets/Yuhan_CV.pdf
git commit -m "Publish the academic homepage."
git push origin main
```

Live site: **https://yzjf.github.io**

The résumé is `assets/Yuhan_CV.pdf`.
