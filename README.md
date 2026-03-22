# OmniCapture App Store Pages

This folder contains static pages for App Store Connect metadata:

- `index.html` → Support URL
- `privacy.html` → Privacy Policy URL

Both pages support language switching:
- Chinese (`zh`)
- English (`en`)

They also:
- auto-detect language from browser
- persist user language with `localStorage`
- keep language in URL query (`?lang=zh` / `?lang=en`)

## 1) Before publish

Edit support email in `index.html`:

- Search `support@example.com`
- Replace with your real support email

## 2) Publish with GitHub Pages

1. Create a public GitHub repo (for example: `omnicapture-support`).
2. Upload all files in this folder (`index.html`, `privacy.html`, `README.md`).
3. In GitHub repo:
   - `Settings` → `Pages`
   - Source: `Deploy from a branch`
   - Branch: `main` and `/root`
4. Wait for deployment.

Your URLs will be:

- Support: `https://<username>.github.io/omnicapture-support/index.html`
- Privacy: `https://<username>.github.io/omnicapture-support/privacy.html`

Optional localized URLs:

- Chinese support: `.../index.html?lang=zh`
- English support: `.../index.html?lang=en`
- Chinese privacy: `.../privacy.html?lang=zh`
- English privacy: `.../privacy.html?lang=en`

## 3) App Store Connect mapping

- App Privacy → Privacy Policy URL: `privacy.html`
- App Information / each localization → Support URL: `index.html`
