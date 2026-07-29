# Handoff: IT-sikkerhed i kontorfællesskaber — slide deck

## Overview
A 27-slide presentation deck (Danish) about IT security in shared office spaces ("kontorfællesskaber"), aimed at a non-technical audience. Warm Scandinavian nature aesthetic. Presented by Gorm Reventlow (FynBus, IT compliance / NIS2). Talk length: 45–60 minutes.

## About the Design Files
The files in this bundle are **design references created in HTML** — they show the intended look, content, and behavior. They are not production code to ship directly. Your task is to **recreate this deck in the target environment** — e.g. a web deck framework (reveal.js, Slidev), PowerPoint/Keynote via a generator, or a React app — using that environment's established patterns. If no environment exists yet, a static HTML/CSS deck (like the reference) or reveal.js is the most appropriate choice.

`IT-sikkerhed i kontorfællesskaber.dc.html` is the source of truth. Each slide is a `<section>` inside a `<deck-stage>` wrapper (`deck-stage.js` provides scaling, keyboard/tap navigation, thumbnail rail, speaker-notes and print-to-PDF; `image-slot.js` provides a drag-and-drop portrait placeholder on slide 2). Recreate the slides; replace the stage/slot components with your framework's equivalents.

## Fidelity
**High-fidelity.** Colors, typography, spacing, and copy are final. Recreate pixel-perfectly at 1920×1080 (16:9). All copy is Danish — reproduce it exactly as in the HTML (it has been proofread; do not re-translate).

## Slide inventory (27 slides)
Three recurring layout archetypes + one-off diagram slides:

