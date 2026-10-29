# SouthGen Management Inc. — Website

Multi-page website for SouthGen Management Inc., a Philippine-based BPO in General Santos City.

## Files

| File | Description |
|------|-------------|
| `HOMEPAGE.html` | **Main site** — Home page (hero, services, team, about, contact form) |
| `Virtual_Office.html` | Virtual Office page — remote staffing details |
| `CAREERS.html` | Careers / Join Our Team page |
| `Credit_repair.html` | Credit Repair VA SEO landing page |

> Rename `HOMEPAGE.html` → `index.html` when deploying so the root URL loads the home page automatically.

## Deployment (GitHub Pages)

1. Create a GitHub repository (e.g. `southgen-website`).
2. Upload all four HTML files — rename `HOMEPAGE.html` to `index.html`.
3. Upload the `CNAME` file (custom domain).
4. Go to **Settings → Pages**, set source to `main` branch / root.
5. Your site will be live at `https://southgenmanagement.com` once DNS is configured.

## Custom Domain Setup

1. Add `CNAME` file to the repo root containing `southgenmanagement.com`.
2. In your domain registrar (e.g. GoDaddy, Namecheap), add these DNS records:

### Apex domain (southgenmanagement.com)
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

## Internal Links

All four pages link to each other — keep them in the **same folder** when deploying.

| From | Links to |
|------|----------|
| HOMEPAGE | Virtual_Office, CAREERS, Credit_repair |
| Virtual_Office | HOMEPAGE |
| CAREERS | HOMEPAGE |
| Credit_repair | HOMEPAGE |

## Contact / Forms

All forms and "Book a Free Consultation" buttons redirect to WhatsApp:
`https://wa.me/639279444620` (+63 927 944 4620)

## Social Links

| Platform | URL |
|----------|-----|
| Facebook | https://www.facebook.com/SouthGenManagement |
| Instagram | https://www.instagram.com/southgen.mgt/ |
| LinkedIn | https://www.linkedin.com/company/southgen-management-inc |

## Tech Notes

- All images are **base64-embedded** — no external image hosting needed.
- Fonts loaded from Google Fonts (internet connection required to render correctly).
- No backend required — fully static HTML.
- All four pages must be in the **same folder** for internal links to work.
