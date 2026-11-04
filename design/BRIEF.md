# amin-niyazov.com redesign: design brief (2026-11-04)

Working document; excluded from deploys by `.vercelignore`.

## Design read
A family memorial and a serious biography of a Soviet Uzbek statesman (1903–1973), read in five
languages by family, historians and people who arrive from the documentary. Register: dignified,
warm, cinematic and scholarly, never a campaign poster.

## Concept spine: *Abr*, the cloud thread
Niyazov was born at Ak-Tepe near Margilan, the home of Uzbek ikat silk (*abr*, "cloud"). The film's
title card already sits on blurred ikat with a Cormorant serif and a gold rule. The site takes the same
identity: ikat silk is the woven thread of the page. A vertical warp thread (the chapter rail) carries the
reader through the life as dated waypoints, and every chapter opens on its years.

## Delivery tier
`editorial`: typography, real archival photographs and bespoke chrome, with micro-motion only.
Animation mode: non-animated. It is a memorial with a 21-minute film as the cinematic centrepiece.
A scroll-driven generated film of real places would invent history, so there is none.

## Combinatorial pick (held across all boards)
- Theme paradigm: Deep Dark with a twist (ikat night indigo, not graphite); light mode = mulberry paper.
- Background: solid with soft ambient depth + tactile silk/paper texture.
- Typography: editorial serif + sans pairing.
- Hero architecture: cinematic centered, with the real portrait in a museum mount.
- Section system: alternating editorial blocks inside a reading column with a sticky chapter rail.
- Signature components: vertical rhythm lines (chapter rail) · oversized metrics strip ·
  layered image crop frames (gallery) · career ladder (offices on a 1900–1975 axis).
- Narrative spine: journey / waypoints.
- Second-read moment: oversized chapter years as structure.

## Locked palette (dark first)
| Token | Dark | Light | Defence |
|---|---|---|---|
| ground | `#0D1222` night indigo | `#F6F4EF` mulberry paper | ikat indigo dye; Samarkand paper |
| surface | `#141B31` | `#FFFFFF` | |
| ink | `#ECE6DA` silk ivory | `#141A2E` | |
| muted | `#A3A1AC` | `#5C5D69` | AA on both grounds |
| accent | `#E2B04A` Margilan saffron | `#8A5A00` | the film's gold rule; AA on paper |
| ikat only | madder `#A5302E` · emerald `#1F6F5C` · indigo `#2B3A7A` | same | never UI chrome |

The accent is the user's own film identity (gold rule on dark ikat). That is the brand-colour exception to the
dark-plus-amber ban.

## Locked type
- Display: **Cormorant Garamond** 500/600 + italic. It is the film's title face and has full Cyrillic.
- Text: **Literata** 400/600 + italic: a sturdy screen serif for long reading, with Cyrillic.
- UI, labels, numerals: **IBM Plex Sans** 500/600: an engineer's sans for the builder; Cyrillic, and Uzbek ʻ.

## Section plan
1. Top bar: seal, name, Chapters index, language, theme. Reading-progress thread.
2. Hero: real portrait in a mount over a blurred ikat field; name, Cyrillic name, dates, titles; CTAs.
3. Film: theatre frame, EN/RU switch, meta row.
4. At a glance: fact file + career ladder chart (replaces the sticky Wikipedia infobox).
5. Chapters (biography → legacy): sticky rail + 68ch column; pull quotes on an ikat thread;
   metrics strips; What He Built bento with custom icons; Fall with its two subsections.
6. Contemporaries: role-tagged cards.
7. Gallery: real aspect ratios, captions below, accessible lightbox (dialog, swipe, keys).
8. Family: parents and four children.
9. Sources: grouped accordions.
10. Colophon footer: dedication, related memorials, languages.

## Asset plan (Higgsfield)
- Reference boards per section (gpt_image_2_5, high, 2k), stored in `design/boards/`.
- Ikat silk textile family (hero field, divider strip, night grade); mulberry-paper texture.
- Custom icon set (6 domains + awards) generated as one sheet, vectorised to SVG for theming.
- No generated people or places. Every photograph of a person is a real archival photo, untouched.
- OG card composed from the real portrait + type + generated silk (HTML render, not AI).

## Outcome (boards → build)
- Three hero directions were boarded (`design/boards/00–02`): A "Silk and Night" (centered), B "Inscription"
  (light, giant surname) and C "Woven Spine" (ikat panel, portrait across the seam, year rail).
  **C was chosen.** B read as a campaign poster and A as expected; C carries the concept spine and its year rail
  is real navigation.
- The section boards (03–08) and the mobile board (09) were built faithfully. The gallery comp's photographs
  are model inventions; the build uses only the real archive.
- Asset kit (`10-asset-kit-contact.jpg`): ikat A (ivory ground) became the hero panel, OG card and ribbon;
  ikat B (indigo ground) became the Water & Land tile; mulberry paper is the light-theme ground; the icon sheet,
  ganch ring and fleuron were traced to SVG.
- Higgsfield spend: 16 GPT Image 2.5 jobs at high quality, 2k, 2.75 credits each = 44 credits.

## CTA inventory
- "Watch the film · 21 min": saffron-ringed play disc + label (hero).
- "Read his life": underlined inline link with an arrow (hero).
- Film language switch: segmented silk pills.
- Chapters: index sheet trigger (top bar), rail links with thread markers.
- Gallery tiles: whole-figure buttons; lightbox controls as round glass buttons.
- Related memorials: framed cards with an arrow (footer).
