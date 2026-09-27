# ร่วมมือหรือหักหลัง · Prisoner's Dilemma Arena

An interactive explainer of the repeated prisoner's dilemma and Axelrod's strategy tournaments. You can play a few rounds yourself, watch classic strategies face each other, run round-robin tournaments and evolution, and build your own strategy.

- **Thai** (home page): `index.html`
- **English**: `en/index.html`

Each page has a language switch in its top bar that keeps the tab you're on.

## What's in this folder

| File | What it is |
| --- | --- |
| `index.html` | The Thai site |
| `en/index.html` | The English site |
| `favicon.svg`, `apple-touch-icon.png` | Browser-tab and home-screen icons |
| `.nojekyll` | A hidden, empty file that tells GitHub Pages to serve the files as they are. If your upload leaves it out, the site still works. |

It's a static site with no build step and no dependencies. Everything runs in the visitor's browser, and only the fonts come from Google Fonts. To preview it locally, double-click `index.html`.

## Publish on GitHub Pages

1. Create a new **public** repository on GitHub, for example `dilemma-arena`. On a free account, Pages needs a public repository.
2. On the repository page, choose **Add file → Upload files**. Drag the *contents* of this folder into the page (`index.html`, the `en` folder and the icons), not the folder itself. Then click **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then click **Save**.
4. After a minute or two the site is live at:
   - Thai: `https://<your-username>.github.io/dilemma-arena/`
   - English: `https://<your-username>.github.io/dilemma-arena/en/`

If you name the repository `<your-username>.github.io`, the site is served from `https://<your-username>.github.io/` instead.

To update the site later, upload the changed file again with the same name and commit. Pages redeploys automatically.

If you use git instead:

```bash
cd dilemma-arena
git init -b main
git add .
git commit -m "Prisoner's Dilemma Arena"
git remote add origin https://github.com/<your-username>/dilemma-arena.git
git push -u origin main
```

## Notes

- Strategies people build are saved in their own browser (localStorage). Nothing is sent to a server.
- Share codes (`PDA1.…`) work in both the Thai and English versions.
- Links to a specific tab work, for example `…/dilemma-arena/#tournament` or `…/en/#evolution`.
