# pawel-motyka.github.io

Personal research website of Paweł Motyka, built with [Quarto](https://quarto.org) and published on GitHub Pages by GitHub Actions on every push to `main`.

## Editing

| What | Where |
|---|---|
| Bio, research summary, teaching | `index.qmd` |
| Publications (one YAML entry per paper; "Motyka, P." is bolded automatically) | `publications.yml` |
| Talks | `publications.qmd` |
| Ongoing projects, funding | `projects.qmd` |
| Repositories | `code.qmd` |
| Colours and fonts | `styles/` |
| Photo | put `assets/photo.jpg` and swap the monogram line in `index.qmd` |

Local preview: `quarto preview`.

## One-time setup

1. **Settings → Pages → Build and deployment → Source: GitHub Actions.**
2. After buying the domain: **Settings → Pages → Custom domain:** `pawelmotyka.com`, then **Enforce HTTPS**. In the registrar's DNS, add the four GitHub Pages `A` records (and `AAAA` records) for the apex domain and a `CNAME` record `www → pawel-motyka.github.io`; with Cloudflare, keep these records set to *DNS only*. Verify the domain under the GitHub account's **Settings → Pages**. Finally, change `site-url` in `_quarto.yml` to `https://pawelmotyka.com`.
