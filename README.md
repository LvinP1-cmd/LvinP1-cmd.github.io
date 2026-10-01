# Luminaries GitHub Pages Kit

This free static site provides:
- an official developer website for Google Play
- a Privacy Policy URL
- a Support URL
- a root-level `app-ads.txt` for AdMob verification

## Recommended repository

For the cleanest AdMob setup, create a GitHub **user or organization Pages** repository named exactly:

`YOUR_GITHUB_USERNAME.github.io`

Copy this kit into that repository root.

Your URLs will be:

- `https://YOUR_GITHUB_USERNAME.github.io/`
- `https://YOUR_GITHUB_USERNAME.github.io/privacy.html`
- `https://YOUR_GITHUB_USERNAME.github.io/support.html`
- `https://YOUR_GITHUB_USERNAME.github.io/app-ads.txt`

The last URL is important because AdMob expects `app-ads.txt` at the hostname root.

## Before publishing

1. Replace `support@your-domain.example` in `support.html`.
2. Review `privacy.html` against your actual Play Console Data safety answers and final SDK list.
3. In AdMob, open the app-ads.txt setup page and compare its personalized line with this kit's `app-ads.txt`.
4. If AdMob shows a different publisher line, replace the file with the exact line AdMob gives you.

Current line in this kit:

`google.com, pub-5403736045950469, DIRECT, f08c47fec0942fa0`

## Enable GitHub Pages

The kit includes a GitHub Actions Pages workflow.

Go to:

`Repository → Settings → Pages → Build and deployment → Source → GitHub Actions`

Push to `main`.

Alternatively, remove `.github/workflows/pages.yml` and deploy directly from the `main` branch root.

## Google Play

Use:

Developer website:
`https://YOUR_GITHUB_USERNAME.github.io`

Privacy policy:
`https://YOUR_GITHUB_USERNAME.github.io/privacy.html`

Support:
`https://YOUR_GITHUB_USERNAME.github.io/support.html`

## AdMob

Verify this works publicly as plain text:

`https://YOUR_GITHUB_USERNAME.github.io/app-ads.txt`

Then allow AdMob time to crawl it. Do not claim verification is complete until AdMob itself reports that it is verified.

## Avoid project-only Pages paths

A URL such as:

`https://YOUR_GITHUB_USERNAME.github.io/luminaries/`

is less suitable for app-ads.txt unless the hostname root also serves the required file. A user/organization site avoids that issue.

## Custom domain later

You can add a custom domain later. When you do, update the Google Play Developer website and make sure the custom domain serves `/app-ads.txt` at its root.
