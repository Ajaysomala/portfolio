# Somala Ajay — Portfolio Website

Personal portfolio website hosted on **Cloudflare Pages** via GitHub.

## Tech Stack
- Pure HTML / CSS / Vanilla JS (no build step required)
- Hosted on Cloudflare Pages (free tier)
- Auto-deploys on every push to `main`

## File Structure
```
portfolio/
├── index.html   ← Main portfolio page (all-in-one)
└── README.md
```

## Deploy to Cloudflare Pages

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/Ajaysomala/ajay-portfolio.git
git push -u origin main
```

### Step 2 — Connect to Cloudflare Pages
1. Go to https://pages.cloudflare.com
2. Click "Create a project" → "Connect to Git"
3. Select your GitHub account → pick the repo
4. Build settings:
   - Production branch: `main`
   - Build command: *(leave empty)*
   - Build output directory: `/`
5. Click "Save and Deploy" — done!

Cloudflare gives you a free URL like `ajay-portfolio.pages.dev`.
Every push to `main` auto-deploys the site within seconds.

### Optional: Custom Domain
Cloudflare Pages → your project → Custom Domains → add your domain.
