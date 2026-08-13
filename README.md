# 971 Hospitality — Brand Assets

Organized, repo-ready brand assets for **971 Hospitality** (Dubai; est. 2018) and its
sub-brands. Extracted and normalized from the company profile deck (15 slides), layered
PSDs, and standalone logo/portrait files.

## Structure

```
971-hospitality-assets/
├── README.md
├── logos/
│   ├── 971-hospitality-wordmark.png    # primary wordmark (gold on green)
│   ├── 971-caffe.png                   # 971 Caffe medallion
│   ├── 971-gourmet.png                 # 971 Gourmet medallion
│   ├── table-971.png                   # Table 971 (circular medallion)
│   ├── steamed-and-stuffed.png         # Steamed & Stuffed sub-brand
│   ├── supper-club.png                 # see note ⚠️ below
│   └── clients/                        # corporate client logos (one file each)
├── people/                             # founder + investor portraits
├── photography/
│   ├── food/                           # plated / collage food photography
│   ├── venue-events/                   # (see NOTES.md — none separable in source)
│   └── textures-backgrounds/           # brand textures & cover artwork
├── map/
│   └── global-footprint-map.png
├── pages-reference/                    # flattened PNG render of all 15 deck slides
├── text-content/                       # page-01.txt … page-15.txt
└── _source-do-not-commit/              # raw PSDs + 523 MB master PDF + full extraction (gitignored)
```

## What's here

- **logos/** — 6 first-party brand marks + **9 client logos** (Crocs ×2, Mastercard,
  Michael Kors ×2, Sephora, Zurich, Amazon, Bloomberg). Raster logos are PNG; the two
  vector logos (Mastercard, Michael Kors) are kept as **SVG** since vector is the
  superior source form for a logo.
- **people/** — Tamanna Moolchandani (Founder & CEO), Sanjay Advani, Manisha Advani. JPEG q90.
- **photography/food/** — `971-food-collage.jpg` (15-dish marble collage, clean) and
  `plated-dish-hero.jpg` (dark plated hero; note: a small "Our Mission" headline is baked
  into the source photo).
- **photography/textures-backgrounds/** — `971-green-paper-texture.jpg` (the brand's green
  paper field) and `971-cover-gold-brown.jpg` (deck cover artwork; the wordmark is baked in).
- **map/** — the "Global Footprint" world map screenshot.
- **pages-reference/** — every slide rendered to PNG (long edge 3000 px) for reference.
- **text-content/** — real extracted copy for the 4 text slides (03, 05, 06, 12); the
  other 11 are image-only and carry a stub note.

## Normalization

- Any image over **3000 px** on its long edge was downscaled to 3000 px (aspect preserved).
- Photos: **JPEG quality 90**. Logos / anything needing transparency: **PNG**.
- **No file exceeds 15 MB** (largest committed file ≈ 5.6 MB).

## Excluded (intentionally, per brief)

- `PHOTO-2026-08-12-14-01-43.jpg` — internal feedback screenshot, not a brand asset.
- `Screenshot …5.43.08 PM.png` — a stray "THAILAND" label crop from the map.
- One duplicate wordmark JPEG (identical MD5).

Both excluded files remain on disk in the original working folder; they are not deleted.

## ⚠️ Notes & judgment calls

1. **`logos/supper-club.png`** — the source file `Supper club logo.jpeg` was requested for
   cataloging, but the exact folder spec had no slot for it, and its **content is actually a
   rectangular "Table 971" lockup** (not a distinct "supper club" mark). It is placed in
   `logos/` under its source name; treat as a Table 971 wordmark variant.
2. **Two Crocs logos** exist in the source (`crocs.png` black + `crocs-green.png`). The brief
   listed "Crocs" once; both are kept rather than dropping a brand asset.
3. **venue-events/** is empty of photography — the source has no separable venue/event shots
   (see `photography/venue-events/NOTES.md`).
4. Full PSD layer exports (incl. hidden layers), per-PSD text dumps, flattened composites, the
   layer manifest (`psd-manifest.md`), and all 55 embedded PDF images are preserved in
   `_source-do-not-commit/` — available but **gitignored** to keep the repo lean.
5. **"Humans of 971" campaign images: none found** anywhere in the source.
