# Cammack Consulting LLC site

Static website for Cammack Consulting LLC and Joshua D. Cammack's research profile.

## Files

- `index.html` - consulting/business homepage.
- `research/index.html` - research profile and manuscript links.
- `resume/index.html` - web-native professional resume.
- `404.html` - custom not-found page for GitHub Pages.
- `styles.css` - responsive styling.
- `assets/` - production image assets used by the site.
- `CNAME` - GitHub Pages custom-domain setting for `cammackco.com`.
- `.nojekyll` - disables Jekyll processing on GitHub Pages.
- `robots.txt` and `sitemap.xml` - basic search-indexing helpers.

Ignored local scratch work such as design drafts should stay under
`design_candidates/` and must not be committed.

## Local preview

Run a local static server:

```powershell
python -m http.server 8080
```

from this folder and visit `http://localhost:8080`.

Directly opening `index.html` also works for basic review, but the local server
is better because root-relative links such as `/assets/favicon.png` resolve the
same way they do on GitHub Pages.

## Deployment notes

This can be deployed as a static site to GitHub Pages, Netlify, Cloudflare Pages, Vercel, or any ordinary web host.

Recommended public URLs:

```text
https://cammackco.com/
https://cammackco.com/research/
https://cammackco.com/resume/
```

If deployed under a different domain, update the `canonical` URLs and JSON-LD
`url` values in `index.html`, `research/index.html`, and `resume/index.html`.

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

## Quality checklist

Before pushing site changes:

- Check desktop and mobile layouts for `/`, `/research/`, `/resume/`, and
  `/404.html`.
- Confirm there is no horizontal overflow on mobile.
- Keep generated design candidates and scratch artifacts out of the repository.
- Keep page titles, descriptions, canonical URLs, Open Graph metadata, and
  sitemap entries aligned with public URLs.
- Keep client/NDA work anonymized unless explicit permission exists.
