# hereproof.com

Static public site for **HereProof**, the iPhone app by Agile On Target LLC.

Three pages, zero build step, no JavaScript, no third-party assets. Hosted on GitHub Pages at `hereproof.com`.

| Path | Purpose |
| --- | --- |
| `/` | Landing page |
| `/privacy` | Privacy policy (App Store Connect uses this URL) |
| `/support` | Support page (App Store Connect uses this URL) |

## Source of truth

Content mirrors the canonical docs in the private HereProof engineering repo:
- Privacy policy source: `PRIVACY_POLICY.md` v2.0
- Brand voice: `BRAND_SYSTEM.md` v2.1

If either source changes, update the corresponding `<section>` of the HTML here and re-deploy.

## Deploy

```sh
git add .
git commit -m "update: <what changed>"
git push
```

GitHub Pages rebuilds within ~30 seconds. `.nojekyll` is present so HTML is served as-is.

## DNS

Apex `hereproof.com` points at GitHub Pages IPs:
```
A    @    185.199.108.153
A    @    185.199.109.153
A    @    185.199.110.153
A    @    185.199.111.153
CNAME www  agileontarget.github.io
```

## License

Content © 2026 Agile On Target LLC. All rights reserved.
