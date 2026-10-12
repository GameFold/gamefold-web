# gamefold-web

Marketing and legal site for [GameFold](https://gamefold.app) — the Letterboxd for video games.

Static site served via GitHub Pages at `gamefold.app`.

## Pages

- `/` — Landing
- `/privacy.html` — Privacy Policy (GDPR / LOPDGDD / COPPA aligned)
- `/terms.html` — Terms of Service
- `/delete-account.html` — Public account deletion instructions (required by Google Play)
- `/support.html` — Support & FAQ
- `/auth/confirm/` — Sign-up email confirmation (EN/ES). The app's confirmation email links here with a one-time `token_hash`; the page verifies it with Supabase when the user taps the button. Not indexed. See [GameFold#164](https://github.com/GameFold/GameFold/issues/164) and the "Auth emails" section of `docs/SECURITY.md` in the app repo.
- `/404.html` — Not-found page

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
