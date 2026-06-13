# HereProof — Asset catalog

Canonical paths for iOS, web, and design reference. **Use only files under `assets/app/` and `assets/web/` in production builds.**

Last organized: 2026-06-13

---

## Production — `assets/app/` (ship these)

| File | Size | Use |
| --- | --- | --- |
| `herph_hero.png` | 1142×1377 | Primary mascot — Home hero, success screen, tier preview, onboarding |
| `herph_hero_white.png` | 1254×1254 | Square mascot variant — dark backgrounds, marketing |
| `hereproof_logo.png` | 360×150 | Wordmark + star — nav header, onboarding, web site |
| `hereproof_icon.png` | 1024×1024 | App Store icon source → `AppIcon.appiconset` |
| `herph_app_button.png` | 1254×1254 | CTA / marketing button graphic (optional UI) |

### iOS copy targets

| Source | Xcode destination |
| --- | --- |
| `herph_hero.png` | `Presence/Assets.xcassets/HerphMascot.imageset/herph_mascot.png` |
| `hereproof_logo.png` | `Presence/Assets.xcassets/HereProofLogo.imageset/` (create) |
| `hereproof_icon.png` | `Presence/Assets.xcassets/AppIcon.appiconset/` |

---

## Web — `assets/web/` (hereproof.com)

| File | Use |
| --- | --- |
| `favicon-32.png` | Browser tab favicon |
| `favicon-192.png` | Android / PWA icon |
| `apple-touch-icon.png` | iOS home-screen bookmark |

Referenced from `index.html`, `privacy.html`, `support.html`.

---

## Design reference — `assets/design/` (do not ship in app binary)

High-fidelity composites for engineering alignment. See `01_PRODUCT/v1/DESIGN_FLOW_BACKLOG.md`.

| File | Screens | Product version |
| --- | --- | --- |
| `gold-screens.png` | 4 — onboarding, home, tiers, success | v1 TestFlight visual |
| `more-screen-designs.png` | 11 — QR/NFC, activity, profile, receipt | v1.1 flows |
| `blockchain-art.png` | 12 — mint, Solana, watch | v2 |

---

## Archived — `_archive/` (do not use)

Superseded April 2026 iterations. Kept for history only.

| Path | Contents |
| --- | --- |
| `_archive/2026-04-early/HereProof/` | Early ChatGPT mascot drafts, old nested site, brand docx, Namecheap PDF |

---

## Removed duplicates (2026-06-13)

| File | Reason |
| --- | --- |
| `Herph Screens.png` | Byte-identical to `gold-screens.png` |
