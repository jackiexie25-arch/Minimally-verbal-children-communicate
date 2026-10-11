# Porto — waitlist landing page

A plain static "join the waitlist" page for Porto, a family-controlled profile app for minimally verbal children.

- No framework, no build step: `index.html`, `success.html`, `styles.css`.
- Sign-ups go to **Netlify Forms** (form name: `waitlist`). There is no custom backend.
- Brand (logo, colours, type, illustration rules): [`brand/porto-brand-guidelines.md`](brand/porto-brand-guidelines.md). Layout and spacing: [`STYLE.md`](STYLE.md).

## Files

| File | What it is |
|---|---|
| `index.html` | Landing page: hero + waitlist form, problem, how it works, who it's for, bottom call to action, footer |
| `success.html` | Thank-you page the form redirects to |
| `styles.css` | The only stylesheet (mobile-first) |
| `netlify.toml` | Tells Netlify to publish the repo root with no build command, and adds basic security headers |
| `porto-logo.svg`, `porto-mark.svg` | Wordmark (header) and mark (favicon) |
| `brand/` | Porto brand guidelines, white logo and app icon |
| `STYLE.md` | Original layout brief (the palette and type in it are superseded by the Porto brand) |

## Contact and social links

The footer of `index.html` and `success.html` has:

- Team email: porto.communicate@gmail.com, as a `mailto:` link (opens the visitor's default email app) plus a "write to us in Gmail" link that opens Gmail's compose window in a new tab
- Icon links (open in a new tab) to Facebook, LinkedIn and Instagram. To change a link, edit the `href` in the `<nav class="social">` block on both pages.

Brand icons are from Font Awesome Free 6.5.2 (CC BY 4.0).

## Run locally

Any static file server works, for example:

```sh
python3 -m http.server 8080
# open http://localhost:8080
```

Submitting the form locally won't store anything. Netlify only processes the form once the site is deployed on Netlify.

## The form

```html
<form name="waitlist" method="POST" data-netlify="true" netlify-honeypot="bot-field" action="/success.html">
```

| Field | Name | Required |
|---|---|---|
| Email | `email` | yes (`type="email"`) |
| Role | `role` | yes: Family member / Support worker / Agency or provider / Camp or school / Other |
| Organisation name | `organisation` | no |
| Honeypot (hidden spam trap) | `bot-field` | must stay empty |

The form deliberately asks nothing about the child.

## Accessibility

- Every input has a visible `<label>`; required fields use native `required` validation.
- Text contrast meets WCAG AA (body text 6.8:1, headings 11.7:1, button text 7.1:1 on apricot and 4.9:1 on hover).
- Keyboard: skip link, logical tab order, and a strong focus ring (3px ink outline; inputs get an ink border plus sky ring).
- Respects `prefers-reduced-motion`. Decorative illustrations are hidden from screen readers; the hero illustration has a text description.
