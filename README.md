# Gagnatorg sveitarfélaga

Static-vefur með mælaborðum og greiningum á opnum gögnum frá Reykjavíkurborg, Hagstofu Íslands, Sambandi íslenskra sveitarfélaga og Gagnagátt Reykjavíkur.

**Live:** https://gagnatorg.skattgreidendur.is

## Mælaborð og greiningar

| Slóð | Lýsing |
|---|---|
| `/` | Forsíða gagnatorgs (`index.html` = `gagnatorg.html`) |
| `/rvk-utforska.html` | Útforska reikninga · Reykjavíkurborg 2019–2025 |
| `/svf-heilsuvog.html` | Fjárhagsleg heilsuvog 40 sveitarfélaga |
| `/skatttekjur-per-ibua.html` | Skatttekjur á mann (útsvar, fasteignaskattur, jöfnunarsjóður) |
| `/rvk-2025-forskot.html` | 2025 ársreikningar — forsýning |
| `/rvk-er-bestrekna.html` | Reykjavík tap 19,4 ma.kr. 2018-2024 |
| `/rvk-tekjuhlid.html` | Tekjuhliðin · Reykjavíkurborg |

## Tækni

- **Static HTML** með innbyggðu JSON (engin live DB-kall)
- **Hostað á Vercel** í gegnum GitHub
- **Sjálfvirk uppfærsla:** `git push` → Vercel byggir og setur upp

## Þróun

Allt þróunarefni er í aðal-repo (private). Hér eru bara public-facing skrár.

```bash
# Ný útgáfa
git pull
# Edit HTML / JSON
git add .
git commit -m "Lýsing"
git push
# Vercel uppfærir sjálfkrafa á 1-2 mínútum
```

## Léttvægar leiðbeiningar

- Hver HTML-síða er sjálfstæð — engin sameiginleg navigation, hver síða hýsir öll sín CSS+JS+gögn
- Öll JSON-gögn eru í `public/data/`
- Samfélagsmiðla-myndir í `public/img/`

© Samtök skattgreiðenda · skattgreidendur.is
