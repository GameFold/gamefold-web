# gamefold-web

Marketing and legal site for [GameFold](https://gamefold.app) — the Letterboxd for video games.

Static site served via GitHub Pages at `gamefold.app`.

## Pages

- `/` — Landing
- `/privacy.html` — Privacy Policy (GDPR / LOPDGDD / COPPA aligned)
- `/terms.html` — Terms of Service
- `/es/privacy.html`, `/es/terms.html` — Spanish versions of the two above, linked both ways
- `/delete-account.html` — Public account deletion instructions (required by Google Play)
- `/support.html` — Support & FAQ
- `/404.html` — Not-found page

The legal pages mirror the in-app text in `src/constants/legalContent.ts` (GameFold repo), in English and Spanish. Change both languages, in the app and here, together.

## Local preview

No build step. Open `index.html` in a browser, or serve locally:

```bash
npx http-server .
# or
python -m http.server
```

## Deployment

Pushes to `main` are served automatically by GitHub Pages. The `CNAME` file binds the site to `gamefold.app`. See repository Settings → Pages for configuration.

## Contact

- General: hello@gamefold.app
- Privacy: privacy@gamefold.app
- Support: support@gamefold.app
