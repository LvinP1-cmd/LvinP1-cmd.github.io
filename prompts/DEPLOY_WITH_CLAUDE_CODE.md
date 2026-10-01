# Claude Code Prompt — Deploy Luminaries GitHub Pages

Use the `luminaries_github_pages_kit` in this workspace to create the public developer website for Luminaries.

Do not modify the Expo React Native app during this task.

First read:
- `README.md`
- `index.html`
- `privacy.html`
- `support.html`
- `app-ads.txt`

Before deployment, identify:
1. my GitHub username and intended Pages repository
2. the support-email placeholder that still needs replacement
3. whether the `app-ads.txt` publisher ID matches the AdMob publisher ID already used by Luminaries

Never expose private credentials.

Prefer a GitHub user/organization Pages repository named:
`<github-username>.github.io`

The required AdMob URL should be:
`https://<github-username>.github.io/app-ads.txt`

Verify no secret or mobile build files are copied into this website repository, including:
- `credentials.json`
- `google-services.json`
- keystores
- service-account JSON
- Expo/EAS secret files
- environment files containing secrets

Keep this as a static HTML/CSS site. Do not introduce React, Next.js, a database, or a CMS.

Deploy using the included GitHub Pages workflow unless the repository already uses another valid Pages deployment method.

After deployment, verify:
- `/`
- `/privacy.html`
- `/support.html`
- `/app-ads.txt`

`/app-ads.txt` must return the plain AdMob line, not an HTML page.

Then report the exact public URLs to use for:
- Google Play Developer website
- Google Play Privacy policy
- Support
- AdMob app-ads.txt

Do not claim AdMob verification is complete until AdMob reports it verified.
