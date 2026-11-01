# TechBuilder website

A static, responsive landing page for https://techbuilder.dev. No build step, JavaScript framework, or paid hosting required.

## Publish on GitHub Pages

1. In the `tech-builder-dev` organization, create a **public** repository named `tech-builder-dev.github.io` (if available). If a Pages site already exists, inspect it before replacing anything.
2. Upload the files in this folder to the repository root on the `main` branch (not a nested folder).
3. Open repository **Settings → Pages**. Choose **Deploy from a branch**, `main`, `/ (root)` and Save.
4. In **Settings → Pages → Custom domain**, enter `techbuilder.dev`. GitHub may take time to validate it. Keep the `CNAME` file committed.
5. Before editing DNS, export/screenshot all current GoDaddy DNS records, especially MX, TXT (SPF, DKIM, DMARC), CNAME records for newsletter and email, and any verification records.
6. In GoDaddy DNS, update only the records required for the website apex (`@`). GitHub Pages currently documents these IPv4 A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. Confirm these against GitHub's current official docs before changing them. Remove conflicting apex A/AAAA records only after verifying their purpose; do not touch email/newsletter records.
7. Optionally set `www` as a CNAME to `tech-builder-dev.github.io` (only if `www` is not already serving something important). GitHub Pages can redirect between apex and www after both are configured.
8. After DNS propagates, enable **Enforce HTTPS** in Pages and test `https://techbuilder.dev` on desktop and mobile.
9. Check navigation, favicon, metadata, and GitHub links. Submit `https://techbuilder.dev/sitemap.xml` to Google Search Console if desired.

## Before launch

- `mailto:hello@techbuilder.dev` is a **placeholder**. Replace it with an address you actually monitor or remove the contact link. Do not create or change MX records just for this placeholder.
- LinkedIn, X, newsletter signup and book/product links are intentionally **not fabricated**. Add verified URLs and a real signup form when available.
- No analytics or third-party scripts are installed. Add privacy-conscious analytics after choosing a provider.
- This landing page intentionally makes no claims of existing clients, staff, or product adoption.

## Official guidance

https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
