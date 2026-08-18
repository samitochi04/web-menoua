# Menoua — Vercel static site

This folder is intentionally a plain static HTML site:
- `index.html` is the root page
- `privacy.html` is the privacy policy
- `terms.html` is the terms of service
- no build command
- no framework
- no dependencies
- no `vercel.json` is required

## Vercel settings

When importing this folder/repository into Vercel:

- Root Directory: `.`
- Framework Preset: leave Vercel's static/default handling; do not force Next.js
- Build Command: leave empty/default
- Output Directory: leave empty/default

Most importantly, deploy the contents of this folder as the project root. Do not deploy the parent directory containing this folder as a nested `web/` directory.

After deployment, these paths should work:
- `/`
- `/privacy.html`
- `/terms.html`

If using the Vercel CLI from this folder:
`vercel --prod`

Vercel's current NOT_FOUND troubleshooting says to verify the deployment output and make sure an index is present, and to check Root Directory / Output Directory when the deployment output is wrong.
