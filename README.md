# the-britannia.com

Static one-page site for The Britannia, 62 Eastborough, Scarborough.
No build step: `index.html` plus the `images/` folder. Edit the HTML directly.

## Publish with GitHub Pages

1. Create a new **public** repo (suggested name: `the-britannia`).
2. Upload everything in this folder — `index.html`, `images/`, `CNAME`, `.nojekyll` — to the repo root.
3. Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`. Save.
4. Settings → Pages → Custom domain: `www.the-britannia.com`. Tick *Enforce HTTPS* once it appears (can take an hour).

## DNS (at your domain registrar)

| Type  | Name | Value |
| ----- | ---- | ----- |
| CNAME | www  | mikemerron.github.io |
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |

The four A records make the bare domain (the-britannia.com) redirect to www.
Remove the Squarespace records for @ and www first, or they will conflict.

## Meta verification

- Domain verification: Meta Business Manager → Brand safety → Domains → add
  `the-britannia.com`, choose the **DNS TXT** method, add the TXT record at your
  registrar alongside the records above.
- Business verification: the entity is **Pax Britannia** (a partnership) trading as
  The Britannia. The footer of this site carries that wording and the address —
  type them into Meta exactly as they appear there.
