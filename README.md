# MMA Fight Timer — web app (PWA)

## Put it online free with GitHub Pages
1. On github.com, create a new **public** repository, e.g. `mma-timer`.
2. Click **Add file → Upload files**, and drag in everything in this folder
   (`index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, the `icons` folder). Commit.
3. Go to **Settings → Pages**. Under "Build and deployment", pick **Deploy from a branch**,
   branch **main**, folder **/ (root)**, then Save.
4. After a minute or two the app is live at `https://<your-username>.github.io/mma-timer/`.

## Install on iPhone
Open the link in **Safari** → tap **Share** → **Add to Home Screen** → **Add**.
It opens full screen with its own icon and works offline after the first visit.

## Updating the app
Upload the changed files, then change `CACHE = 'mmatimer-v1'` in `sw.js` to `v2`, `v3`…
so phones pick up the new version (it applies the next time the app is opened).

## Known iPhone limits of web apps
- Keep the app open on screen during a fight. iOS pauses web apps when locked or in the background;
  the clock catches up when you return, but sounds can't play while it's paused.
- If the bell is quiet or silent, check the silent switch and volume.
