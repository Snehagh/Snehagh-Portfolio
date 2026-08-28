# Sneha Ghosh - Portfolio

A single-file, dependency-free portfolio site positioning me for both
**Software Engineering** and **AI/ML** early-career roles. Projects are
filterable by track so recruiters can view the work through the lens of the
role they're hiring for.

**Live:** `https://Snehagh.github.io/portfolio/` (once Pages is enabled - see below)

## Stack
- Plain HTML + CSS + vanilla JS. No build step, no framework, no dependencies.
- Google Fonts (Space Grotesk, Inter, JetBrains Mono) via CDN.
- Accessible: keyboard focus states, reduced-motion support, semantic markup.

## Files
```
index.html                 # the whole site
Sneha_Ghosh_Resume.pdf     # linked from the nav + contact section
README.md
```

## Deploy on GitHub Pages
1. Create a repo (e.g. `portfolio`) and push these files to the `main` branch.
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/Snehagh/portfolio.git
   git push -u origin main
   ```
2. In the repo: **Settings → Pages → Build and deployment**.
3. Set **Source: Deploy from a branch**, **Branch: `main` / `root`**, then **Save**.
4. Wait ~1 minute. Your site is live at `https://Snehagh.github.io/portfolio/`.

> Tip: to serve it at `https://Snehagh.github.io` (no `/portfolio`), name the
> repo `Snehagh.github.io` instead.

## Editing
Everything lives in `index.html`:
- **Projects** - each is an `<article class="card" data-track="sde ai">`. The
  `data-track` value (`sde`, `ai`, or both) controls the filter and the
  ENG/AI pills. Filter counts update automatically.
- **Colors / fonts** - the `:root` CSS variables at the top.
- **Résumé** - replace `Sneha_Ghosh_Resume.pdf` with an updated file (keep the
  name, or update the two links in `index.html`).

## Preview locally
```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
