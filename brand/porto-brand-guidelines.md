# Porto

Porto is a family-controlled profile that helps every new support worker, camp leader or school aide support a minimally verbal autistic child well from their first shift. The name comes from *port*, a harbour: a calm, safe place where you know where you are. The brand should feel the same way: **warm, calm, and quietly sure of what to do next.**

Porto is light-theme only. Its look is humanist minimalism: lots of soft space, one warm accent, plain words, and hand-drawn doodle people.

## Personality

| We are | We are not |
| --- | --- |
| Warm: we sound like a kind, experienced carer | Saccharine, cutesy or pitying |
| Calm: few elements, soft colours, nothing urgent | Clinical, alarming or busy |
| Assured: clear steps, specific advice | Vague, salesy or full of jargon |
| Respectful: the child and family lead | Talking about autistic people as problems to fix |

## Voice and copy

- Write plainly, the way a trusted support worker talks. Short sentences, everyday words.
- Lead with what to do: "Offer the same food again before trying something new," not "Food preferences may vary."
- Put the family in charge: "Families choose who sees the profile," "Shared by Susie's family."
- Use identity-first or person-first language as the family prefers; default to "autistic child" and "minimally verbal".
- Buttons say exactly what happens: "Join the waitlist", "Share for this shift". Confirmation: "You're on the list."
- Avoid: "suffers from", "special needs", "warriors", exclamation marks, and puzzle-piece imagery.

**Tagline:** Know what to do, from the first shift.

## Logo

The wordmark is lowercase **porto** in Fraunces SemiBold, ink coloured. The final "o" is a sun resting on a wave: the warmth of the sun over a calm harbour. The mark on its own (sun and wave) is used for small spaces and app icons. See the Logos group for files, clear space and minimum sizes.

- Primary: ink wordmark on `ground` or `surface`.
- Reversed: white wordmark on `ink` only. The sun always stays `apricot`.
- Never on `apricot`, never recoloured, outlined, shadowed or stretched.

## Colour

Use roughly **60 / 30 / 10**: `ground` for the page; `surface` and `ink` for structure and text; `apricot` for the few things that matter most.

- **Ground** `ground` (harbour mist, a lavender-tinted white) is the page background. `surface` (white) is for cards, the form panel and the illustration's backdrop blob.
- **Text** is always `ink` (headings), `ink-soft` (body) or `muted` (captions). Never put text in `apricot`, `sky` or `rose`.
- **Apricot** is the one warm accent: primary buttons, the logo's sun, and fills in the illustrations. Keep it to about one primary button per screen.
- **Sky** and **rose** are only for illustration fills and soft tags.
- `success` is only for confirmation messages.

## Typography

- **Fraunces SemiBold** (Google Fonts) for headings: `hero`, `h2`, `h3`. Its soft serifs bring the warmth. Use `text-wrap: balance` on headings.
- **Figtree** (Google Fonts) for everything else: `body-lg` for intro text, `body` for paragraphs, `small` for captions, `button` for buttons and nav.
- Keep paragraphs around 60 to 70 characters wide. Centre the hero only; left-align longer text.

## Illustration

Doodle-style human figures, drawn as if with one pen:

- A single `ink` line, about 2px at 1x, round caps and joins, slightly wobbly but confident. No gradients, no shadows.
- Sparse flat fills in `apricot`, `sky` or `rose` on clothing or objects, usually one or two per figure. Faces stay unfilled.
- Calm faces: closed or softly smiling eyes, simple shapes, diverse figures without caricature.
- Scenes show connection and everyday moments: an adult and child side by side, a worker reading the profile, a meal, a quiet corner, headphones, a book or checklist, a sun, a plant, water.
- Set scenes on a soft `surface` blob over `ground`, with a few small leaf shapes in `blob` or `sky` drifting nearby.
- Never: puzzle pieces, sad or distressed children as a hook, medical equipment, stock photos.

## Components

**Primary button.** Fill `apricot`, text `ink` in the `button` style, 2px `ink` border, radius `radius-md`, shadow `shadow-button`. Hover: fill `apricot-deep`. Pressed: shadow 1px 1px and move 2px down-right. Focus: 3px `ink` outline with 3px offset.

**Secondary button / link.** Text `ink`, underline on hover, no fill.

**Inputs and selects.** Fill `surface`, 1.5px `control-border`, radius `radius-sm`, 48px tall, `body` text in `ink`. Labels above in `small` 600 `ink-soft`. Focus: border `ink` plus a 3px `sky` ring.

**Cards and form panel.** Fill `surface`, radius `radius-lg`, padding `space-6`, 1px border in `blob`, no shadow.

**Nav.** Logo left, links in `ink-soft`, primary button right.

## Using this with the existing waitlist page

The current page's layout, copy, sections and interactions stay exactly as they are. Only the brand changes:

1. Replace the logo and product name placeholder with `porto-logo.svg` and "Porto".
2. Swap the colour variables for the tokens above (old teal-grey background → `ground`, old dark teal → `ink`/`ink-soft`, old yellow → `apricot`, old hover yellow → `apricot-deep`).
3. Recolour the illustration to the illustration rules (ink lines; apricot, sky and rose fills).
4. Use Fraunces for headings and Figtree for body text, if the page doesn't already.
5. Set the favicon to `porto-mark.svg` and the page title to "Porto: Know what to do, from the first shift".

## CSS variables

```css
:root {
  --ground: #F3F1FA;
  --surface: #FFFFFF;
  --blob: #E7E3F4;
  --ink: #24304F;
  --ink-soft: #4A5372;
  --muted: #646A88;
  --control-border: #7F84A3;
  --apricot: #F5B07A;
  --apricot-deep: #E3894A;
  --sky: #C9DAF2;
  --rose: #F4CFC6;
  --success: #2F6E4E;
  --radius-sm: 10px;
  --radius-md: 14px;
  --radius-lg: 24px;
  --shadow-button: 3px 3px 0 #24304F;
  --font-display: "Fraunces", Georgia, serif;
  --font-sans: "Figtree", system-ui, sans-serif;
}
```

Google Fonts: `https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,600&family=Figtree:wght@400;600&display=swap`

## Logo files

- `porto-logo.svg`: the primary wordmark. Lowercase "porto" in Fraunces SemiBold, with the final "o" drawn as an apricot sun resting on a wave. Use it on ground or surface.
- `porto-logo-white.svg`: white wordmark (the sun stays apricot) for use on ink backgrounds only.
- `porto-mark.svg`: the sun-and-wave mark on its own, for small spaces, social avatars and favicons.
- `porto-app-icon.svg`: the mark on a rounded harbour-mist tile, for app icons.

Clear space: keep empty space around the logo at least the height of the sun on every side. Minimum size: wordmark 88px wide on screen; mark 20px.

Don't: recolour the sun, outline or add shadows to the logo, stretch it, rebuild it in another typeface, or place it on an apricot background.
