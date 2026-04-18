# Dream Planners — Mum Engagement Tool

Deploy this to your existing GitHub Pages repo (`jasondporganisation.github.io`) and it goes live at:

**`https://jasondporganisation.github.io/mum-tool/`**

Co-branded for Dream Planners Group × Great Eastern Life.

---

## 📁 What's in this package

```
mum-tool/
├── index.html        ← The app itself
├── manifest.json     ← PWA config (makes it installable on iPad)
├── icon-192.png      ← App icon (iPad home screen)
├── icon-512.png      ← App icon (larger, for splash screen)
├── dp-logo-full.png  ← Dream Planners full logo (mark + wordmark)
├── dp-mark.png       ← Dream Planners mark only (transparent PNG)
└── README.md         ← This file
```

---

## 🚀 Deploy in 3 minutes

### Option A — Using your Mac Terminal (fastest)

Open Terminal and paste these commands one by one. Replace `~/path/to/jasondporganisation.github.io` with your actual local repo path.

```bash
# 1. Go to your local repo folder
cd ~/path/to/jasondporganisation.github.io

# 2. Make sure you're on the latest
git pull

# 3. Copy the mum-tool folder here
#    (Assumes you downloaded mum-tool-package to Downloads)
cp -r ~/Downloads/mum-tool-package/mum-tool ./

# 4. Commit and push
git add mum-tool/
git commit -m "Add DPG Mum Engagement Tool"
git push

# 5. Wait ~1 minute, then visit:
#    https://jasondporganisation.github.io/mum-tool/
```

That's it. GitHub Pages auto-rebuilds on push.

### Option B — Using GitHub web UI (no Terminal)

1. Go to **github.com/jasondporganisation/jasondporganisation.github.io** (or wherever your Pages repo lives)
2. Click **"Add file" → "Upload files"**
3. Create a new folder by typing `mum-tool/` in the filename field, then drag the 4 files (`index.html`, `manifest.json`, `icon-192.png`, `icon-512.png`) into the uploader
4. Scroll down, write commit message `Add DPG Mum Engagement Tool`, click **"Commit changes"**
5. Wait ~1 minute, visit `https://jasondporganisation.github.io/mum-tool/`

---

## 📲 Tell your agents to bookmark it

### iPad / iPhone (Safari)
1. Open `https://jasondporganisation.github.io/mum-tool/` in Safari
2. Tap the **Share** button (square with arrow)
3. Scroll down → tap **"Add to Home Screen"**
4. Name it **"DPG Mum"** → tap **Add**
5. Icon now sits on home screen like a native app — opens full-screen, no Safari chrome

### Android (Chrome)
1. Open the URL in Chrome
2. Tap the ⋮ menu → **"Add to Home screen"** / **"Install app"**

### Desktop (for practice / office use)
- Just bookmark the URL in Chrome or Safari

---

## 🔄 Updating the tool later

When you want to push updates (new scripts, new objections, etc.):

```bash
cd ~/path/to/jasondporganisation.github.io
# Edit mum-tool/index.html with your changes
git add mum-tool/
git commit -m "Update mum tool — [what you changed]"
git push
```

Live URL auto-updates in ~1 minute. Agents don't need to reinstall — the PWA refreshes on next launch.

---

## 🔗 Cross-link from DP Sales Tracker

Since your Sales Tracker is already at `jasondporganisation.github.io`, you can add a button on it like:

```html
<a href="/mum-tool/" class="btn">🌸 Open Mum Tool</a>
```

Same domain, one-click launch for agents.

---

## 🛠️ Troubleshooting

**"404 Page Not Found" after push**
- Wait 2 minutes — GitHub Pages takes a moment to rebuild
- Check repo Settings → Pages → confirm source is set to `main` branch, root folder
- Make sure the folder is exactly `mum-tool` (lowercase, no spaces)

**Icons not showing on iPad home screen**
- Clear Safari cache → re-add to home screen
- Make sure all 4 files uploaded (especially `manifest.json`)

**WhatsApp share button not working**
- Works only on mobile. On desktop it opens WhatsApp Web.

**Print layout looks off**
- Use Chrome's print preview → set margins to "Default" and scale to 100%
- Save as PDF for the cleanest leave-behind

---

## 🔒 Security & privacy notes (for your agents)

- **All data stays in-browser.** No backend, no database, no leaks.
- Closing the tab / reloading **clears everything** — agents should generate the PDF/WhatsApp summary before closing.
- Nothing is saved about the mum on GitHub — it's a stateless tool.

---

## ❓ Questions

Drop feedback via the thumbs-down on this session or ping me next iteration.

🦁 Built for DP Organisation × Great Eastern Life — April 2026
