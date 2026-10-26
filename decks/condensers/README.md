# Condensers

Film vs dropwise condensation, non-condensables, and design heuristics.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/condensers/
- **Download the .pptx (101 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Condensers.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 5

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Condensers
- Joshua Sharpes
- Source: Cheremisinoff, N.P., Chemical Engineer’s Condensed Encyclopedia of Process Equipment (Gulf, 2000)

### Slide 2: Condenser Types
  |  | Fluid Mixing | Equipment Examples | Efficiency | Condensate Re-use | Subcooling |
  | Surface Condenser | None | S&T Exchanger | Low | Possible | Possible with two outlet nozzles |
  | Contact Condenser | Complete mixing | Cooling Towers, spray chambers, venturi liquid jet eductor* | High | Impossible (Contaminated) | Requires greater heat load as heating is much more uniform |
- *also an absorber

### Slide 3: Condensation Mechanisms: Film vs Drop-wise
- Due to differences in surface energy and hydrophobicity of substances, two different mechanisms with drastically different heat transfer coefficients are apparent:
  - Film-wise Condensation occurs when liquid condensate film builds up on heat transfer surface which insulates that bare metal and saturated vapor
    - High surface energy, hydrophilic substances
  - Drop-wise Condensation occurs when liquid condensate drops off surface in time to avoid this film buildup, allowing for direct contact of bare metal and saturated vapor.
    - Low surface energy, hydrophobic substances
- As expected, Ufilm < Udrop, but most industrial applications are film wise due to capacity trade-off.
  - Dropwise heat transfer coefficients are anywhere from 5-10 times greater
  - Steam is one of the only drop-wise applications
- Sometimes, additives such as oleic acid are charged to promote drop-wise behavior, but this results in contamination of condensate.

### Slide 4: Condensation Heat Transfer Trends
- Ideally, Q=U*A*Tlm  could be used, but condensation is often more complex due to the buildup of liquid films and the necessary diffusion through accumulating non-condensable vapors
  - Heat transfer coefficients expectantly go down with increasing film thickness but there is a moderate reversal of this trend due to turbulence in the expanding liquid film (Ctrl + “+: to zoom):
  - Larger sensible heat loads are required for the presence of non-condensables to achieve same dT:

### Slide 5: Condenser Design Heuristics
- Effective contact condensers will reach equilibrium temperature (modeled as single-stage, 100% efficient)
- Dilute material condensation can be considered isothermal
  - Low temperature range also justifies isothermal assumption
- Condensation volume reduction is assumed to be isobaric
- Pressure drop of vapor in low pressure operation increases heat load (PSAT = f(T); harder to condense a lower pressure vapor)
- Steam under vacuum (low ρ) increases velocity in tubes
- Non-condensables can reduce U by as much as 50%
  - Dissolved gas in cooling water (jet condensers), steam or vapor entrainment, leaks
- Horizontal condensers have better vapor distribution and condensate disposal
  - Liquid pools must be prevented
- S/T allocation is dependent on fouling, corrosivity, and performance
  - Condensation coefficients are higher on shell side (increased film thickness in tubes, lower coolant velocity in shell)
