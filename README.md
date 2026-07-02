# Modus Economic Consulting LLC — Website

A single-page site built with plain HTML/CSS/JS — no build step, no framework, so it deploys straight to GitHub Pages.

## Files
- `index.html` — all page content
- `styles.css` — design system (colors, type, layout)
- `script.js` — mobile nav, footer year, contact form

## Status
Placeholder content has been replaced with real firm and principal details
(bio, credentials, services, and contact info) based on Kan Chen's CV and
sample expert reports. Double-check the About, Services, and Contact
sections before launch, and update them as the firm's practice evolves.

## Optimization pass (2026-07-02)
- Added SEO metadata: Open Graph/Twitter tags, canonical link, JSON-LD
  `ProfessionalService` structured data, `robots.txt`, `sitemap.xml`.
  **Update the domain** in these (currently `https://modusecon.com/`) if the
  real production domain differs.
- Added `favicon.svg` (brand monogram) referenced from `index.html`.
- Cross-device polish: Safari/Firefox vendor prefixes for backdrop-filter and
  font smoothing, safe-area padding for notched phones, larger (44px) mobile
  menu tap target.
- Added a header "Email us" button (desktop/tablet) and turned the contact
  email into a styled button, both prefilled with a mailto subject line, so
  visitors can reach out in one tap/click.
- Minor copy tweak: removed a duplicate "matter at hand" phrase in the
  Contact section.

## Deploying to your existing GitHub repo
1. Copy `index.html`, `styles.css`, and `script.js` into the root of your repo (replacing the placeholder file).
2. Commit and push:
   ```
   git add index.html styles.css script.js
   git commit -m "Add Modus Economic Consulting site"
   git push
   ```
3. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, choose `main` (or your default branch) and `/ (root)`, then save.
4. GitHub will publish at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Custom domain (optional)
If you own a domain (e.g. `moduseconconsulting.com`):
1. In **Settings → Pages**, enter the domain under "Custom domain" — this creates a `CNAME` file in your repo automatically.
2. At your domain registrar, add a `CNAME` record pointing `www` to `<your-username>.github.io`, and `A` records for the root domain pointing to GitHub's IPs (GitHub's Pages docs list the current set).
3. Wait for DNS to propagate, then enable "Enforce HTTPS" in the same settings panel.
