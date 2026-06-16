# Shrimad Bhagwat Katha Website

Event website for **श्रीमद् भागवत कथा** (22–28 October 2026) at Gopalapur, Bhadohi, UP.

## Local preview

```bash
cd ~/Projects/bhagwat-katha
python3 -m http.server 8080
```

Open http://localhost:8080

## Deploy (low-cost / free — fast in Mumbai)

### Option 1: Cloudflare Pages (Recommended — FREE, Mumbai edge node)

1. Push this repo to GitHub
2. Go to [dash.cloudflare.com](https://dash.cloudflare.com) → Pages → Create project
3. Connect GitHub repo → Build settings: **None** (static site, no build command)
4. Publish directory: `/` (root)
5. Custom domain optional (~₹700/year for `.in` domain elsewhere)

### Option 2: Netlify (FREE tier)

1. Push to GitHub
2. [app.netlify.com](https://app.netlify.com) → Add new site → Import from Git
3. Build command: *(leave empty)* | Publish directory: `.`
4. Or drag-and-drop the folder at netlify.com/drop

### Option 3: GitHub Pages (FREE)

1. Push to GitHub
2. Settings → Pages → Source: Deploy from branch `main` → folder `/ (root)`

### Option 4: Indian shared hosting (paid, ~₹69–129/month)

- **Hostinger India** — Mumbai data center, `.in` domain + hosting bundles
- **BigRock** — Indian provider, cPanel upload

Upload all files via FTP/cPanel File Manager.

## Project structure

```
bhagwat-katha/
├── index.html
├── css/styles.css
├── js/main.js
├── assets/images/
│   ├── speaker-hero.jpg
│   ├── poster-main.jpg
│   ├── poster-alt.jpg
│   └── gallery/
└── netlify.toml
```
