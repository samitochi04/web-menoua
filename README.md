# Hosting these pages

Two static files. No build step, no framework, no dependencies.

## Fastest route (5 minutes, free)

**Netlify Drop** — drag this `web/` folder onto https://app.netlify.com/drop.
You get a URL immediately. Rename the site to `menoua` and you have:

```
https://menoua.netlify.app/privacy.html
https://menoua.netlify.app/terms.html
```

Those URLs are valid for the Play Console listing today. Point `menoua.app` at
the same site later; the store record can be updated.

## Alternatives

- **GitHub Pages** — push `web/` to a repo, Settings → Pages → deploy from branch
- **Vercel** — `npx vercel --prod` inside `web/`
- **Cloudflare Pages** — connect the repo, no build command

## Then

1. Play Console → App content → **Privacy policy** → paste the privacy URL
2. Play Console → **Data safety** form. Answer it honestly:
   - Audio recordings: **collected? No.** They stay on the device.
   - The waveform summary is not audio and cannot be reversed into audio.
   - Personal info: email, **optional**, for account sign-in
   - Health info: yes, optional, for exercise safety
   - Data is encrypted in transit and users can request deletion in-app
3. App Store Connect → App Privacy → the same answers

## Before launch

- Set up `privacy@menoua.app` and `support@menoua.app`. Both pages reference
  them and a bounced privacy email is a compliance problem, not a typo.
