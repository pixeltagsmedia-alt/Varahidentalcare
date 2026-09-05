# Deploy Varahi Dental Care to Vercel

The whole website is the `site/` folder: `index.html` + `img/` (10 photos) + `robots.txt`. No build step, no dependencies.

## Easiest way (drag & drop, ~2 minutes)
1. Download the `site` folder from this project (zip).
2. Unzip it on your computer.
3. Go to vercel.com/new → "Deploy" → drag the **contents of the unzipped folder** (index.html, img/, robots.txt) into the drop area.
   - Important: drop the *contents*, not the folder itself, so `index.html` sits at the root.
4. Framework preset: **Other**. Build command: leave empty. Output directory: leave empty.
5. Deploy. You get a live URL like `varahi-dental-care.vercel.app`.

## Via GitHub (better for future edits)
1. Create a repo, put `index.html`, `img/`, `robots.txt` at the repo root.
2. vercel.com/new → Import that repo → Framework preset **Other** → Deploy.
3. Any push to `main` redeploys automatically.

## Custom domain
Vercel project → Settings → Domains → add e.g. `varahidentalcare.com`.
Then at your registrar, set the records Vercel shows (usually `A 76.76.21.21` for the root and `CNAME cname.vercel-dns.com` for `www`). HTTPS is issued automatically.

## Before going live
- Replace the text logo in the header with your gold-tooth PNG (drop `logo.png` into `img/`, swap the logo block in `index.html`).
- Update the `canonical` and `og:image` URLs in `<head>` to your real domain.
- Confirm the Mon–Sat 10:00–8:30 PM hours (used in the contact card and the schema block).
