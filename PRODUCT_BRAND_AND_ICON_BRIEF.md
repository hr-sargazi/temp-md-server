# Lira Card Platform — Brand & Icon Deliverables Brief

**Document for:** Product / Brand / Design team  
**Product:** `lira-card-platform-ui` (Lira Card Platform web app)  
**Repository:** `card-platform/lira-card-platform-ui`  
**Date:** June 2026  
**Status:** Complete deliverables list — all items below are required.

---

## 1. Product summary

| Field | Value |
|-------|--------|
| **Full name (EN)** | Lira Card Platform |
| **Full name (FA)** | پلتفرم کارت لیرا |
| **Category** | B2B fintech operations — card issuing, KYC, tenants, fulfillments |
| **Users** | Platform admins + tenant operators (not end-cardholders) |
| **Languages** | English (LTR), Farsi / Persian (RTL) |
| **Deployment** | Web app + **installable PWA** (Add to Home Screen / Install app) |
| **Desktop + mobile** | Both — responsive admin/tenant console |

The app will be installable as a Progressive Web App. Icons, splash screens, and manifest metadata must support iOS, Android, and desktop browsers (Chrome, Edge, Safari).

---

## 2. Brand identity direction (current UI)

### 2.1 Visual language

- **Motif:** Card / fintech — today the in-app logo uses a **credit card** symbol on a gradient tile.
- **Shape language:** Rounded corners (approximately 14–24px on tiles; full pills for chips).
- **Depth:** Soft shadows, subtle glass/blur panels, light gradients — **not** flat black-and-white.
- **Primary interaction gradient:** Teal → indigo at **135°** (top-left to bottom-right).

### 2.2 Typography (for any text in marketing assets only — not inside small icons)

| Locale | Font family |
|--------|-------------|
| English | Inter |
| Farsi | Vazirmatn |
| Monospace (UI data) | JetBrains Mono |

**Rule:** App icons at 72–192px must **not** include readable text or long wordmarks. The OS shows the app name under the icon.

---

## 3. Color palette (exact values)

Design all icons and splashes using these tokens. The app has **light** and **dark** themes; artwork must remain legible on both.

### 3.1 Brand colors (primary — use in icons)

| Token | Light theme | Dark theme | Role |
|-------|-------------|------------|------|
| **Accent (teal)** | `#0D9488` | `#2DD4BF` | Primary brand |
| **Accent hover** | `#0F766E` | `#5EEAD4` | Hover / emphasis |
| **Accent secondary (indigo)** | `#6366F1` | `#818CF8` | Gradient end, secondary highlight |
| **Brand gradient** | `linear-gradient(135deg, #0D9488 0%, #6366F1 100%)` | `linear-gradient(135deg, #2DD4BF 0%, #818CF8 100%)` | Logo tiles, primary buttons |
| **On-accent** (glyph on gradient) | `#FFFFFF` | `#0F172A` | Icon stroke/fill on gradient background |

### 3.2 Surfaces (test icon contrast on these)

| Token | Light | Dark |
|-------|-------|------|
| Page background | `#F0F7FC` | `#0A101C` |
| Card / panel | `#FFFFFF` | `#111827` |
| Elevated surface | `#E2EEF8` | `#1E293B` |
| Muted / border | `#CBDDEB` | `#334155` |

### 3.3 Text (reference for splash / marketing only)

| Token | Light | Dark |
|-------|-------|------|
| Primary text | `#0C1C2D` | `#F1F5F9` |
| Secondary text | `#334E68` | `#BACBDC` |
| Muted text | `#64829E` | `#7890A8` |

### 3.4 Semantic colors (reference — badges, not main app icon)

| Meaning | Light | Dark |
|---------|-------|------|
| Success | `#059669` | `#34D399` |
| Warning | `#D97706` | `#FBBF24` |
| Danger | `#DC2626` | `#F87171` |

### 3.5 PWA chrome colors (provide as manifest values)

| Field | Recommended value | Notes |
|-------|-------------------|--------|
| `theme_color` | `#0D9488` | Android status bar, browser UI |
| `background_color` | `#F0F7FC` | Splash while app loads (light) |

Also provide a **dark splash background** color for dark-mode install flows: `#0A101C`.

---

## 4. Icon design rules

