# BLDLNE Website

Static marketing and legal site for [BLDLNE](https://bldlne.app). This repository is independent from the BLDLNE Expo mobile app.

Plain HTML and CSS only — no build step, no dependencies.

## Pages

| File | Description |
|------|-------------|
| `index.html` | Home |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service |
| `support.html` | Support contact |
| `delete-account.html` | Account deletion requests |

Legal copy is sourced from the BLDLNE mobile app (`privacy-policy`, `terms-of-service`, `contact` screens).

## Local preview

Open any HTML file in a browser, or serve the folder:

```bash
cd bldlne-website
python3 -m http.server 8080
```

Then visit http://localhost:8080

## Deploy to Cloudflare Pages

1. Push this repository to GitHub.
2. In [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
3. Select the `bldlne-website` repository.
4. Build settings:
   - **Framework preset:** None
   - **Build command:** (leave empty)
   - **Build output directory:** `/` (repository root)
5. Deploy. Cloudflare will serve `index.html` at the site root.

Custom domain: add `bldlne.app` (or your subdomain) under **Custom domains** for the Pages project.

## Support

support@bldlne.app
