# Cammack Consulting LLC site

Static website for Cammack Consulting LLC and Joshua D. Cammack's research profile.

## Files

- `index.html` - consulting/business homepage.
- `research/index.html` - research profile and manuscript links.
- `styles.css` - responsive styling.
- `assets/spectral-triad-constellation.png` - local visual asset copied from the Navier-Stokes visualization work.
- `CNAME` - GitHub Pages custom-domain setting for `cammackco.com`.
- `.nojekyll` - disables Jekyll processing on GitHub Pages.
- `robots.txt` and `sitemap.xml` - basic search-indexing helpers.

## Local preview

Open `index.html` directly in a browser, or run:

```powershell
python -m http.server 8080
```

from this folder and visit `http://localhost:8080`.

## Deployment notes

This can be deployed as a static site to GitHub Pages, Netlify, Cloudflare Pages, Vercel, or any ordinary web host.

Recommended public URLs:

```text
https://cammackco.com/
https://cammackco.com/research/
```

If deployed under a different domain, update the `canonical` URLs and JSON-LD
`url` values in `index.html` and `research/index.html`.

Recommended GitHub repository name:

```text
cammackco-site
```

Recommended GitHub Pages settings:

- Source: deploy from branch.
- Branch: `main`.
- Folder: `/root`.
- Custom domain: `cammackco.com`.

## Tone

The research page intentionally avoids prize claims and proof-hype language. It
is meant to be credible to search engines, endorsers, professors, editors,
referees, and potential collaborators.

The root page presents Cammack Consulting LLC as a software consulting business.
The research page keeps the consulting business and independent research roles
distinct, and does not present the manuscripts as institutionally sponsored.
