# SouthGen Management Inc. — Website

A two-page marketing site, built as plain, self-contained HTML files.
No build step, no server, no dependencies to install.

## What's in this folder

```
southgen-site/
├── index.html          Main page (home)
├── creatives.html      Creative services & pricing page
├── styles.css          Reference copy of the site's CSS
├── script.js           Reference copy of the site's JS
└── assets/
    ├── logo.png           Full logo (icon + wordmark)
    ├── logo-mark.png      Icon-only mark
    ├── board/             Board of directors photos
    ├── culture/           Team culture photos (slideshow)
    └── legal/             SEC Certificate of Incorporation
```

## Viewing the site

Double-click `index.html` or `creatives.html` to open either one in
any browser. Both pages are fully self-contained — all styling,
scripts, and images are embedded directly in the HTML, so nothing
breaks if the files are moved, emailed, or opened offline.

## Publishing it live

To put this on a real domain (e.g., southgensolutions.com), upload
both HTML files to any standard web host, keeping the filenames
exactly as they are. A few options:

- Your existing hosting, if the domain is already set up
- Netlify or Vercel — free, drag-and-drop the two files
- Any cPanel / FTP host — upload into the `public_html` folder

If you'd like help publishing directly, just ask.

## Making edits

For content changes — prices, phone numbers, team bios, adding a
photo — it's easiest to just describe the change and have it done
directly.

If editing by hand: **the live pages read from the `<style>` and
`<script>` blocks built into `index.html` and `creatives.html`
themselves.** `styles.css` and `script.js` are kept alongside as
readable reference copies, but changing them alone won't update the
site — the HTML files would need their inline blocks updated too.

## Good to know

- **Brand colors:** navy `#002d4b` / `#0b3c5d`, tan `#d8c3a5`, cream `#eae4dc`
- **Fonts:** Playfair Display (titles), Poppins (subtitles), Public
  Sans (body) — all free via Google Fonts. The original brand sheet
  specified "The Seasons" for titles, which is a paid font not
  available on any free CDN, so Playfair Display stands in as the
  closest match.
- **Contact CTAs:** WhatsApp (+63 927 944 4620) and email
  (admin@southgensolutions.com) are wired up as clickable links
  throughout.
- **SEC certificate:** the image in the "Corporate Registration"
  section is the actual Certificate of Incorporation, not a mockup.
