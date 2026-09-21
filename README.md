# ◈ Yangiboyev Shohjahon — Portfolio (Vercel-ready)

Jiddiy, klassik uslubdagi portfolio: particle-network foni, day/night rejim, UZ/RU/EN, Times New Roman.

**Jonli:** `https://portfolio-3d.vercel.app`

## struktura
```
index.html      — profil + malaka + tajriba + 6 loyiha + sertifikatlar + aloqa
assets/         — photo.jpg, cv.pdf, ustoz-ai.jpg, ustoz-ai.pdf
projects/       — 7 jonli demo:
  fuqarolar-ovoz.html (+ admin)
  avtokredit-kalkulyator.html
  hujjatai-demo.html, datalens-demo.html
  skillproof-demo.html, yolxaritam-demo.html
vercel.json     — cleanUrls + security headers
robots.txt / sitemap.xml / 404.html
```

## lokal tekshiruv
```bash
cd portfolio-3d
python3 -m http.server 8000
```

## Vercel deploy
vercel.com → Add New → Project → Import `wax-yv/portfolio-3d` → Framework **Other** → Deploy.
