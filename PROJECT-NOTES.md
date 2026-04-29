# Pinaka Legal Main Site Project Notes

This file is the master memory note for the main website project. At the end of any future chat, ask: "Update PROJECT-NOTES.md before we close." In a new chat, ask: "Read PROJECT-NOTES.md and continue."

## Project Purpose

Maintain the static main website for:

```text
https://www.pinakalegal.com
```

The non-www root domain `pinakalegal.com` is not the official working URL right now. Use the `www` URL everywhere for SEO, links, Google Business Profile, Search Console, sitemap, and canonical URLs.

Current public phone number used in hardcoded HTML contact links:

```text
+91 8595704798
tel:+918595704798
```

## GitHub Repository

```text
https://github.com/adityaLegalRepublic/pinakalegal.com.git
```

Local project folder:

```text
/Users/tiwari/Documents/GitHub/pinakalegal.com
```

The current main branch is pushed to GitHub. Local SSH push is configured and works for this repo.

## Cloudflare Pages

Cloudflare Pages project:

```text
pinakalegal-com
```

Live domains:

```text
https://www.pinakalegal.com
https://pinakalegal-com.pages.dev
```

Deployment method:

```text
Direct Upload
```

Important: this Cloudflare Pages project is not GitHub-connected. Cloudflare reported `source: null`. Therefore pushing to GitHub alone does not update the live main site.

Normal publishing workflow for the main site:

```text
Edit local repo -> commit -> push main -> direct-upload same files to Cloudflare Pages -> verify live URL
```

Cloudflare API access is available for Pages/DNS management, but do not store API tokens in this file. If Cloudflare access is needed in a future chat, ask the user for current authorized access or verify the existing local/session token.

Last known successful direct-upload deployment:

```text
Project: pinakalegal-com
Deployment ID: 54903e8a-8f11-4172-9f11-cd2c40b4e535
Deployment URL: https://54903e8a.pinakalegal-com.pages.dev
Purpose: published new phone number +91 8595704798
```

## DNS And Domains

Wix currently manages DNS for `pinakalegal.com`.

Recommended current Wix DNS records:

```text
CNAME www.pinakalegal.com  -> pinakalegal-com.pages.dev
CNAME blog.pinakalegal.com -> pinaka-legal-blog.pages.dev
```

The old/fake A record should not be used:

```text
pinakalegal.com -> 123.45.67.89
```

Cloudflare has a `pinakalegal.com` zone, but it was last seen as `pending`, meaning nameservers/DNS authority were not fully moved to Cloudflare. Until that is fixed, root-domain behavior may still depend on Wix.

Pending future improvement:

```text
Make pinakalegal.com redirect to https://www.pinakalegal.com
```

No server is required for this; later it can be solved through proper DNS/Cloudflare routing/redirect setup.

## SEO URL Policy

Use this as the official main-site URL:

```text
https://www.pinakalegal.com
```

Main-site canonical URLs, `sitemap.xml`, and `robots.txt` should use `www.pinakalegal.com`.

## Related Blog Project

Blog website:

```text
https://blog.pinakalegal.com
```

Blog GitHub repo:

```text
https://github.com/adityaLegalRepublic/pinaka-legal-blog.git
```

Blog local folder:

```text
/Users/tiwari/Documents/New project 2
```

Blog Cloudflare Pages project:

```text
pinaka-legal-blog
```

Blog deployment method:

```text
GitHub connected auto-deploy from main
```
