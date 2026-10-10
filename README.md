# [PRODUCT NAME] — waitlist landing page

A plain static "join the waitlist" page for [PRODUCT NAME], a family-controlled profile app for minimally verbal autistic children.

- No framework, no build step: `index.html`, `success.html`, `styles.css`.
- Sign-ups go to **Netlify Forms** (form name: `waitlist`). There is no custom backend.
- The visual style is described in [`STYLE.md`](STYLE.md).

## Files

| File | What it is |
|---|---|
| `index.html` | Landing page: hero + waitlist form, problem, how it works, who it's for, bottom call to action, footer |
| `success.html` | Thank-you page the form redirects to |
| `styles.css` | The only stylesheet (mobile-first) |
| `netlify.toml` | Tells Netlify to publish the repo root with no build command, and adds basic security headers |
| `STYLE.md` | Style brief (palette, type, layout, components, tone) |

## Before launch: replace the placeholders

Search the repo for these and replace them everywhere (`index.html`, `success.html`, `README.md`, `styles.css` comment):

- `[PRODUCT NAME]`
- `[TEAM EMAIL]` (used in the footer `mailto:` link)

```sh
grep -rn "\[PRODUCT NAME\]\|\[TEAM EMAIL\]" .
```

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
- Text contrast meets WCAG AA (body text 6.1:1, headings 8.6:1, button text 7.1:1).
- Keyboard: skip link, logical tab order, and a strong focus ring (teal outline plus yellow halo).
- Respects `prefers-reduced-motion`. Decorative illustrations are hidden from screen readers; the hero illustration has a text description.
