# Portfolio — Uziel Rodríguez Andújar

## What's here
- `index.html` — the whole site (one file, no build step needed).
- `resume.pdf` — your current resume, linked from the nav bar and contact section.
- `images/` — empty for now, for photos/renders once you add them.

## 1. Publish it with GitHub Pages (free)

1. Go to [github.com](https://github.com) and create a new **public** repository — e.g. `portfolio`.
2. Upload these three items (`index.html`, `resume.pdf`, `images/`) to the repo. Easiest way: on the repo page, click **Add file → Upload files**, drag them in, and commit.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait ~1 minute, then your site is live at:
   `https://<your-github-username>.github.io/portfolio/`
6. (Optional) Under Settings → Pages → Custom domain, you can point a bought domain (e.g. `uzielrodriguez.com`) at it instead.

Every time you want to update the site, just re-upload the changed file to the repo (or use `git push` if you're comfortable with git) — Pages redeploys automatically in under a minute.

## 2. Swap in real photos/renders

Each project card currently has a dashed placeholder box like:

```html
<div class="img-slot">[ Add photo/render: quadcopter platform or PETG mounting bracket ]</div>
```

To replace one with a real image:
1. Drop the image file into `images/` (e.g. `images/bprl-bracket.jpg`).
2. Replace that whole `<div class="img-slot">...</div>` line with:
```html
<img src="images/bprl-bracket.jpg" alt="PETG mounting bracket" style="width:100%; border-radius:6px; display:block;">
```
Do this once per project (BPRL, LIFTS, ROCS, Power Puzzle).

## 3. Two things still need your input

- **LinkedIn link**: the "LinkedIn ↗" button in the Contact section currently points to `#` (nowhere). Find it near the bottom of `index.html` and replace `href="#"` with your actual profile URL.
- **Images**: once you connect Notion (or send the files directly), I can pull them in and do the swap above for you.

## 4. Updating content later

All the text lives directly in `index.html` as plain HTML — search for the text you want to change and edit it in place. No templating system, no dependencies.
