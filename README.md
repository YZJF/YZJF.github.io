# Personal Homepage

A static, two-page portfolio. No build step.

## Preview

```bash
cd personal-homepage
python -m http.server 4173
```

Open `http://localhost:4173`. Gallery is a separate page at `http://localhost:4173/gallery.html` and is not previewed on the home page.

## Publish to GitHub Pages (`yzjf.github.io`)

GitHub Pages for a user site must live in a public repo named exactly `YZJF.github.io`.

If that repo does not exist yet:

```bash
cd personal-homepage
git init
git checkout -b main
git add index.html gallery.html README.md assets
git commit -m "Publish personal homepage."
gh repo create YZJF.github.io --public --source=. --remote=origin --push
```

If the repo already exists:

```bash
cd personal-homepage
git remote add origin https://github.com/YZJF/YZJF.github.io.git
git checkout -b main
git add index.html gallery.html README.md assets
git commit -m "Update personal homepage."
git push -u origin main
```

Then:

1. Open **https://github.com/YZJF/YZJF.github.io/settings/pages**
2. **Build and deployment → Source:** Deploy from a branch
3. Branch: `main`, folder: `/ (root)`
4. Wait a minute, then open **https://yzjf.github.io**

The home page is `index.html`. Gallery lives on `gallery.html`. Images stay under `assets/gallery/`; the room background is `assets/room-background.webp`.
