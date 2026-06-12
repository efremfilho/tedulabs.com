# tedulabs.com

Institutional site for **tedulabs** — technology consulting, GenAI and AI-agent building; trainings, talks and inceptions.

Brand: **t** (technology) + **edu** (education) + **labs** (experiments).

Static site, no build step.

## Structure

- `index.html` — English version (root)
- `pt-br/index.html` — Brazilian Portuguese version (`/pt-br/`)
- `styles.css` — shared styles
- `logo.svg` — logo (lab flask wearing a graduation cap + wordmark)
- `logo-dark.svg` — logo variant for dark backgrounds
- `favicon.svg` — favicon (logo mark)
- `CNAME` — custom domain for GitHub Pages

## Preview locally

Open `index.html` in a browser, or run:

```sh
python3 -m http.server 8000
```

and visit <http://localhost:8000>.

## Deploy (GitHub Pages)

1. Repository **Settings → Pages → Source**: "Deploy from a branch", branch `main`, folder `/ (root)`.
2. The `CNAME` file already sets the custom domain to `tedulabs.com`. In your DNS provider, point the apex domain to GitHub Pages (A records `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`) and `www` to `efremfilho.github.io` if desired.
3. Enable "Enforce HTTPS" once the certificate is issued.
