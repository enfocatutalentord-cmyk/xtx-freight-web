# XTX Freight Group — xtxfreightgroup.com

Static one-page website for XTX Freight Group LLC, deployed on Vercel from this repository.

## Structure

```
index.html                              Landing page
privacy-policy-for-sms/index.html       /privacy-policy-for-sms/
terms-and-conditions-for-sms/index.html /terms-and-conditions-for-sms/
thanks/index.html                       Shown after the contact form is sent
assets/                                 Styles, logos, photos, social image
favicon.svg, apple-touch-icon.png       Browser and phone icons
vercel.json                             Clean URLs and headers
```

No build step: Vercel serves the files as they are (Framework preset: "Other").

## Updating the site

Edit the files, commit and push to `main`. Vercel publishes the change automatically in about a minute.

## Contact form

The form sends to `Support@xtxfreightgroup.com` through FormSubmit. The first submission triggers a one-time activation email to that inbox; click the link in it and later messages arrive normally.

## Pending content

- USDOT and MC numbers (search `[NUMBER]` in `index.html`)
- Coverage area (search `[COVERAGE AREA]`)
- Effective date on both SMS pages (search `[DATE]`)
- Replace `assets/hero-truck.jpg` and `assets/truck-door.jpg` with real fleet photos when available

## Domain (DNS at Bizee)

Add the domain in Vercel → Project → Settings → Domains, then create the two records Vercel shows (an `A` record for the root and a `CNAME` for `www`) in the Bizee DNS panel. Do not change the nameservers or the MX records, or the company email will stop working.
