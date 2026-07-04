# Conquet — concept homepage

Static one-page site for Mondhygiënepraktijk Conquet (Leiden). Deploys free on GitHub Pages.

## Before you deploy — 2 quick edits to `index.html`

1. Replace the two placeholders in the top concept bar: `[uw bedrijfsnaam]` and `[telefoon]`.
2. (Optional) Update the email `info@mondhygiene-conquet.nl` in the contact section if you have their real one.

The reviews section and opening hours are honest placeholders — leave them, or fill in real values once you have them from the business's Google profile.

## Deploy to GitHub Pages (~2 minutes)

Run these from inside this folder. Replace `YOURNAME` with your GitHub username.

```bash
# 1. create the repo on github.com first (empty, no README), named e.g. conquet
# 2. then, in this folder:
git init
git add .
git commit -m "Conquet concept homepage"
git branch -M main
git remote add origin https://github.com/YOURNAME/conquet.git
git push -u origin main
```

Then on github.com:

1. Go to the repo → **Settings** → **Pages**.
2. Under "Build and deployment", set **Source: Deploy from a branch**.
3. Branch: **main**, folder: **/ (root)** → **Save**.
4. Wait ~1 minute. Your site is live at:

   `https://YOURNAME.github.io/conquet/`

That's the URL you drop into the outreach email.

## Nicer URL (recommended for real outreach)

`YOURNAME.github.io/conquet` reads as a demo. To use your own domain (e.g. `demos.uwbedrijf.nl/conquet`):

1. Add a `CNAME` file to this repo containing just your domain.
2. At your domain registrar, add a DNS record pointing to GitHub Pages.
3. Set the custom domain under Settings → Pages.

## Scaling past one business

GitHub Pages is great for proving this with a handful of leads. For hundreds of
auto-generated pages, script the deploys instead — one repo with a subfolder per
business, or a host built for programmatic deploys (Netlify / Cloudflare Pages /
Vercel). Ask and I can set that pipeline up.
