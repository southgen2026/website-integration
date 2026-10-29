# SouthGen Management Inc. — Website

Multi-page website for SouthGen Management Inc., a Philippine-based BPO in General Santos City.

## Files

| File | Description |
|------|-------------|
| `southgen_website_v2.html` | **Main site** — Home page (hero, services, team, about, contact form) |
| `southgen_virtual_office.html` | Virtual Office page — remote staffing details |
| `southgen_careers.html` | Careers / Join Our Team page |

> Rename `southgen_website_v2.html` → `index.html` when deploying so the root URL loads the home page automatically.

## Deployment (GitHub Pages)

1. Create a GitHub repository (e.g. `southgen-website`).
2. Upload all three HTML files — rename `southgen_website_v2.html` to `index.html`.
3. Upload the `CNAME` file if using a custom domain (see below).
4. Go to **Settings → Pages**, set source to `main` branch / root.
5. Your site will be live at `https://<your-github-username>.github.io/southgen-website/`
   or at your custom domain once DNS is configured.

## Custom Domain Setup

1. Add `CNAME` file to the repo root containing your domain (e.g. `southgen.com.ph`).
2. In your domain registrar (e.g. GoDaddy, Namecheap), add these DNS records:

### Apex domain (southgen.com.ph)
```
Type: A   Name: @   Value: 185.199.108.153
Type: A   Name: @   Value: 185.199.109.153
Type: A   Name: @   Value: 185.199.110.153
Type: A   Name: @   Value: 185.199.111.153
```

### www subdomain
```
Type: CNAME   Name: www   Value: <your-github-username>.github.io
```

DNS changes may take up to 48 hours to propagate.

## Contact Form

The contact form on the main site is wired to WhatsApp (+63 927 944 4620).  
When a visitor submits the form, WhatsApp opens with a pre-filled message containing their inquiry details.

## Social Links

| Platform | URL |
|----------|-----|
| Facebook | https://www.facebook.com/SouthGenManagement |
| Instagram | https://www.instagram.com/southgen.mgt/ |
| LinkedIn | https://www.linkedin.com/company/southgen-management-inc |

## WhatsApp CTA

Both "Book a Free Consultation" buttons link to:  
`https://wa.me/639279444620`

## Tech Notes

- All images are **base64-embedded** — no external image hosting needed.
- Fonts loaded from Google Fonts (internet connection required to render correctly).
- No backend required — fully static HTML.
- All three pages link to each other via relative `href` — keep them in the **same folder**.
