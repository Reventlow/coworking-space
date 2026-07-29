# IT-sikkerhed i kontorfællesskaber

A Danish presentation deck about IT security in shared office spaces,
presented by Gorm Reventlow. Warm Scandinavian nature aesthetic, 1920×1080,
built as a static HTML deck with two small web components.

Footer slide numbers are computed by `deck-stage.js` from each slide's
position (skip-aware), so they never drift when slides are added or removed —
`site/index.html` holds no hardcoded `NN / NN` strings.

Live at: <https://kontor.blacklog.net>

## Structure

```
site/
  index.html            The deck - 27 inline-styled <section> slides
  assets/deck-stage.js  Stage component: scaling, keyboard/tap navigation,
                        thumbnail rail, speaker notes, print-to-PDF
  assets/image-slot.js  Drag-and-drop portrait placeholder (slide 2)
docs/                   Original design handoff and outline
Dockerfile              nginx:alpine serving site/
.github/workflows/      Builds and pushes the image to Docker Hub
```

## Run locally

```bash
cd site && python3 -m http.server 8080
# or
docker build -t coworking-space . && docker run -p 8080:80 coworking-space
```

## Usage

- Navigate: ←/→, Space, PgUp/PgDn, Home/End, or tap left/right half
- `F` toggles fullscreen, `S` toggles the slide-list rail, `N` toggles speaker notes
- On-screen buttons (bottom-left) mirror those three toggles
- `R` resets to slide 1
- Speaker notes live in each slide's `data-speaker-notes` attribute
- Print → Save as PDF gives one page per slide at 1920×1080
- Slide 2 portrait: drag a photo onto the circular placeholder

## Deployment

Pushing to `main` triggers a GitHub Action that builds the image and
pushes `coworking-space:latest` to Docker Hub. The container runs on
ZimaOS behind Nginx Proxy Manager at `kontor.blacklog.net` (DNS via
Cloudflare).
