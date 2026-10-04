# Battle Field — Generative Art

> A seed-based generative system for two-force compositions.  
> A reproducible catalogue of computational textile compositions.

---

## What is this?

**Battle Field** is a generative design system that stages a conflict between two colour-forces — yellow and black — across a grid, a wavefront, or concentric rings. Where the two sides meet, the field resolves: a composition that is neither fully planned nor fully random, but **emergent**.

Every artwork in this catalogue is defined by a single numeric seed. The same seed always produces the identical composition — making each piece **traceable, reproducible, and licensable** across textile, print, and apparel applications.

Named for the ground on which opposing forces meet — the field that decides which side holds — **Battle Field** translates that idea into code.

---

## Live

🌐 **[View the catalogue →](https://reyrove.github.io/Battle-Field-Generative-Art/)**

---

## The System

The generator combines two forces:

| Force | Description |
|-------|-------------|
| **Yellow** | Bright, high-saturation bands in the hue range 50–70. |
| **Black** | Deep, low-brightness bands in the hue range 220–260. |

Both forces are driven by the same seed, ensuring deterministic output.

### Parameters

- **Battle intensity** — 0 to 1, drives grid density and noise flips
- **Grid size** — 15 × 15 up to 30 × 30 cells
- **Pattern type** — checkerboard, wavefront, or concentric rings
- **Colour palette** — HSB, randomized per seed

---

## Structure

```
Battle-Field-Generative-Art/
├── index.html          ← Full catalogue (single-file)
├── images/
│   ├── fav.svg
│   ├── tote.png
│   ├── tee.png
│   └── cushion.png
└── README.md
```

The entire project is contained in a single `index.html` — no build step, no framework. Open it in any modern browser.

---

## Features

- **Seed-based generation** — every composition is deterministic and reproducible
- **Live catalogue** — cover, plate, surfaces, process, archive, commission sections
- **Multiple surfaces** — print, scarf, textile, wallpaper — all rendered from the same seed
- **Archive of 8 seeds** — click any plate to load it into the main view
- **PNG export** — download any composition directly from the browser
- **Keyboard shortcuts** — `R` for new seed, `S` to save
- **Legal modal** — licensing, terms, and credits built in
- **Responsive** — works on desktop, tablet, and mobile
- **Mobile-first navbar** — horizontally scrollable with fade hint

---

## Usage

### Generate a new composition

Click **New Seed** or press `R`.

### Download the current composition

Click **Download** or press `S`.

### Load a seed from the archive

Click any plate in the **Archive** section.

---

## Colour System

Each seed selects one of three battle formations:

- **Checkerboard** — alternating cells with a noise-driven front line
- **Wavefront** — a sine-wave boundary with distance-based colour mixing
- **Concentric** — rings of alternating forces with damage-jittered thickness

Each formation resolves the same two forces on different geometry. No two seeds share the same field.

---

## Technical Notes

- p5.js 1.9.0 (CDN) for canvas rendering
- Custom seeded random generator for deterministic output
- `noiseSeed()` reset per tile so repeats agree
- HSB colour mode, per-instance
- Rectangular surfaces tile the square composition to fill aspect ratio

---

## About

**Battle Field** is a project by [Reyhaneh Daneshdoost](https://reyrove.github.io/) — an Iranian-born artist working at the intersection of classical textile logic and generative systems.

The work begins with a simple observation: the woven surface — repetitive, mathematically structured, infinitely variable — has always been a form of computation, long before computers.

**Battle Field** is an attempt to render that logic visible.

> *Two colours meet on a grid — and the grid decides who wins.*

---

## Licensing

All compositions are seed-documented and available for licensing across textile, surface, and apparel applications.

For commercial use, custom editions, or exclusive rights:

📧 **reyhanehdaneshdoost@gmail.com**

See the **Licensing** section in the live catalogue for details.

---

## Links

- 🌐 [Website](https://reyrove.github.io/)
- 📷 [Instagram](https://www.instagram.com/rey._.rove/)
- 💼 [LinkedIn](https://www.linkedin.com/in/reyhaneh-daneshdoost-730481160/)
- 🐦 [X](https://x.com/reyrove)

---

## Credits

**Design & Generative System**  
Reyhaneh Daneshdoost

**Typefaces**  
Cormorant Garamond · DM Mono

**Edition**  
Battle Field — Autumn 2026

---

<p align="center">
  <em>Computational Textile Design</em><br />
  <sub>© Reyrove Studio · All compositions reproducible by seed</sub>
</p>