1. **One unified mark** that reads clearly on light phone wallpapers (`#F0F7FC`, white) and dark wallpapers (`#111827`, black).
2. **Maskable / adaptive icon:** Critical logo content must sit inside the **center 80% circle** (Android crops corners).
3. **No small text** inside icon PNGs (no “Lira”, no Persian text at 72–192px).
4. **Export sharp PNGs** — no blurry downscaling from a single small source; export each size from vector.
5. **Deliver SVG source** for all marks (master artwork).
6. **Favicon:** Provide **light-theme** and **dark-theme** variants (browser tab).
7. **Home screen icon does not change** when the user toggles in-app theme — design one strong mark that works everywhere.

---

## 5. Required deliverables — file list

Deliver a folder (zip or shared drive) with the structure below. **All files are required.**

### 5.1 Master source files

| File | Format | Spec |
|------|--------|------|
| `icon-master.svg` | SVG | Full vector logo; editable layers |
| `icon-master.png` | PNG | **1024×1024** px, transparent or solid bg per design |
| `icon-maskable-master.svg` | SVG | Maskable variant with safe-zone guides visible (for review) |
| `brand-guidelines.pdf` | PDF | 1–4 pages: colors, gradient, clear space, do/don’t |

### 5.2 PWA / Web App Manifest icons (`purpose: any`)

Export as PNG, sRGB, no interlacing.

| Filename | Size (px) |
|----------|-----------|
| `icon-72.png` | 72×72 |
| `icon-96.png` | 96×96 |
| `icon-128.png` | 128×128 |
| `icon-144.png` | 144×144 |
| `icon-152.png` | 152×152 |
| `icon-192.png` | 192×192 |
| `icon-384.png` | 384×384 |
| `icon-512.png` | 512×512 |

### 5.3 Maskable PWA icon (`purpose: maskable`)

| Filename | Size (px) | Notes |
|----------|-----------|--------|
| `icon-maskable-512.png` | 512×512 | Logo within center 80% safe circle |

### 5.4 Apple / iOS

| Filename | Size (px) | Notes |
|----------|-----------|--------|
| `apple-touch-icon.png` | **180×180** | iOS Add to Home Screen |
| `apple-touch-icon-152.png` | 152×152 | Legacy iPad |
| `apple-touch-icon-120.png` | 120×120 | Legacy iPhone |

### 5.5 Favicons (browser tab)

| Filename | Size (px) | Theme |
|----------|-----------|--------|
| `favicon-16.png` | 16×16 | Light UI |
| `favicon-32.png` | 32×32 | Light UI |
| `favicon-48.png` | 48×48 | Light UI |
| `favicon-dark-16.png` | 16×16 | Dark UI |
| `favicon-dark-32.png` | 32×32 | Dark UI |
| `favicon-dark-48.png` | 48×48 | Dark UI |
| `favicon.ico` | Multi-size ICO | Contains 16, 32, 48 (light set) |
| `favicon.svg` | SVG | Optional single SVG with `prefers-color-scheme` if supported |

### 5.6 Safari pinned tab

| Filename | Format | Notes |
|----------|--------|--------|
| `safari-pinned-tab.svg` | SVG | **Single color** silhouette; transparent bg |

### 5.7 Splash / install screens

| Filename | Size (px) | Notes |
|----------|-----------|--------|
| `splash-light-1280x720.png` | 1280×720 | Landscape splash, light bg |
| `splash-light-750x1334.png` | 750×1334 | Portrait iPhone reference, light |
| `splash-dark-1280x720.png` | 1280×720 | Landscape splash, dark bg |
| `splash-dark-750x1334.png` | 750×1334 | Portrait, dark |
| `splash.svg` | SVG | Vector splash (logo + bg) for engineering export |

Splash should use: logo mark + `#F0F7FC` (light) or `#0A101C` (dark). No heavy text; optional subtle gradient consistent with brand.

### 5.8 Open Graph / social preview (link sharing)

| Filename | Size (px) |
|----------|-----------|
| `og-image.png` | **1200×630** |

### 5.9 Design system reference (in-app logo tile)

| Filename | Size (px) | Notes |
|----------|-----------|--------|
| `logo-tile-44.png` | 44×44 | Sidebar / auth brand icon size |
| `logo-tile-88.png` | 88×88 | @2x |
| `logo-tile.svg` | SVG | Matches gradient tile + card glyph in UI |

---

## 6. Manifest & metadata copy (provide in deliverable)

Fill this table. Engineering will wire into `manifest.json` and Next.js metadata.

| Key | English | Farsi | Max length guidance |
|-----|---------|-------|---------------------|
| `name` | Lira Card Platform | پلتفرم کارت لیرا | Full store name |
| `short_name` | Lira Cards | لیرا کارت | **≤ 12 characters** for home screen |
| `description` | *(you write)* | *(you write)* | 1–2 sentences, install prompt |
| `theme_color` | `#0D9488` | — | Hex |
| `background_color` | `#F0F7FC` | — | Hex (light splash) |
| `background_color_dark` | `#0A101C` | — | Hex (dark splash) |
| `categories` | `finance`, `business` | — | W3C manifest categories |

