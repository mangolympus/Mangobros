# 🥭 Mango Bros

A mobile-first 2D platformer built as a single self-contained HTML file (Canvas 2D + vanilla JS, no build step, no dependencies, no server required).

- 3 worlds, 7 levels
- Swipe/touch controls with a gesture mode and a button mode
- Auto-rotate landscape support, dynamic screen fitting
- Background music + sound effects
- Progress saved locally in the browser (`localStorage`)

## Running it locally
Just open `index.html` in any modern browser (double-click it, or drag it into a browser tab). No install, no server needed.

## Deploying (get a shareable link)
This repo is ready to deploy as-is on **Vercel** or **GitHub Pages** — both serve `index.html` directly with zero configuration, since there's no build step.

### Option A: Vercel (recommended)
1. Push this repo to GitHub (see below).
2. Go to [vercel.com](https://vercel.com) → **Continue with GitHub** → **Add New Project** → select this repo → **Deploy**.
3. Vercel gives you a permanent URL like `https://mango-bros.vercel.app`.

### Option B: GitHub Pages
1. Push this repo to GitHub.
2. In the repo: **Settings → Pages → Source** → select the `main` branch and `/ (root)` folder → **Save**.
3. GitHub gives you a URL like `https://yourusername.github.io/mango-bros/`.

## Updating the live game (same link)
Both platforms redeploy automatically whenever you update `index.html` on the branch they're watching — the link never changes.

- **Easiest:** on GitHub.com, open `index.html` in the repo → click the pencil (Edit) icon → paste in the new version → **Commit changes**.
- **Or via git:**
  ```bash
  git add index.html
  git commit -m "Update game"
  git push
  ```

Either way, Vercel/GitHub Pages picks up the change and republishes to the same URL, usually within well under a minute.

## Notes
- The file is ~2MB (it embeds the character art and background music directly as base64, so the whole game is one portable file). This is well within the limits of both platforms.
- Progress/settings are saved per-browser via `localStorage` — clearing site data or switching browsers/devices resets progress.
