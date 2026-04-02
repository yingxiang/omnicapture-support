# OmniCapture App Store Pages

This folder contains the static website used for App Store Connect metadata and product presentation.

- `index.html` → main support page, product overview, privacy, and changelog
- `privacy.html` → compatibility redirect to `index.html?tab=privacy`
- `changelog.html` → compatibility redirect to `index.html?tab=changelog`
- `assets/` → screenshots and demo images used by the page

## Language and tabs

The main page supports:

- `lang=en|zh-Hans|zh-Hant|fr|de|it|ja|ko`
- `tab=overview|privacy|changelog`

Examples:

- `index.html`
- `index.html?lang=zh-Hans`
- `index.html?lang=ja&tab=privacy`
- `index.html?lang=en&tab=changelog`

Behavior:

- `tab` defaults to `overview`
- language is auto-detected from browser settings when possible
- selected language is persisted with `localStorage`
- `privacy.html` and `changelog.html` preserve the `lang` query if present

## Publish with GitHub Pages

1. Create a public GitHub repo.
2. Upload this folder's contents.
3. In GitHub:
   - `Settings` → `Pages`
   - Source: `Deploy from a branch`
   - Branch: `main` and `/root`
4. Wait for deployment.

## App Store Connect mapping

- App Information / each localization → Support URL: `index.html`
- App Privacy → Privacy Policy URL: `privacy.html`
