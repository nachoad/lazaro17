# Lázaro 17 — Project Context

## What this is

Static marketing site for **Lázaro 17**, an indie app studio. Hosted via GitHub Pages (branch: `main`). No build step — plain HTML + CSS + CDN-loaded scripts.

## File structure

```
/
├── index.html              # Main landing page
├── style.css               # Global styles (prose, hero gradient, UnoCSS overrides)
└── viveparacuellos-privacy/
    └── index.html          # Privacy policy for viveParacuellos app
```

## Tech stack

- **CSS framework**: [UnoCSS](https://unocss.dev/) runtime via CDN (`@unocss/runtime`) — utility classes are processed client-side, no build needed
- **Reset**: `@unocss/reset/tailwind.min.css`
- **Fonts**: Inter (Google Fonts)
- **Icons**: Font Awesome 6.5 Free via cdnjs (brands: `fa-apple`, `fa-google-play`)

## Design system

- Background: `zinc-950`
- Cards: `zinc-900` with `zinc-800` border
- Accent: `yellow-400`
- Text hierarchy: white → `zinc-100` → `zinc-400` → `zinc-500`
- Radius: `rounded-2xl` for cards, `rounded-xl` for badges, `rounded-full` for pill buttons
- Font: Inter

## Current apps / projects

### viveParacuellos
- **Description**: City directory app for Paracuellos del Jarama (Madrid)
- **Platforms**: iOS & Android
- **App Store**: https://apps.apple.com/es/app/viveparacuellos/id6776241644
- **Google Play**: https://play.google.com/store/apps/details?id=com.lazaro17.viveparacuellos
- **Privacy policy**: `/viveparacuellos-privacy/`
- **Bundle ID (Android)**: `com.lazaro17.viveparacuellos`

## Store badges

Store badges in the project cards use Font Awesome brand icons + two-line text layout ("Download on the / App Store", "Get it on / Google Play"). Style: black background, `rounded-xl`, `zinc-700` border.

## Git

- Repo: https://github.com/nachoad/lazaro17
- Branch: `main` (also the deploy branch)
- Git user: nachoad / nacmagic@gmail.com
- Commit messages are in Spanish, imperative mood

## Deployment

Pushing to `main` deploys automatically via GitHub Pages. No CI pipeline.
