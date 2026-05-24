# Bouquet — Deployment Guide

## What you have
Three files to deploy:
- `bouquet.html` → rename to `index.html`
- `manifest.json`
- `sw.js`

You also need two icon images (see step 3 below).

---

## Option A — Vercel (recommended, free, 5 minutes)

1. Go to vercel.com and sign up with GitHub
2. Create a new GitHub repository (github.com → New repository → name it "bouquet")
3. Upload your files:
   - Rename `bouquet.html` to `index.html`
   - Add `manifest.json` and `sw.js`
   - Add two icon files: `icon-192.png` and `icon-512.png`
     (Use any wine-themed image, resize to 192×192 and 512×512 px)
4. In Vercel: click "Add New Project" → import your GitHub repo → click Deploy
5. Your app is live at `your-repo-name.vercel.app`
6. Optional: buy a custom domain (e.g. `bouquet.app`) and connect it in Vercel settings

---

## Option B — Netlify (also free, drag-and-drop)

1. Go to netlify.com → sign up
2. From your dashboard, drag your entire project folder onto the deploy zone
3. Done — you get a URL like `random-name.netlify.app`
4. Rename it under Site Settings → Site name

---

## Installing on your iPhone

1. Open Safari and go to your deployed URL
2. Tap the Share button (box with arrow pointing up)
3. Scroll down and tap "Add to Home Screen"
4. Name it "Bouquet" → tap Add
5. The app icon appears on your home screen and opens full-screen, no browser chrome

## Sharing with friends
Just send them the URL — same steps above to install on their phones.
Each person's wine data is stored locally on their own device.

---

## Icons (quick option)
If you don't have icons yet, create simple burgundy square images with a wine glass:
- Use canva.com → create a 512×512 design → burgundy background + white wine glass icon
- Export as PNG, resize to 192×192 for the second icon
- Name them `icon-192.png` and `icon-512.png`

---

## Current limitations (v1)
Wine entries are saved to each user's device (localStorage).
For shared social features — seeing friends' wines, profiles, etc. — a backend
database is needed (Supabase is a good free option). That's the next build step.

---

## File checklist before deploying
- [ ] index.html (renamed from bouquet.html)
- [ ] manifest.json
- [ ] sw.js
- [ ] icon-192.png
- [ ] icon-512.png
