# Vertical Gas-Liquid Separators

Souders-Brown sizing, height heuristics, residence time, mist extractor, and control loops.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/vgl-separators/
- **Download the .pptx (95 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Vertical-Gas-Liquid-Separators.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 5

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Vertical Gas-Liquid Separator Design
- Joshua Sharpes
- *Also referred to as KO Pots, two-phase separators

### Slide 2: Design Considerations
- Purpose of the vessel is to separate vapors from liquids
  - Used to purge non-condensables, dry compressor feed
  - No heat exchanger or throttle used
- Impingement devices knockdown liquids from vapors 
  - This reduces required vessel volume as
    - Reduces vapor-liquid mixing
    - Liquid will coalesce on this devices surface that is binding site for entrained droplets
- Mist Extractors (demister) knockdown entrained droplets from vapor effluent 

### Slide 3: Vessel Diameter: Max Vapor Velocity Using Souders-Brown to Prevent Entrainment
- The greater the difference in vapor/liquid densities the easier the separation.
- K is between 0.15 and 0.25 ft/s.
  - This value decreases with higher pressures.
- Must ensure that Vmax is not exceeded in the overhead piping.

### Slide 4: Vessel Height
- Evaluations:
  - Baseline Heuristic: Height = 4 x Diameter
  - Adequate Liquid Residence Time for Separation:
    - 1–3 minutes for clean, low‑viscosity hydrocarbon service
    - 3–5 minutes for moderate viscosity or mildly foaming service
    - 5–10 minutes for high viscosity, dirty, or foaming liquids
    - ≥10 minutes where slug handling or unstable liquid flow is expected
  - Adequate Liquid Residence Time for Proper Level Control – next slide
- Significant discrepancy of 2 or 3 from 1 requires reiteration of the diameter

### Slide 5: Control Schemes
- PIC is used to control vapor effluent
  - Valve type should not be sensitive to liquid entrainment
- LIC is used to control liquid effluent
- These two control schemes are competing and should
  - be independent of each other
  - have similar integral times
