# NicheMoat Reports

Public NicheMoat extension reports, served as static HTML.

**Live:** https://share.nichemoat.com/

## How it works

```
local edit → git push (main) → Cloudflare Pages auto-deploy → share.nichemoat.com
```

- Hosting: Cloudflare Pages (static, no build step).
- Reports live at repo **root**: a file `report.html` serves at `https://share.nichemoat.com/report.html`.
- `index.html` is the landing page at `https://share.nichemoat.com/`.

## Add a report

1. Copy the `.html` file into this folder (root).
2. Commit and push to `main`:
   ```bash
   git add .
   git commit -m "Add <report-name>"
   git push
   ```
3. Live in ~30s at `https://share.nichemoat.com/<file>.html`.

## Notes

- Only public-safe reports belong here — this repo is **public**.
- Plain HTML only; no build command configured in Pages.
