> **Note:** the page is now branded as **Porto**. Logo, colours, fonts and illustration colours follow [`brand/porto-brand-guidelines.md`](brand/porto-brand-guidelines.md); the palette and type below are the original pre-brand brief. Layout, spacing and components still follow this file.

# Style brief

Reference: gatheredhere.com.au. I studied it from two screenshots you sent: the desktop hero and a spot illustration. I couldn't load the live site. The hex values below are sampled from the screenshots and rounded, so treat them as close matches, not exact brand values.

**Overall feel:** calm, warm and domestic. A cool, misty teal background, one sunny yellow accent, hand-drawn line art of ordinary family moments, and lots of air around everything. It feels like a kind neighbour rather than a clinic, and that's the feeling we want.

---

## 1. Colour palette

| Role | Hex | Notes |
|---|---|---|
| Page background | `#E8F1F1` | Pale misty teal; covers the whole page |
| Soft panel / blob | `#F5F9F9` | Near-white organic blob behind illustrations; also used for card backgrounds |
| Surface (cards, form) | `#FFFFFF` | |
| Heading text | `#1D4A4D` | Deep teal, not black (8.6:1 on background) |
| Body text | `#3E5F61` | Softer teal-grey (6.1:1 on background, AA) |
| Accent / button fill | `#F7D96B` | Warm sunflower yellow |
| Button text + border + hard shadow | `#1D4A4D` | 7.1:1 on yellow |
| Decorative shapes | `#9DBDBD` | Muted sage-teal. Decorative only, never used for text |
| Line art | `#2B3436` | Charcoal hand-drawn strokes |
| Focus ring | `#1D4A4D` outline + `#F7D96B` halo | Visible on every background |

Yellow is the only warm colour. It appears on buttons and as small fills inside the illustrations (a shirt, a cheek, a flower). Everything else stays in the teal family.

## 2. Typography

- **Headings: Fraunces** (Google Fonts), weight 400 for H1 and 500 for H2–H3, `SOFT` 100 / `WONK` 0. The reference uses a gentle, slightly rounded serif ("Everything End-of-Life"), and Fraunces with its soft setting is the closest free match.
  - H1: `clamp(2.1rem, 5vw, 3.75rem)`, line-height 1.1, letter-spacing −0.01em, centred in the hero
  - H2: `clamp(1.75rem, 3.5vw, 2.5rem)`, line-height 1.15
  - H3 (card titles): 1.3rem, weight 600
- **Body / UI: Figtree** (Google Fonts), weights 400/500/600. The reference's nav and buttons use a rounded geometric sans (Proxima Nova / Gilroy style), and Figtree is the closest free option.
  - Body 1.0625rem (17px), line-height 1.6
  - Nav links 1rem, weight 400; buttons 1.125rem, weight 500
  - No all-caps and no wide tracking. Everything is sentence case.

## 3. Layout patterns

- **Max content width** ~1200px; text columns ~640px; generous side gutters (16px on mobile, 24–48px on desktop).
- **Nav:** a single slim row with the wordmark on the left, a few plain text links, and one yellow pill button on the right ("Need Help?"). A thin vertical divider sits after the logo. No background bar; the nav floats on the page colour.
- **Hero:** centred and stacked. First a wide line-art illustration on a soft near-white blob, then a big centred serif headline, then a row of yellow buttons. Lots of vertical space (~120px+ on desktop).
- **Section rhythm:** roomy, about 96–128px between sections on desktop and 64–80px on mobile. Sections are told apart by soft curved white "waves" or blobs rather than hard lines. You can see one starting at the bottom edge of the screenshot.
- **Grid / cards:** an equal-width row of buttons or cards that stacks to one column on mobile.
- **Imagery:** hand-drawn, slightly wobbly charcoal line art with selective yellow fills, placed on an irregular pale blob. Small muted-teal leaf shapes drift at the page edges as decoration.

**How I'll adapt it (no copying):** I'll draw simple **original** SVG line art in the same spirit, with charcoal strokes, yellow fills and a pale blob behind:
- Hero: an open notebook / profile card with a few cue icons, plus a small sun.
- Cards: a two-minute card, a key with a small clock (access that expires), and a sprout (gets smarter every shift).
- Decoration: small pebble and petal shapes in sage-teal.

No people copied from their art, no umbrella, no leaves in their style, and **no puzzle pieces**.

## 4. Components

- **Primary button:** yellow `#F7D96B` fill, 1.5px deep-teal border, **hard offset shadow** `4px 4px 0 #1D4A4D` (no blur), radius ~10px, generous padding (14px × 32px), deep-teal text with a small `›` chevron. On hover/press the button nudges down-right and the shadow shrinks, so it feels "pressable". This button is the reference's signature detail.
- **Nav button:** the same style, smaller.
- **Form fields:** white fill, 1.5px deep-teal border, radius 10px, 52px tall, 17px text, labels above the field in Figtree 500. The focus state is a thick yellow halo plus the teal border. (The reference shows no form, so this follows the button language.)
- **Cards:** white `#FFFFFF` on the page background, radius ~20px, no drop shadow (or a barely-there one), 1px soft border `#D5E3E3`, an illustration at the top.
- **Footer:** quiet, on a near-white wave, small teal text, plain links. (Not visible in the screenshots; I'll keep it minimal to match.)

## 5. Tone of voice

From the small amount of copy visible ("Everything End-of-Life", "Need Help?", plain service names), the voice is **plain-spoken, short and unflinching but gentle**. It names a hard subject directly without euphemism, then immediately offers help. There's no jargon, no exclamation marks and no hype.

For us, that means:
- Short sentences in everyday words ("cues", "what calms them", not "behavioural indicators").
- Talk to families as the experts on their child. Respectful and never pitying.
- Calm reassurance about privacy and control, stated plainly.
- No clinical or deficit language, no puzzle-piece or "fix" framing.