**Suggested description (EN) — edit as needed:**  
*“Operate card programs, KYC, and fulfillment for your organization.”*

**Suggested description (FA) — edit as needed:**  
*«مدیریت برنامه‌های کارت، احراز هویت و صدور برای سازمان شما.»*

---

## 7. Maskable icon safe zone

For `icon-maskable-512.png`:

- Canvas: **512×512** px  
- **Safe zone:** circle **410×410** px centered (80% diameter)  
- **Critical content** (logo mark) must fit entirely inside safe zone  
- Background may extend to full bleed; corners may be cropped on Android  

Include in `brand-guidelines.pdf` a diagram showing safe zone on a 512px grid.

---

## 8. Quality checklist (design sign-off)

Before handoff, confirm:

- [ ] Icon readable at **16×16** (favicon) and **512×512** (PWA)
- [ ] Tested on **white**, **#F0F7FC**, **#111827**, and **black** backgrounds
- [ ] Maskable 512px passes Android adaptive icon preview (no clipped logo)
- [ ] Light and dark favicons distinct and recognizable at 16px
- [ ] Gradient direction **135°** teal → indigo matches brand table
- [ ] No Persian/English text inside icon PNGs ≤ 192px
- [ ] All PNGs exported sRGB, no compression artifacts
- [ ] SVG sources use clean paths (suitable for web)
- [ ] `apple-touch-icon.png` has **no transparency** (iOS fills transparent with black)
- [ ] OG image 1200×630 legible when cropped in messaging apps

---

## 9. Delivery format

**Folder structure:**

```
lira-card-platform-brand/
├── source/
│   ├── icon-master.svg
│   ├── icon-master.png
│   ├── icon-maskable-master.svg
│   ├── splash.svg
│   ├── logo-tile.svg
│   └── safari-pinned-tab.svg
├── icons/
│   ├── icon-72.png … icon-512.png
│   ├── icon-maskable-512.png
│   ├── apple-touch-icon.png
│   ├── apple-touch-icon-152.png
│   ├── apple-touch-icon-120.png
│   └── logo-tile-44.png, logo-tile-88.png
├── favicons/
│   ├── favicon-16.png … favicon-48.png
│   ├── favicon-dark-16.png … favicon-dark-48.png
│   ├── favicon.ico
│   └── favicon.svg (if provided)
├── splash/
│   ├── splash-light-1280x720.png
│   ├── splash-light-750x1334.png
│   ├── splash-dark-1280x720.png
│   └── splash-dark-750x1334.png
├── social/
│   └── og-image.png
├── docs/
│   ├── brand-guidelines.pdf
│   └── manifest-copy.md (section 6 filled in)
└── figma/ (or Adobe)
    └── *.fig (optional but encouraged — link to Figma also acceptable)
```

**Also provide:** Link to Figma/Adobe Cloud file with export settings documented.

---

## 10. Relationship to other Lira products

This app is the **card platform admin/tenant console** (B2B). It is related to but distinct from:

- **Lira Troy Card app** (`lira-troy-card-app`) — consumer/virtual card panel  
- Family resemblance is welcome; identical consumer wallet icon is **not** required  

If brand team maintains a shared **Lira fintech icon system**, align teal/indigo gradient with that system.

---

## 11. What engineering will do after handoff

*(For product team awareness — no action required.)*

1. Place assets under `public/icons/`, `public/favicons/`, etc.
2. Add Web App Manifest and Next.js metadata
3. Wire light/dark favicon swap when user changes theme in-app
4. Enable PWA install prompt (desktop + mobile)
5. Set `theme_color` / splash for installed app

---

## 12. Contact & questions

| Topic | Owner |
|-------|--------|
| Product / naming (EN + FA) | Product team |
| Technical constraints | Engineering (`lira-card-platform-ui`) |
| Brand approval | Brand / design lead |

**Open questions for product to resolve before final export:**

1. Final `short_name` for home screen (EN + FA) — 12 char limit  
2. Final one-line `description` (EN + FA) for install dialog  
3. Confirm app icon motif: **card glyph on gradient** vs abstract mark  
4. Confirm whether splash shows logo only or logo + wordmark  

---

*End of brief — please deliver all items in sections 5–6 and section 9 folder structure.*
