# Local to GitHub

A SKILL.SCH lab: take a project that only exists on your laptop and publish it on GitHub.

The project is a single-page portfolio site (`index.html`, plain HTML and CSS).

## Steps

```bash
cd my-site
git init
git add index.html
git commit -m "First version of portfolio page"
git branch -M main
git remote add origin https://github.com/raphgm/localtogithub.git
git push -u origin main
```

## Check it worked

```bash
git remote -v
git log --oneline
git status   # nothing to commit, working tree clean
```

## Run the site locally

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Publish with GitHub Pages

Settings -> Pages -> Source: `main` branch, `/ (root)`. The site goes live at `https://raphgm.github.io/localtogithub/`.
