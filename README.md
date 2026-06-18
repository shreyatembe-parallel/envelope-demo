# Gullak · Envelope Opening Animation

A tap-to-open envelope animation prototype: the envelope opens, the postcard
emerges as the envelope fades back, then enlarges and centers with a closing
message and CTA.

Open `index.html` in any browser — no build step.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire demo (HTML + CSS + JS, self-contained) |
| `Back.svg`, `Middle.svg`, `Bottom.svg` | Envelope body layers |
| `Top-Close.svg`, `Top-Open.svg` | Closed / open flap faces |
| `Postcard.png` | The postcard shown inside |
| `.nojekyll` | Tells GitHub Pages to serve all files as-is |
| `Postcards/` | Alternate postcard designs (not used by default) |
| `server.js` | Optional local static server (`node server.js`) — not needed for Pages |

## Deploy to GitHub Pages

This folder is a self-contained git repo. Publish it:

```bash
# from inside this folder
git init
git add .
git commit -m "Envelope opening animation"
git branch -M main
git remote add origin https://github.com/<you>/<repo>.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Build and deployment**
- Source: **Deploy from a branch**
- Branch: **main** / **/ (root)** → Save

Your demo will be live at `https://<you>.github.io/<repo>/` within a minute or two.

> Note: GitHub Pages is case-sensitive. The asset filenames in `index.html`
> match the files exactly (e.g. `Top-Close.svg`), so don't rename their casing.
