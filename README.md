# Nuxt 3 PWA Starter

**Live Demo: [https://kmrsfrnc.github.io/notes/](https://kmrsfrnc.github.io/notes/)**

A beautiful, single-page Progressive Web App (PWA) built with Nuxt 3, Vue.js, and Tailwind CSS. The app features a premium UI describing how users can install the PWA on their devices.

## Features
- **Nuxt 3 & Vue 3** - Fast, modern framework
- **Tailwind CSS** - Beautiful, customized UI with dark mode support
- **Vite PWA** - Full PWA capabilities (manifest, service worker, install prompts)
- **GitHub Pages** - Automated Static Site Generation (SSG) deployment

## Installation & Development

To run the application locally:

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Open `http://localhost:3000` to preview your changes.

## Deployment to GitHub Pages

This repository is configured to automatically deploy to GitHub Pages as a statically generated site.

### Deployment Process
1. A GitHub Actions workflow (`.github/workflows/deploy.yml`) is triggered on every push to the `main` branch.
2. The workflow installs exactly the defined npm packages via `npm ci`.
3. It generates the static site using `npx nuxt generate`.
4. The resulting output in `.output/public` is deployed instantly to the `gh-pages` environment by actions.

### Setup Instructions for your Repository
1. Push this code to a new or existing repository on GitHub.
2. In your repository settings, go to **Pages**.
3. Under **Build and deployment**, ensure the **Source** is set to **GitHub Actions**.
4. Push a new commit to the `main` branch, and the Action will automatically build and publish your app.

## How to Install the PWA

Once deployed or running locally, you can install the app on your device:

**iOS (Safari)**
1. Tap the Share button.
2. Scroll to and tap **Add to Home Screen**.
3. Tap **Add**.

**Android (Chrome)**
1. Tap the Menu icon (3 dots).
2. Tap **Install app** or **Add to Home screen**.
3. Follow the on-screen prompt to complete installation.