1. **Titel** (dark) — kicker "Et fælles ansvar", H1 "IT-sikkerhed i kontorfællesskaber", subtitle, presenter name with 64×4px terracotta rule. Decorative circles (see Decorative motif).
2. **Kort om mig** (light content) — 380×380px circular portrait placeholder left; name (Lora 58/500), role paragraph, two contact pills (`gorm@reventlow.com`, `20 52 93 67`, bg #EAE0CD, radius 999px).
3. **Dagens program** (light content) — 2-col × 6-row grid, gap 34×120px; each row: Lora 28px terracotta number (01–12, 44px wide) + Work Sans 31px topic.
4. **Kapitel 01 · Det fælles ansvar** (chapter divider).
5. **Ligesom det fysiske kontor** — intro line + 3 mapping rows, grid `1fr 90px 1fr`: sand pill ("Vi låser døren") → terracotta Lora arrow "→" → cream card with border ("Vi låser skærmen"). Pairs: låser døren/låser skærmen; lukker vinduerne/lukker sikkerhedshullerne; slår alarmen til/har backup af det vigtige.
6. **Følsomme data og tillid** (light statement) — Lora 76/500 "Flere af jer arbejder med følsomme data for klienter." + 38px sub. Sage circle decoration bottom-left.
7. **Sikker nok til jeres data** — intro + two sand cards (radius 22, padding 52/56) numbered "1." / "2." (Lora 44 terracotta) with Lora 40px questions.
8. **Det mest kritiske behov** (dark statement, centered) — 64×4px terracotta rule, Lora 84/500 "Fællesskabet følger det mest kritiske behov.", 34px sub at 75% cream.
9. **Kapitel 02 · Det fælles netværk** (divider).
10. **Ét netværk, fri trafik** — hub-and-spoke diagram: dark pill "Routeren" (30px, padding 22/56, radius 999) → 2×42px vertical line → 1140×2px horizontal line → 4 columns (340px wide, gap 40) each with 2×32px tick + chip (28px text, padding 26/20, bg #FFFDF6, border 2px #C9C3AF, radius 16). 4th chip highlighted: bg #F5E4D6, border #C05F33, text "Gæstens telefon og bærbar". Line/tick color #B9BCA8. Caption 34px centered below.
11. **Segmentér netværket** — 3 equal cards (radius 24, padding 44/44/48): "Arbejdsnetværket" solid 3px #7E9070 border on #FFFDF6; "Gæstenetværket" dashed 3px #C05F33 on #FFFDF6; "Hver for sig?" dashed 3px #B9BCA8, no bg. Card title Lora 38/600, body 29px. Note line 31px below.
12. **Kapitel 03 · Jeres computer** (divider).
13. **Den største angrebsflade** (light statement) — Lora 76/500 line 1 "Computeren er den største angrebsflade," + line 2 italic terracotta "fordi der sidder et menneske bag." + 38px sub.
14. **Fire gode vaner** — 2×2 grid of sand cards (radius 22, padding 40/48, gap 32): terracotta Lora 30px number, 33/600 title, 27px body. Titles: Kun til arbejde / Firewallen slået til / Microsoft Defender / Fast opdateringsdag.
15. **Kapitel 04 · Fælles udstyr** (divider).
16. **Printeren og serveren** — intro + two sand cards (Lora 40/600 titles "Printeren", "Serveren / NAS", 29px body) + "Husk:" note line (label terracotta 600).
17. **Andres USB-nøgler** — 3 stacked rows (radius 20): rows 1–2 cream (#FFFDF6, border 2px #D8D1BC, 14px terracotta dot bullet, 32px text); row 3 emphasized dark (#2F3E33, dot #D9895C, Lora italic 36px cream): "Du låner aldrig en USB-nøgle ud. Du giver den væk."
18. **Kapitel 05 · Backup, backup, backup** (divider).
19. **3-2-1-reglen** — 3 sand cards with giant Lora 120/500 terracotta numerals 3 / 2 / 1, 33/600 sublines ("kopier af dine data" / "forskellige medier" / "kopi et andet sted"), 27px body.
20. **Kapitel 06 · IT-politik og regler** (divider).
21. **Fælles og personlig IT-politik** — two sand cards ("Den fælles" / "Din egen", Lora 42/600 + 30px body) + Lora italic 38px terracotta closer "Politikker er levende. De kan altid ændres."
22. **GDPR og NIS2** — two cream cards (border 2px #D8D1BC) with Lora 64/600 acronyms + 29px body; "Rådet:" note line.
23. **Kapitel 07 · Når uheldet sker** (divider).
24. **Fem skridt, når det går galt** — Lora italic 32px terracotta intro "Ingen skam. Ingen pegefingre. Vi standser ulykken." + 5 rows (gap 22): 62px circle (Lora 30px cream; step 1 bg #C05F33, steps 2–5 bg #2F3E33) + 31/600 text with regular-weight #4A4E42 suffix span.
25. **Truslerne derude** (dark content slide) — Lora italic 30px quote »The web is dark and full of terrors« at 65% cream; two glass cards (bg rgba(246,241,231,0.07), border 2px rgba(246,241,231,0.18), radius 22): "Phishing, nu med AI" / "Ransomware" (Lora 42/600 + 29px body at 80% cream); closing 31px line.
26. **Huskelisten** — 2-col grid (gap 34×90) of 10 checklist rows: 30×30px empty checkbox (border 3px #7E9070, radius 8) + 30px text.
27. **Spørgetime** (dark, same composition as Titel) — kicker "Tak for i dag", H2 Lora 112px "Spørgetime", contact block: Lora 44/500 name, 30px role at 75%, two outlined pills (border 2px rgba(246,241,231,0.35), radius 999).

## Layout archetypes
- **Content slide (light):** bg #F6F1E7, text #2A2E26, `flex-column`, padding `96px 110px 64px`. Kicker (26px/600, letter-spacing 0.18em, uppercase, #C05F33, margin-bottom 22px) → title (Lora 72px/600, letter-spacing −0.01em, line-height 1.08) → optional intro (34px, 1.5, #4A4E42) → content. Footer pinned via `margin-top:auto`: left = section name, right = "NN / 27", both 24px, letter-spacing 0.08em, #97998A.
- **Chapter divider (dark):** bg #2F3E33, text #F6F1E7, vertically centered, padding `0 150px`. Kicker "Kapitel NN" (28px/600, 0.22em, uppercase, #D9895C, margin-bottom 34px) → Lora 104px/600 title (line-height 1.08, letter-spacing −0.015em) → 120×4px #D9895C rule (margin-top 48px). Slide number absolute right 110px / bottom 44px at rgba(246,241,231,0.55). Identical decorative circles on all 7 dividers (parallelism is intentional).
- **Statement slide:** vertically centered, padding `0 150px` (light) or `0 200px` centered text (dark). Big Lora 76–84px/500 line, then 34–38px sub. Number absolute bottom-right.
- **Decorative motif (dark slides):** outlined circle 640–680px, border 2px rgba(246,241,231,0.14–0.16), offset top-right beyond canvas; filled sage circle 520–560px rgba(126,144,112,0.18–0.22) offset bottom-right. Title/Spørgetime add a solid 150px #C05F33 circle at right:340px/bottom:120px. All `overflow:hidden` on the slide.

## Interactions & Behavior
- Keyboard ←/→ and tap/click to navigate; slide counter overlay (provided by deck-stage — replicate with your framework's nav).
- Print-to-PDF: one page per slide at 1920×1080.
- Speaker notes: stored per-slide in `data-speaker-notes` attributes (Danish, supplementary talking points — icebreakers, examples, audience questions; deliberately NOT copies of slide text). Surface them in presenter view.
- Slide 2 portrait: drag-and-drop image slot, circular crop, placeholder text "portræt her". In production: static `<img>` with 50% border-radius once the real photo exists.
- No animations/transitions are required beyond the framework's default slide transition (subtle fade/slide is fine).

## State Management
None beyond current-slide index. Persist position (URL hash or localStorage) if the framework doesn't already.

## Design Tokens
Colors:
- Background light (birch): `#F6F1E7` (also used as cream text on dark)
- Background dark (spruce): `#2F3E33`
- Ink: `#2A2E26`; secondary ink: `#4A4E42`; muted footer: `#97998A`
- Terracotta accent: `#C05F33`; terracotta on dark: `#D9895C`
- Sage: `#7E9070`; sage fills: `rgba(126,144,112,0.14–0.22)`
- Sand card: `#EAE0CD`; cream card: `#FFFDF6`; card borders: `#D8D1BC`, `#C9C3AF`; diagram lines: `#B9BCA8`; guest highlight: `#F5E4D6`
- Cream alphas on dark: text 0.75–0.8, quotes 0.65, footers 0.55, glass cards 0.07 bg / 0.18 border
- Page letterbox behind deck: `#262B22`

Typography (Google Fonts):
- Display: **Lora** (400/500/600 + italics) — titles, numerals, quotes
- Body/UI: **Work Sans** (400/500/600)
- Scale: 112 (title slides) / 104 (dividers) / 84–76 (statements) / 72 (content titles) / 64–58 (big card text) / 44–38 (card titles) / 34–29 (body) / 27–26 (small/kicker) / 24 (footer, minimum anywhere)
- Kickers: uppercase, 600, letter-spacing 0.18–0.22em

Spacing & shape:
- Content padding 96/110/64; divider/statement padding 0/150
- Card radius 20–24px; pills 999px; checkbox radius 8px; card padding 40–52px
- Grid gaps: cards 32–40px, list rows 22–30px, checklist 34×90px
- Rules: 64–120px × 4px terracotta

## Assets
- No raster images. Slide 2 expects a portrait photo (user-supplied; circular, 380×380).
- Decorative shapes are pure CSS circles — no SVG assets.
- Fonts loaded from Google Fonts (`Lora`, `Work Sans`).

## Files
- `IT-sikkerhed i kontorfællesskaber.dc.html` — the deck (all 27 slides, inline-styled; speaker notes in `data-speaker-notes`)
- `deck-stage.js` — stage component used by the reference (scaling/nav/notes/print)
- `image-slot.js` — portrait placeholder component used on slide 2
- `scratchpad.md` — outline/title sequence and palette notes
