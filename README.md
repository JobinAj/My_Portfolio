# Jobin AJ — Portfolio

Personal portfolio site. Single-file HTML — no build step, no dependencies, deploys in seconds.

## Deploy to Cloudflare Pages

1. Push this repo to GitHub
2. Go to [Cloudflare Pages](https://pages.cloudflare.com) → **Create a project** → Connect GitHub
3. Select this repo
4. Build settings: **Framework preset → None**, build command blank, output directory `/` (root)
5. Click **Save and Deploy**

`_headers` and `_redirects` are picked up automatically by Cloudflare Pages.

## Local preview

```bash
# Python
python3 -m http.server 8080

# Or with npx serve
npx serve .
```

Then open `http://localhost:8080`.

## Structure

```
.
├── index.html      # entire site — HTML + CSS + JS
├── favicon.svg     # JA initials favicon
├── _headers        # Cloudflare Pages security headers (CSP, HSTS, etc.)
├── _redirects      # SPA fallback route
└── assets/         # future images / files
```
