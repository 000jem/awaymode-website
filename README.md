# holt-website

Static site for **Holt**, the iOS focus app.

Three pages, one stylesheet, no build step:

- `index.html` — landing
- `privacy.html` — privacy policy
- `support.html` — support / FAQ
- `assets/style.css` — shared styles

## Local preview

```bash
python3 -m http.server 8080
```

Open <http://localhost:8080>.

## Deploy

GitHub Pages serves directly from `main`. Settings → Pages → Source: *Deploy
from a branch* → `main` / `/ (root)`.

After the first deploy the URLs are:

- `https://000jem.github.io/holt-website/`
- `https://000jem.github.io/holt-website/privacy.html`
- `https://000jem.github.io/holt-website/support.html`

Those are the URLs to paste into App Store Connect → App Privacy and App
Information.

## Brand

Visual tokens are pulled from the iOS app's warm-dark ember palette and
defined as CSS custom properties at the top of `assets/style.css`. Two
typefaces, both from Google Fonts:

- **Fraunces** (semibold 600) — wordmark and headings
- **Jost** (400/500/600) — body and UI

Keep it quiet.
