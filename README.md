# Code 73 — code73.co.uk

Single-page site for Code 73 Ltd (Danny Woolston), built as one self-contained `index.html`.

## Deploy to GitHub Pages

1. Create a GitHub repo (e.g. `code73-site`), push this folder.
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
3. Custom domain: enter `code73.co.uk` (this writes the `CNAME` file — already included here) and tick **Enforce HTTPS** once the certificate is issued.

## DNS (at 123-Reg, when moving off Wix DNS)

Apex `code73.co.uk` A records → GitHub Pages:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
`www` CNAME → `<github-username>.github.io`

Keep the email records (Zoho):
```
MX  @  mx.zoho.com   10
MX  @  mx2.zoho.com  20
MX  @  mx3.zoho.com  50
TXT @  v=spf1 include:zohomail.com ~all
CNAME zb14701334 → zmverify.zoho.com
```
