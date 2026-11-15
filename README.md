# Hiddify Deep Link Resolver & Generator

A zero-dependency static single-page web app (`index.html`) that converts Hiddify subscription URLs, proxy URIs, and configurations into shareable HTTPS wrapper links, `hiddify://` deep links, Android `intent://` links, and QR codes.

All encoding happens locally in the browser; nothing is sent to any server.

## Deploy to Cloudflare Pages

1. Push this directory to a GitHub/GitLab repo, or deploy directly from the Cloudflare dashboard (**Workers & Pages -> Create -> Pages -> Upload assets**).
2. If connecting via Git:
   - **Framework preset**: `None`
   - **Build command**: *(leave empty)*
   - **Build output directory**: `/` (or `.`)
3. Cloudflare Pages automatically applies `_headers` (`Referrer-Policy: no-referrer`, `X-Content-Type-Options: nosniff`).

## Deploy to GitHub Pages

1. Push this repository to GitHub (default branch `main` or `master`).
2. In the GitHub repository, open **Settings -> Pages -> Build and deployment -> Source** and select **GitHub Actions**.
3. The included workflow (`.github/workflows/deploy.yml`) deploys the static site automatically on push.
