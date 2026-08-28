# Sneha Ghosh - Portfolio

A single-file, dependency-free portfolio site positioning me for both
**Software Engineering** and **AI/ML** early-career roles. Projects are
filterable by track so recruiters can view the work through the lens of the
role they're hiring for.

**Live:** https://snehagh.github.io/Snehagh-Portfolio/

## Stack
- Plain HTML + CSS + vanilla JS. No build step, no framework, no dependencies.
- Google Fonts (Space Grotesk, Inter, JetBrains Mono) via CDN.
- Accessible: keyboard focus states, reduced-motion support, semantic markup.

## Files
​```
index.html                 # the whole site
Sneha_Ghosh_Resume.pdf     # linked from the nav + contact section
README.md
​```

## Editing
Everything lives in `index.html`:
- **Projects** - each is an `<article class="card" data-track="sde ai">`. The `data-track` value (`sde`, `ai`, or both) controls the filter and the ENG/AI pills. Filter counts update automatically.
- **Colors / fonts** - the `:root` CSS variables at the top.
- **Resume** - replace `Sneha_Ghosh_Resume.pdf` with an updated file (keep the name, or update the two links in `index.html`).
