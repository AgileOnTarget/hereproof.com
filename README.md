# hereproof.com + HereProof art

Static public site for **HereProof** (Agile On Target LLC) and the **canonical art library** for the iOS app.

---

## Folder layout

```
HERPH/
├── index.html              # Landing (GitHub Pages)
├── privacy.html            # App Store privacy URL
├── support.html            # App Store support URL
├── CNAME · .nojekyll
├── assets/
│   ├── ASSET_CATALOG.md    # ← start here for paths
│   ├── app/                # Production art (iOS + site)
│   ├── web/                # Favicons
│   └── design/             # UI reference composites (not shipped)
└── _archive/               # Superseded — do not use
```

---

## Site (GitHub Pages)

| Path | Purpose |
| --- | --- |
| `/` | Landing page |
| `/privacy` | Privacy policy (App Store Connect) |
| `/support` | Support page (App Store Connect) |

Deploy:

```sh
git add .
git commit -m "update: <what changed>"
git push
```

GitHub Pages rebuilds within ~30 seconds. `.nojekyll` is present so HTML is served as-is.

---

## Art for iOS engineering

**Catalog:** `assets/ASSET_CATALOG.md`

**Production files:** `assets/app/` only

**Design references:** `assets/design/` — mapped to backlog in `01_PRODUCT/v1/DESIGN_FLOW_BACKLOG.md`

---

## Content source of truth

Privacy policy content mirrors `02_TECHNICAL/APP_STORE/PRIVACY_POLICY.md` v2.0.  
Brand voice: `01_PRODUCT/BRAND_SYSTEM/BRAND_SYSTEM.md` v2.1

If either source changes, update the corresponding HTML section and re-deploy.

---

## DNS

Apex `hereproof.com` → GitHub Pages IPs:

```
A    @    185.199.108.153
A    @    185.199.109.153
A    @    185.199.110.153
A    @    185.199.111.153
CNAME www  agileontarget.github.io
```

---

## License

Content © 2026 Agile On Target LLC. All rights reserved.
