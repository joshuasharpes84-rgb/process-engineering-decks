# Shell and Tube Exchanger Design Heuristics

Temperature crossover, pass configuration, and shell-side vs tube-side assignment rules.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/hx-heuristics/
- **Download the .pptx (0 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Heat-Exchanger-Heuristics.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 4

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Shell-and-Tube Exchanger Design Heuristics
- Joshua Sharpes

### Slide 2: Temperature Crossover (TC)
- For singular exchanger, can be addressed primarily through three approaches:
  - 1 Tube Pass, 1 Shell Pass Design: this design (this is usually first approach) is TC-proof but prone to velocity or pressure deviations
    - Tube length can only be increased so much before vibration, maldistribution, maintenance accessibility, and shell-side pressure drop become problematic
  - Shell in Series: slightly more prone to TC. Potential pressure drop and vibration issues on shell side
  - Split-Shell Flow: Most prone to TC.
- Next approach is to re-evaluate exchanger selection with potential need for multiple exchangers.
- Note that TC extent is usually quantified through LMTD correct factors, Ft:
  - FT  < 0.7  Near TC
  - FT  = undefined  TC

### Slide 3: TEMA Configuration Hierarchy
- From best to worst (shell-tube passes):
  - 1-1
  - 1-2
  - 2-4
  - 3-6
  - 4-8
- Why are 2-2, 4-4 not TEMA arrangements?
  - Shell partitions take up exchanger volume
  - Heat Transfer: Less lateral shell flow
- Best to increase tube passes

### Slide 4: S/T Allocation (includes Condensation)
- Biggest Considerations (in order of Priority):
  - Corrosion: more corrosive material  tubes. Much easier to replace a bundle
  - Fouling (Particulate): dirtier material  tubes. Much easier to clean tubes
    - Condensation w/ severe fouling:
      - Particulate: tube-side, orientation depending mixture composition
      - Liquid-Film: shell-side, horizontal
  - Pressure Drop: lower pressure drop required  Tubes
  - Pressure: Higher Pressure  Tubes
  - Temperature: Higher Temperature  Tubes
  - Viscosity: Higher Viscosity  Shell
  - Flow Rate: Higher Flow Rate  Shell
- Source: Coulson/Richardson
