# TLPT registration hosting

GitHub Pages serves the unlisted form at https://register.tlpt.org/.
Porkbun CNAME: `register` → `bostnmike.github.io`.

The source of truth remains `register.html` in `bostnmike/TLPT-poker`.
This repository contains only the publishing workflow: no player submissions,
photos, credentials, duplicated form source, or cashier code.

Run **Actions → Publish registration → Run workflow** after a form edit for
immediate publication. An hourly scheduled run also picks up changes automatically
(GitHub schedules can be delayed and are disabled after 60 days of repository
inactivity; manual publishing remains available).

Artwork, shared styles, navigation and scripts load from https://tlpt.org/.
FormSubmit continues to deliver the answers, JSON and photos to the commissioner's
existing inbox. The confirmation returns to the registration subdomain.
The form is unlisted and requests no indexing; it is not password protected.

GitHub Pages settings must use **GitHub Actions**, custom domain
`register.tlpt.org`, and **Enforce HTTPS** once the certificate is issued.
No Cloudflare project is required. Do not change the main site or cashier DNS.
