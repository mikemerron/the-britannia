# The Britannia — the-britannia.com

Static one-page site for The Britannia, a bar at 62 Eastborough, Scarborough YO11 1NJ.
No build step, no framework: `index.html` (all CSS/JS inline) plus `images/`. Edit the HTML directly.

## Hosting & deploy

- **Live at https://www.the-britannia.com** via GitHub Pages, repo `mikemerron/the-britannia`, deploy-from-branch: `main`, `/ (root)`. HTTPS enforced.
- Deploying = commit and push to `main`. Live within ~1 minute. Verify with `curl -s https://www.the-britannia.com | grep <something-you-changed>`.
- The `CNAME` file drives the custom domain — don't delete or edit it. GitHub itself sometimes commits `Delete CNAME`/`Create CNAME` when Pages settings change.
- **Never force-push.** If a push is rejected, `git pull --rebase` first — GitHub (or Claude Design saving) may have added commits.
- `.nojekyll` must stay in the repo root.

## DNS & email — handle with care

- DNS is **not** at GoDaddy. Nameservers are Google Cloud DNS, managed at Squarespace Domains (account.squarespace.com/domains).
- Records: `CNAME www → mikemerron.github.io`; four `A @ → 185.199.108–111.153`.
- **Email is Google Workspace** — the MX and Google TXT records on `@` must never be touched.

## Content facts

- Open Wednesday–Sunday from 2pm. Dogs welcome. Instagram: @62.thebritannia.
- Legal entity: **Pax Britannia** (a partnership) trading as The Britannia — footer wording must stay exactly as-is for Meta business verification.
- The OSM map embed marker is the pub itself: 54.28421, -0.39349. If OSM coordinates are needed, geocode "62 Eastborough, Scarborough".

## Design

- The design came from Claude Design; visual changes may arrive as pushes to this repo. Content/data fixes (hours, links, coordinates, meta tags) are edited directly in `index.html`.
- Aesthetic: "18th century bones, 21st century soul" — Playfair Display + Lora, sage/off-white palette, sepia-matted `.plate` photo treatment. Keep changes in that register.

## Outstanding

- Meta domain verification: add the DNS TXT record from Meta Business Manager at Squarespace Domains (see README).
