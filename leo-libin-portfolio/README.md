# Leo Libin — Portfolio

A static one-page site. No build step, no dependencies — just three files:

```
index.html            the site
leo-libin.png          headshot, used in the hero panel
Leo-Libin-Resume.pdf   linked from the nav and the "Download résumé" button
```

## Deploy to Vercel

**Option A — dashboard (no install needed)**
1. Go to https://vercel.com/new
2. Drag this whole folder onto the page (or choose "Upload" if prompted)
3. Leave all settings as default — Vercel auto-detects it as a static site
4. Click **Deploy**

**Option B — CLI**
```bash
npm install -g vercel
cd this-folder
vercel --prod
```

Either way, you'll get a live `*.vercel.app` URL in under a minute. You can attach a custom domain afterward from the Vercel project's **Settings → Domains** tab.

## Notes

- Keep all three files in the same folder — the HTML references the image and PDF by relative path.
- The dark/light toggle defaults to the visitor's system preference and doesn't persist across page reloads. If you want it to remember the last choice, that's a small addition (`localStorage`) — just ask.
- To update your résumé later, replace `Leo-Libin-Resume.pdf` with a new file of the exact same name — no code changes needed.
