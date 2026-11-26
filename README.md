# Thambara Dahanayaka | Portfolio

A static, single-page portfolio. No build step and no dependencies.

## Files
- `index.html`: the whole site (HTML + CSS)
- `vercel.json`: clean URLs and security headers
- Add images or a CV PDF in this folder (for example `cv.pdf`) and link to them from `index.html`

## Deploy to Vercel

**Option A: GitHub (recommended)**
1. Create a GitHub repo and push these files to the root.
2. On vercel.com choose Add New, then Project, and import the repo.
3. Set Framework Preset to **Other**. Leave Build Command and Output Directory empty. Click Deploy.
4. Every push to `main` redeploys automatically.

**Option B: CLI**
```
npm i -g vercel
cd portfolio-site
vercel          # preview deploy
vercel --prod   # production deploy
```

## Custom domain
Project Settings, then Domains, then add your domain and follow the DNS instructions.

## Note on the CSP
`vercel.json` sets a strict Content-Security-Policy (no scripts, inline styles only). If you later add images from other sites, analytics or scripts, update `img-src` / `script-src` there.
