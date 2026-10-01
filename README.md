# Woordentrainer

Dutch vocabulary practice app, packaged as a Progressive Web App (PWA) for GitHub Pages.

## Publish on GitHub Pages

1. Create a new GitHub repository.
2. Upload **all files and folders in this directory** to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the branch containing these files (usually `main`) and folder `/ (root)`.
6. Save and wait for GitHub Pages to publish the site.
7. Open the resulting `https://...github.io/.../` address on your phone.
8. On iPhone use **Share → Add to Home Screen**. On Android use **Install app** / **Add to Home screen**.

## Progress and offline use

The app stores progress locally in the browser using `localStorage`. The service worker also caches the app so it can continue to load offline after the first successful visit.

Use the app's own export/import backup feature when moving progress between devices or browsers.

## Updating the app

When you publish a substantially changed version, increase the `CACHE` value in `sw.js` (for example `woordentrainer-v3`) so installed copies pick up the new files.
