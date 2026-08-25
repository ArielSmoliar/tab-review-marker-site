# Tab Review Marker

This repository hosts the public website, privacy policy, and support entry point for **Tab Review Marker**, a Chrome extension that keeps review status visible directly in the browser tab strip.

[Visit the product site](https://arielsmoliar.github.io/tab-review-marker-site/) · [Read the privacy policy](https://arielsmoliar.github.io/tab-review-marker-site/privacy.html) · [Get support](https://github.com/ArielSmoliar/tab-review-marker-site/issues)

## What Tab Review Marker does

Tab Review Marker places a compact status badge over each page’s existing favicon:

- **To Review** — slate circle
- **Reviewed** — green check
- **Needs Attention** — orange exclamation mark

The marker remains visible while you read, compare, and synthesize multiple sources. The extension can also store a note and AI-access hint, show the marked sources in the current window, and export organized source metadata as JSON or a readable table.

## Public-beta status

Version `0.1.0` has passed its release checks and is prepared for a public Chrome Web Store beta. Google’s developer-account verification is currently pending.

Public installation is not available until the Chrome Web Store listing is approved. The installation link will be added here and on the product site as soon as it is live.

## Privacy

Tab Review Marker is local by design:

- Review statuses, notes, and AI-access hints stay in Chrome’s local extension storage.
- There is no account, analytics service, advertising system, or remote backend.
- The extension does not read page-body content.
- Site access is requested one origin at a time and is used only to apply or restore favicon markers.
- Nothing is exported until the user explicitly chooses to copy or download it.
- Local review records expire after 30 days and can also be deleted manually.

AI exports contain source metadata only and label titles, URLs, and notes as untrusted input. Sensitive-looking URL fields are redacted before export.

See the full [privacy policy](https://arielsmoliar.github.io/tab-review-marker-site/privacy.html).

## Support and feedback

Use [GitHub Issues](https://github.com/ArielSmoliar/tab-review-marker-site/issues) to report a problem, request a feature, or share feedback. Do not include private browsing data, confidential URLs, or sensitive notes in an issue.

## About this repository

This is the public-facing website repository. It intentionally contains no extension source code, private review data, Store upload package, or internal project records.

GitHub Pages publishes:

- `index.html` — product overview and launch status
- `privacy.html` — Chrome Web Store privacy policy
- `styles.css` — responsive light and dark presentation
- `assets/` — public product icons

The private development repository contains the extension source, automated tests, packaging scripts, and Chrome Web Store submission assets.

## Deployment

GitHub Pages deploys the `main` branch automatically. After editing public copy:

1. Commit and push the change to `main`.
2. Wait for the **pages build and deployment** workflow to complete.
3. Verify the live product site and privacy page at desktop and mobile widths.

The public website does not collect form submissions, analytics, cookies, or user data.
