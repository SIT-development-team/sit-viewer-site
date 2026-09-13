# sit-viewer-site

Support and privacy pages for the SIT Viewer mobile app, served by GitHub Pages at
<https://sit-development-team.github.io/sit-viewer-site/>.

Both URLs are filed in App Store Connect, so they must keep working and must keep their paths:

| Page    | Ukrainian      | English           |
|---------|----------------|-------------------|
| Support | `/`            | `/en/`            |
| Privacy | `/privacy.html`| `/en/privacy.html`|

Plain HTML and one stylesheet — no build step, no dependencies. Push to `main` and Pages publishes
it. To preview locally, open `index.html` in a browser, or run `python3 -m http.server` from here.

The colours in `assets/style.css` are copied from the app's own tokens (`mobile/theme/tokens.ts` in
the sit-desktop-client repo) so the site and the app read as one product.

## Editing the privacy policy

Every claim on that page was checked against the app's source, so change it only alongside a change
in the app — and change both languages together. Whenever the wording moves, update the effective
date at the top of both pages; App Review reads it.
