# Sentinels deck on GitHub Pages

This folder is the whole presentation website:

| File | What it is |
|---|---|
| `index.html` | The animated deck (all slides, logos, charts and code in one file) |
| `film.mp4` | The 50-second Arabic product film shown on slide 13 |
| `.nojekyll` | Tells GitHub to serve the files as they are |

When you finish, the deck will be live at:
**https://eslamnabawy.github.io/sentinels-deck/**

---

## Option A: upload in the browser (no tools needed)

### 1. Create the repository
1. Open https://github.com/new
2. **Repository name:** `sentinels-deck`
3. Choose **Public**. GitHub Pages is free only for public repositories.
4. Leave "Add a README" **unchecked**.
5. Click **Create repository**.

### 2. Upload the files
1. Unzip `sentinels-github-pages.zip` on your computer.
2. On the new repository page, click **uploading an existing file**.
3. Drag in `index.html`, `film.mp4` and `README.md`.
   - `.nojekyll` is hidden on most computers. It is optional, so you can skip it.
4. Click **Commit changes**.

### 3. Turn on GitHub Pages
1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main`, folder `/ (root)`
3. Click **Save**.

### 4. Open your link
After 1–2 minutes, refresh **Settings → Pages**. A box shows "Your site is live at…".
Open **https://eslamnabawy.github.io/sentinels-deck/** and check that the slides move and the film plays.

---

## Option B: command line (Git)

```bash
# inside the unzipped folder
git init
git add index.html film.mp4 README.md .nojekyll
git commit -m "Sentinels presentation deck"
git branch -M main
git remote add origin https://github.com/EslamNabawy/sentinels-deck.git
git push -u origin main
```

Then turn on Pages as in step 3 above.

---

## Presenting

| Action | Key / control |
|---|---|
| Next slide | → , ↓ , Space, Page Down, or click the right side |
| Previous slide | ← , ↑ , Page Up, or click the left side |
| First / last slide | Home / End |
| Speaker notes | **N** |
| Fullscreen | **F** |
| Open a specific slide | add `#s6` to the link (slide 6) |
| Phone / tablet | swipe left or right |

- Slide 9: click **Approve fix** to run the remediation demo live.
- Slide 7: click **Replay grouping** to replay the alert merge.
- Slide 13: click the film to play it with sound. Click again to pause/stop. Leaving the slide resets it.

Present in **Chrome or Edge** for the smoothest animation.

---

## Updating the deck later

1. Replace `index.html` (and `film.mp4` if the film changed) in the repository.
   In the browser, use **Add file → Upload files** and commit.
2. GitHub republishes automatically within a minute or two. The link stays the same.
3. If you still see the old version, hard-refresh with **Ctrl + Shift + R**.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| 404 page | Wait 2 minutes. Check that Pages is set to `main` / root and that the file is named exactly `index.html`. |
| Film doesn't play | Make sure `film.mp4` is uploaded next to `index.html` with exactly that name. |
| Fonts look plain | The deck loads fonts from Google Fonts, so you need an internet connection. Offline, it falls back to system fonts. |
| Settings → Pages says it needs an upgrade | The repository is private. Make it public under **Settings → General → Danger Zone → Change visibility**. |
