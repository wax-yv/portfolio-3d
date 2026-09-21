# ◈ Shohjahon Yangiboyev — 3D Portfolio (Vercel-ready)

Realistik 3D, minimalistik, diplomatik portfolio. Zero-build static — Vercel'ga to'g'ridan-to'g'ri deploy.

**Jonli demo:** `https://portfolio-3d.vercel.app` (repo nomiga qarab o'zgaradi)

## stack
- Static `index.html` + `data.json` (UZ / RU / EN)
- Three.js 0.160 (CDN, importmap): TorusKnot + wireframe icosahedron + 26 oltin shard + 1300 yulduz + grid + shadow
- OrbitControls: drag-to-orbit, scroll-zoom, mouse parallax
- `prefers-reduced-motion` qo'llab-quvvatlanadi

## struktura
```
index.html      — 3D sahna + UI + i18n
data.json       — barcha kontent (UZ/RU/EN)
assets/cv.pdf   — CV (Shohjavon_cv.pdf nusxasi)
projects/       — 3 ta jonli demo:
  fuqarolar-ovoz.html
  fuqarolar-ovoz-admin.html
  avtokredit-kalkulyator.html
vercel.json     — cleanUrls + security headers + cache
robots.txt / sitemap.xml / 404.html
```

## kontent manbai (`CV+PORTFOLIO/`)
- `Shohjavon_cv.pdf` → ism, aloqa, ko'nikmalar, tajriba, ta'lim, loyihalar, sertifikatlar
- `Coursera Sertification…` + `shohjahon 1/2.pdf` → Google GenAI, Duke Math, Tableau
- `Saytlar yasash.pdf` → Ustoz AI No-Code (oltin)
- `81-85.pdf` + `Янгибоев Шоҳжаҳон.pdf` → MHXS/IFRS ilmiy maqola
- `fuqarolar-ovoz*.html`, `avtokredit*.html` → projects/

## lokal tekshiruv
```bash
cd portfolio-3d
python3 -m http.server 8000
# http://localhost:8000
```

## Vercel deploy (o'zingiz qilasiz — 2 daqiqa)
1. https://vercel.com → **Add New → Project**
2. **Import** `wax-yv/portfolio-3d` (GitHub)
3. Framework Preset: **Other** (build yo'q)
4. **Deploy** → tayyor. `vercel.json` avtomatik ishlaydi.

Yoki Vercel CLI:
```bash
npm i -g vercel
cd portfolio-3d
vercel --prod
```

## GitHub push
```bash
cd ~/portfolio-3d
git add -A
git commit -m "Mukammal 3D portfolio: hero, i18n, SEO, CV, projects"
git push origin main
```
