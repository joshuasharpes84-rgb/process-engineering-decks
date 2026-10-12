# Heat Exchanger Fouling

Fouling mechanisms (particulate, crystallization, corrosion, chemical reaction), deposit-growth trends, and the Kern-Seaton rate model (Bott).

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/hx-fouling/
- **Download the .pptx (285 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Fouling-of-Heat-Exchangers.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 13

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Heat Exchanger Fouling
- Joshua Sharpes

### Slide 2: Sources
- Fouling of Heat Exchangers (T.R. Bott)

### Slide 3: Contents
- Background
- Fouling Types (particulate, crystallization, corrosion, etc.)
- Fouling Trends
- Fouling Rates

### Slide 4: Fouling Background
- Fouling: the buildup of material on surfaces that reduces effective conductivity & heat transfer
- Significant source of downtime in exchangers
  - Some exchangers need to be cleaned daily
  - Some operations require exchangers in parallel for alternating use
- The problem is that fouling is not well understood
  - Fouling Factors (R, quantification of material buildup) are per service; they do not describe individual mechanisms (types)
  - Data is needed for specific types of fouling within a service  requires research ($)
    - Still very difficult to distinguish types
  - Fouling is hard to model because multiple mechanisms occur at once, at a very slow rate, due to very minimal presence of material, all internally to exchanger that has multiple process streams
- This presentation aims to showcase most up-to-date understanding of Fouling

### Slide 5: Fouling: Best Approach (Type-independent)
- Prevent fouling by having clean upstream service
  - Adequate separation processes designed to dispose of particulate matter (salts, suspended solids)
    - Filters, membranes, cyclones, centrifuges, etc.  See Peters Textbook
  - Reaction processes designed to eliminate byproduct formation
    - Catalyst bed attrition can also lead to particulate  Guard beds, feed stock monitoring will prevent this.
- Mitigate fouling through adequate exchanger design & operation
  - Design: pinch-points, material of construction, uniform heat transfer/flow, appropriate sizing
    - Oversized exchanger loses MTD; problematic for steam heaters
  - Operation:  avoid abnormal temperatures (settling), hot/cold spots, significant time offline
- Monitor Fouling: Data (DCS) will show decreasing heat transfer coefficient
- Reset Fouling: Material additive (online) or cleaning (offline) techniques

> Speaker notes: Steam heaters will set temperature (pressure) below condensate return pressure, filling shell w/ liquid, leading to cycling and potential vacuum brake of outside (no condensable air)  Typically addressed w/ Pressure powered pump trap

### Slide 6: Fouling Types
- L
- bottom, low velocity
- L
- low-velocity zones
- U
- L
- hot end (inverse solubility)
- U
- L
- thickens toward cold end
- U
- pits: L
- U
- general corrosion
- U
- can plug in runaway
- L
- hot end / hot spots
- U
- macrofoulers: L
- U
- biofilm
- U = uniform, L = localized. Gray = tube wall; brown = deposit. Every drawing holds the same total deposit (same fouling allowance); only its distribution differs.

### Slide 7: Particulate
- What it is: deposition of suspended solids
  - Deposit layer buildup is correlated to concentration
  - Asymptotic layer buildup
- Prevention (Upstream): dissolved solids are usually abnormal, undesired byproduct
- Mitigations : avoidance of tight flow pockets (gasketed/welded plate exchangers),
  - Use exchangers w/ open channels

### Slide 8: Crystallization (Scaling)
- What it is:
  - Deposition of crystallized solids (see Crystallization Process Slide) controlled by concentration, temperature
  - Asymptotic layer buildup
- Prevention:
  - Upstream Process: intentional crystallization (through concentration change) to remove solids
  - HX Temp.: avoid solubility temperature transgression
- Mitigations are avoidance of tight flow pockets (gasketed/welded plate exchangers)
  - Use exchangers w/ open channels  Increases shear force on deposit

### Slide 9: Crystallization Process Explained
- Three Stages of Crystallization:
  - Supersaturation [8.3.1]. Depends on state variables:
    - Concentration: C > CS
    - Temperature: T < TS  ( Normal Solubility), T > TS  (Inverse Solubility)
  - Formation of nuclei [8.3.2]:
    - When state of supersaturation is achieved, individual nuclei form (primary nucleation) either through heterogenous (binds to surface) or homogenous (spontaneous)
      -  industrial exchangers are heterogenous (metal selection impacts crystallization)
    - Individual nuclei can also form on existing crystals (secondary nucleation) which is a form of heterogenous nucleation
  - Crystal Growth [8.3.3]:
    - Molecular weight increases, increasing heat capacity of deposited material, and thus resistance
      - Larger MW: greater thermal insulation and more resistance to shear force from flowing fluid (stickier)

### Slide 10: Corrosion
- Many different forms of corrosion exist which depend on service & operating conditions
  - See corrosion presentation
  - Corrosion tends to increase w/ temperature, acidity, and electric potential.
- What Corrosion is: dissolution of metal ions that results in oxide layer formed on metal.
  - Oxide layer does prevent further corrosion – passivation – but this is only beneficial for surfaces intended to insulate
- Prevention: material of construction is biggest lever
  - Removal of corrosion reactants (e.g. O2  for pitting) depend on corrosion mechanism

### Slide 11: Chemical Reaction
- Prevention: exchangers are typically not designed to encompass reaction; this phenomenon is abnormal and addressed w/ measures outside of exchanger design
- Mitigation: runaway reaction can quickly foul exchanger which could itself be used in service to control runaway; exchanger should be designed/configured for such scenario
- Hazard Evaluation Procedure implementation is required for this fouling type
  - See HEP Presentation

### Slide 12: Fouling Trends
- Rate of deposit buildup is classified as either:
- Asymptotic
  - Deposit layer thickness reaches limitation
- Linear
  - Applies for fast deposition scenario (runaway reaction) where shear forces don’t act fast enough
- Falling Rate
  - Most common, a medium of the two above trends, where rate never levels off in approach to allowable thickness.
  - Falling rate is the result resulting (often) from a combination of fouling mechanisms
- Whether a system is classified as Linear or Falling depends on cleaning rate
  - Left untouched, a falling rate system will eventually show asymptotic behavior
  - If cleaning cycle (from fouling threshold) is frequent enough, all trends will show linear behavior

### Slide 13: Fouling Rates
- Kern-Seaton asymptotic model (1959)
  - Rf(t) = Rf* · (1 − e−t/τ)
  - Rf(t) approaches an asymptotic value Rf* with time constant τ, as deposition (proportional to bulk velocity and solution concentration) is balanced by removal (based on wall shearstress and deposit strength). This is a mathematical framework/ansatz, not itself a source of numbers — it still needs a mechanism-specific deposition/removal rate model pluggedin (e.g. Ebert-Panchal, below) to produce an actual Rf* or τ.
- Falling Rate is very case-specific, data needed. One estimation is
  - Ebert-Panchal threshold fouling model (1995) — crude oil / chemical-reaction fouling only
