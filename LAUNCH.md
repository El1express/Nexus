# Nexus — Launch Guide

## What's in this package
```
nexus/
├── index.html          ← The full app
├── manifest.json       ← PWA config (name, icons, colors)
├── sw.js               ← Service worker (offline + caching)
├── icons/              ← All app icons (all sizes)
│   ├── icon-192x192.png
│   ├── icon-512x512.png
│   ├── apple-touch-icon.png
│   └── ... (all sizes)
└── LAUNCH.md           ← This file
```

---

## 🚀 Option 1 — Netlify Drop (Fastest — 60 seconds)

1. Go to **https://app.netlify.com/drop**
2. Drag the entire `nexus/` folder onto the page
3. Netlify gives you a free URL like `https://nexus-abc123.netlify.app`
4. Done — your app is live!

**To get a custom domain** (like `nexus.yourdomain.com`):
- In Netlify → Site Settings → Domain Management → Add custom domain
- Point your DNS CNAME to Netlify

---

## 🚀 Option 2 — Vercel (Also free, very fast)

1. Install Vercel CLI: `npm i -g vercel`
2. In this folder, run: `vercel`
3. Follow prompts — done in 30 seconds
4. Gets you `https://nexus.vercel.app` or similar

---

## 🚀 Option 3 — GitHub Pages (Free, permanent)

1. Create a new repo on **github.com**
2. Upload all files in this folder to the repo
3. Go to Settings → Pages → Source: main branch
4. Your app is at `https://yourusername.github.io/nexus`

---

## 📱 Installing on iPhone (after hosting)

1. Open your Nexus URL in **Safari** (must be Safari)
2. Tap the **Share button** (box with arrow)
3. Tap **"Add to Home Screen"**
4. Tap **"Add"**
5. Nexus appears on your home screen like a real app ✓

---

## 📱 Installing on Android (after hosting)

1. Open your Nexus URL in **Chrome**
2. Tap the **three dots menu**
3. Tap **"Add to Home screen"** or **"Install app"**
4. Tap **"Install"**
5. Nexus appears on your home screen ✓

---

## 💻 Installing on Desktop (Chrome/Edge)

1. Open your Nexus URL
2. Look for the **install icon** in the address bar (right side)
3. Click it → Install
4. Nexus opens as a standalone desktop app ✓

---

## 🔑 API Key (for self-hosted use outside claude.ai)

If you're hosting this yourself and want it to work independently:

1. Get an API key from **https://console.anthropic.com**
2. Open `index.html` in a text editor
3. Find `callAPI` function
4. Add this header: `'x-api-key': 'YOUR_KEY_HERE'`

Or use a backend proxy to keep your key secure.

---

## ✅ Checklist before launch

- [ ] Hosted on a URL (Netlify/Vercel/GitHub Pages)
- [ ] Opened in browser — app loads correctly
- [ ] Tested a conversation — AI responds
- [ ] Tested file upload
- [ ] Installed on phone from Safari/Chrome
- [ ] Nexus icon appears on home screen

---

*Built with Nexus Business Intelligence Suite*
