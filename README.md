# THE PAL EMPIRE — HERITAGE CHRONICLE

A fully static, responsive multi-page historical archive built for **GitHub Pages** with a custom domain. No build step, database, sign-in, contact form, email address, client-side analytics or cookie banner.

## Publishing to GitHub Pages

1. Create a **public GitHub repository** (or use an existing public repository).
2. Upload **the contents of this ZIP** to the repository root. Do **not** upload the outer folder as a nested directory.
3. Go to **Settings → Pages → Build and deployment → Deploy from a branch**; select `main` and `/ (root)`.
4. In **Settings → Pages → Custom domain**, enter `hhroyal.in` and save. The `CNAME` file is already included.
5. Configure DNS at your domain registrar with GitHub Pages' current official apex A/AAAA records (see GitHub Docs). Add `www` CNAME only if you want `www` to work; point it to your GitHub username's Pages hostname. Avoid conflicting DNS records. GitHub has controls for redirecting between www and apex.
6. Once DNS resolves and GitHub provisions a certificate, select **Enforce HTTPS**. Confirm the site loads over HTTPS and that `https://hhroyal.in/sitemap.xml` and `/robots.txt` are accessible.
7. Register the domain in **Google Search Console** and **Bing Webmaster Tools**, verify ownership using their provided DNS TXT record, submit `https://hhroyal.in/sitemap.xml`, and inspect your most important URLs. Indexing cannot be guaranteed or made immediate by metadata.
8. Test social previews with Meta Sharing Debugger, LinkedIn Post Inspector and X Card Validator or a share draft. These all require a publicly accessible HTTPS URL (they do not work from a `file://` local preview).

## Editing

- There is one `index.html` for each clean URL directory (`/sovereigns/gopal-i/index.html`, etc.). There are no runtime server requirements.
- Global styles: `assets/site.css`. Interactions: `assets/site.js`. Local pre-generated search index: `assets/search-data.js`.
- Images: `assets/images/*.webp` and `assets/images/og-*.jpg` (social previews). Replace original illustration assets if desired, retaining the image dimensions and names.
- Sitemap and search data are pre-generated. If adding pages manually, remember to add them to `sitemap.xml` and `assets/search-data.js`, and use unique canonical and OG URLs.
- All visible copy uses the chosen spelling **Pal**. Historic scholarship cited through external URLs may use alternative transliteration in source filenames and bibliographic titles; the visible site does not.

## Editorial standards

- Reigns and numbering are explicitly provisional. No invented historical portraits are presented as actual images.
- The visual presentation deliberately foregrounds Hindu sacred art and architecture while the text retains documented Buddhist historical context.
- Visual artwork is original modern interpretive material. Links to museum collection records permit verification of authentic objects; no third-party museum photographs are redistributed.
- This website is commemorative and independent, not the official website of any present sovereign body or public institution.

## SEO and sharing

Full pre-rendered crawlable HTML, individual page descriptions and titles, canonical URLs, Open Graph tags, Twitter/X summary large image cards, 1200×630 JPEG social images, XML sitemap, robots.txt, hreflang tags, semantic HTML, relevant structured JSON-LD, internal linking, accessible navigation and local search.

Search engines decide whether and when to index pages. Social sharing displays depend on the platform's cache and individual crawler behaviour.
