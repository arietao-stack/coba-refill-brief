# CÔBA'S DAUGHTER — Creator Brief

**The Endless Summer Refill Ritual** — the TikTok / Reels creator brief deck for the 2-video campaign: "The Aesthetic ASMR Refill Duo" + "The Endless Summer Ritual" review (Summer 2026).

🎞️ **Live slide deck:** https://arietao-stack.github.io/coba-refill-brief/deck.html (reveal.js — arrow keys / swipe; add `?print-pdf` then Ctrl/Cmd-P to export a PDF)
🔗 **Legacy pages:** `index.html` (v1 long-form brief) · `deck-v1.html` (v1 deck, "girl math" tone)

## What's inside the deck (15 slides)
- Deliverables + filming requirements (9:16 vertical, bright clean lighting, labels readable)
- The two hero products (Robusta Coffee Scrub + Aloe Soothing Gel, 20 oz refill pouches)
- Video 1 — ASMR Refill Duo: 3 required shots (Zig-Zag Frosting pour, Droplet Peaks, final beauty shot), audio direction, text hook
- Video 2 — Endless Summer Ritual: 4 opening hooks, 4-part talking point flow with suggested wording
- Final pre-submit checklist

## How to add / change images anywhere in the deck
Every image in the deck is a **named slot** that loads from `docs/img/`:

1. Open **`deck.html?edit`** — empty slots appear as dashed boxes labeled with the filename they expect (e.g. `img/v2-talkinghead.jpg`).
2. Drop your image into `docs/img/` with that exact name (`.jpg`, `.jpeg`, `.png`, or `.webp` all work).
3. Commit + push — the slot fills automatically. To **replace** an existing image, overwrite its file in `docs/img/`.

Empty slots are invisible to creators in normal view — only `?edit` reveals them.

Current slots: `cover`, `product-scrub`, `product-aloe`, `v1-shot1-main`, `v1-shot1-alt`, `v1-shot2-main`, `v1-shot2-alt`, `v1-shot3-main`, `v1-shot3-alt` (empty), `v1-audio` (empty), `v2-hero`, `v2-talkinghead` (empty), `v2-scrub`, `v2-aloe`, `v2-refill`.

To add a **brand-new slot** anywhere, insert `<div class="imgslot" data-img="my-slot-name" style="flex:1;min-height:120px"></div>` in `deck.html` and drop `docs/img/my-slot-name.jpg`.

## Structure
- `docs/deck.html` — the 15-slide presentation deck (reveal.js, vendored offline)
- `docs/img/` — product & texture stills (image slots)
- `docs/vendor/` — reveal.js core (self-contained, no CDN)
- `docs/index.html`, `docs/deck-v1.html` — previous campaign version, kept for reference

Static site, no build step. GitHub Pages serves from `main` / `docs`.
