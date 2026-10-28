# Absorber Heuristics

Trayed vs packed selection, flooding correlations, distributors, Kremser, Edmister, HTU/NTU.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/absorber-heuristics/
- **Download the .pptx (474 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Absorber-Heuristics.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 47

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Absorber Selection, Design, and Performance Evaluation
- Joshua Sharpes

### Slide 2: References
- Ludwig, Process Design for Chemical and Petrochemical Plants, Volume 2
- Perry’s Handbook 9th Edition
- Rules of Thumb for Chemical Engineers
- ◂ Contents   ·   #

### Slide 3: Contents
- Absorber and Packing Selection
- Packing Hydraulics
- Tower Internals: Distribution and Support
- Design and Evaluation Methods
- Appendix: Mass-Transfer Correlation References
- ◂ Contents   ·   #

> Speaker notes: Draft contents outline (moved from slide body):
Absorption Applications (link to other presentation)
Trayed vs Packed Towers (Table 11, ch 6 seader seps, 
Pressure Drop estimations (fig 12/13)
Liquid Loading (Table 6)
Packing Type Selection
Distributor Selection (14-71)
HETP Calculation and Estimation
Design and Performance Evaluation Methods
Kremser
Edmister
Tower Retrofits (table 12 and fig 23)

### Slide 4: Absorber and Packing Selection
- Absorption Applications
- Solvent Selection
- Tower Internal Purposes
- Low Liquid Rates: Trays vs Structured Packing (rules of thumb)
- Packing: Structured vs Random Rules of Thumb
- Internals Selection Map: Flow Parameter Spectrum
- Performance Characterization of Trays and Packing
- Random Packing Size Selection
- Navigating Packing Charts: Structured Packing
- Retrofitting Costs and Installation Methods
- ◂ Contents   ·   Absorber and Packing Selection   ·   #
- Back to Table of Contents

### Slide 5: Absorption Applications
- See prior Absorber Presentation for detailed selection guidance
- Absorber Types (from Cheremisinoff, Condensed Encyclopedia of Process Equipment):
  - Packed Towers (Wet Scrubbers)​:  numerous, these are most common type
  - Agitated Vessels​: batch reactors (HCl/ H2O and NH3/H2O)
  - Bubble-plate Towers​: SO2, HCl 
  - Cooler Absorbers​:  SO3, HCl, HF, and NO2
  - Spray Towers​: SO2, quench towers, odor control
  - Venturi Scrubbers​: extremely high affinity pairings
- Packed
- Trayed
- No Internals
- Bubble- Cap Tray Absorber
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 6: Solvent Selection
- Theoretically, high solute-solvent solubility would be default
  - However, lower solubility pairings may be desired due to downstream regeneration benefits:
    - OpEX for disposing/regenerating solvent >> CapEX absorber
- Typically, high solubility is desired when:
  - Heat of absorption (per mass) is low  Feasible Temperature Control
  - Rich Solvent requires no separation (waste)  Reduces OpEX
  - Corrosion-resistant alloy (CRA) is required  Reduces CapEX
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 7: Tower Internal Purposes
- Internals increase contact surface area which increases absorption per volume  Greater efficiency
- Generally, increasing specific area is unnecessary for
    - high affinity solute-solvent pairings
    - Low absorption demands
  - …and is undesirable for high ∆Habs (best to use vessel with internal coils/jacket)
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 8: Low Liquid Rates: Trays vs Structured Packing (rules of thumb)
- Roughly 2/3 of absorbers have FP  < 0.1
- Most gases are very lean
- Trays are prone to:
- Foaming
- Entrainment
- Higher Pressure Drop
- Structured Packing is prone to:
- Plugging from scaling
- Corrosion (higher surface area and more pinch points)
- This diagram should be used for both new and exiting towers with potential retrofit in mind
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 9: Packing: Structured vs Random Rules of Thumb
- Structured Packing (Table 14-14) is better for:
  - Larger towers: Diameter >3ft
  - Lower Liquid Rates: 0.02 < Fp < 0.3
  - Lower pressure drop requirement
- Random Packing (Table 14-13) is better for:
  - Small Towers : Diameter <3ft
  - Higher Liquid Rates: 0.3 < Fp < 0.5
  - Higher pressure drop tolerances (typically high-pressure process)
- **For Fp  < 0.02  Consider Bubble-Cap Tower
- These heuristics are under the assumption of adequate liquid distribution and non-restrictive internals
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 10: Internals Selection Map: Flow Parameter (FP) Spectrum
- ◂ Contents   ·   Absorber and Packing Selection   ·   #
- From prior slide:

> Speaker notes: Sources: Kister et al., Chem. Eng. Progr. 90(2):23 (1994), via Perry's 9th p.14-78 and Rules of Thumb pp.92-93 (trays, random and structured packing compared, optimized distillation designs, F_P 0.02-0.5). Perry's 9th Table 14-5 and pp.14-26/27 (sieve, fixed valve, moving valve), p.14-32 (bubble caps: very low gas and liquid rates), p.14-77/78 (trays beat random packing at low liquid rates, not structured; multipass for high liquid rates). TEG contactor: this unit 0.0066; GPSA Ex 20-11 approx. 0.008. Grouped graphic: drag a corner to scale; click into the group to edit a cell.

### Slide 11: Performance Characterization of Trays and Packing
- Material Legend:
- M = Metal, C = Ceramic, P = Plastic
- Performance Hierarchy:
- S. Packing > R. Packing > Trays
- Affordability Hierarchy:
- Trays > R. Packing > S. Packing
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 12: Random Packing Size Selection Heuristic
- Packing Size is dependent on tower diameter.
- Smaller packing is more efficient, but carries higher pressure drop
- Robbins Recommends that tower diameter should be at least 8x packing size
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 13: Navigating Packing Charts: Structured Packing
- Size or Number:
- Number corresponds to surface area
  - 350Y  ap = 350 m2/m3
- Letter Corresponds to corrugation angle:
  - Y-type: 45̊
    - Denser, higher pressure drop
  - X-type: 60̊
    - More porous, lower pressure drop
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 14: Retrofitting Costs and Installation Methods
- Example: A 30ft tower with  tray  packing swap would cost about $50k
- Not shown are factors for labor, packing spacing, and removal.
- Installation of Packing Material:
- Structured Packing is much more expensive as material
  - needs to be stacked by hand
- Random Packing is dumped into bed onto support, preferably with the use of a metal cone for more dense dispersion.
- ◂ Contents   ·   Absorber and Packing Selection   ·   #

### Slide 15: Absorber, Packing Selection Workflow
- Finalize Rich Gas Feed Conditions
- Select Solvent
- Determine ∆Habsorption , Fouling, Foaming, and Corrosion Potential
- Select Material of Construction
- Select Absorber Type

### Slide 16: Packing Hydraulics
- Packing Checklist
- Liquid Wetting Rates: Min & Max
- Absorber Operation → Ensure Selected Packing is Appropriate
- Why we typically operate within 60-80% of loading range…
- Allowable Pressure Drop: Random Packing
- Predicting Flood Point with Pressure Drop (1st method)
- Predicting Flood Point with Pressure Drop (2nd method)
- Packing Factors FP
- ◂ Contents   ·   Packing Hydraulics   ·   #
- Back to Table of Contents

### Slide 17: Packing Checklist
- Ensure following heuristics, shown in upcoming slides, are met:
  - Liquid Loading is between Minimum (MWR) and Maximum
  - Operating Range is established  Efficiency ensured
  - Pressure Drop is kept low enough
  - Packing height achieves required separation: connect with EQ and Rate Methods
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 18: Liquid Wetting Rates: Min & Max
- Maximum is dependent on packing size:
- Minimum is dependent on packing specific area, at:
  - Newer model incorporates surface material (use this if material of construction is listed):
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 19: Absorber Operation  Ensure Selected Packing is Appropriate
- Loading Point: lower dP vs Gas rate inflection point where gas begins to restrict liquid flow
- Flood Point: upper dP vs Gas rate inflection point where gas entrains liquid flow
- Loading Range is between loading and flood points
  - Incipient Flood Point: Gas rate where liquid flow becomes unstable
- Operating Ranges are usually kept
  - …To ensure pressure drop is lower than predetermined value which is dependent on service (next slide)
  - …Between 60-80% of loading range
- Incipient flood point within these loading ranges – indicated by “x”
- Pressure drop of 0.4 (in/ft) usually corresponds to Incipient flooding point
- Capacity Factor vs Flow Parameter Graph
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 20: Why we typically operate within 60-80% of loading range…
- Flow Parameter, X
- From previous slide:
- Capacity Factor, Cs
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 21: Allowable Pressure Drop: Random Packing
- Random Packing
  - For Standard Distillation, Allowable pressure drop is largely dependent on operating Pressure:
    - Medium Pressure: 0.40 – 0.60 in/ft
    - Higher Pressure: 1.5 – 2.0 in/ft
  - For Absorption, Allowable Pressure Drops Are Lower:
    - 0.1 – 0.4 in/ft for non-foaming systems
    - 0.25 – 0.4 in/ft for moderate foaming systems
- Structured Packing:
  - Absorption:
    - 0.3-0.5 in/ft, regardless of foaming
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 22: Predicting Flood Point with Pressure Drop (1st method)
- To determine the actual pressure drop, select constants from table:
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 23: Predicting Flood Point with Pressure Drop (2nd method)
  - In addition to the heuristics, following correlations should be used:
    - Pressure drop that usually results in flooding:
    - Gas Flow Rate  that usually results in flooding:
      - Sherwood-type Correlation for Gas Flow Rate 
- Despite identical notation, Packing Factor ≠ Flow Parameter
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 24: Packing Factors FP
- These quantify capacity and pressure drop of packing: lower is better
- These can be found through either charts (predetermined by vendor, Table 9-26) or through characteristic equations:
- Effective surface area of packing increases with settling and breakage during operation:
- As much as 70% for ceramic materials
- at  is the initial, manufactured surface area of the material
- ◂ Contents   ·   Packing Hydraulics   ·   #

### Slide 25: Tower Internals: Distribution and Support
- Liquid Distribution
- Liquid Distributor Heuristics
- Liquid Distributors: Drip Points
- Liquid Distributor Types
- Liquid Distributor Type Selection
- Liquid Collectors
- Support Plates
- Pressure Drop Across Packing Supports and Redistribution Plates
- Redistribution Heuristics
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #
- Back to Table of Contents

### Slide 26: Liquid Distribution
- A tower is not just packing/trays, devices are needed to ensure necessary irrigation of liquid throughout these contacting volumes:
  - Liquid Distributors: most important device in tower, required for any external liquid stream introduction
  - Liquid Collection Devices: necessary for change in tower diameter; rectifying section is often smaller than stripping section
  - Liquid Re-distributors: required for any separate section of packing
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 27: Liquid Distributor Heuristics
- Liquid Distributors directly impact the efficiency of the packing
  - Poor distribution leads to flow maldistribution throughout tower
  - Maldistribution increases with bed depth as liquid begins to flow down tower walls
- Flow uniformity is much more important than number of distribution points (Drip Points)
- Void space between distributor and packing should be no greater than 12 inches  reduce impact of falling liquid
  - 18-36 inches for spray nozzles in vacuum applications
- Distributor performance drops due to fouling, vapor presence, etc:
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 28: Liquid Distributors: Drip Points
- More drip points are required for Smaller Packing (component pieces) and Lower Liquid Load
- Despite maldistribution tendencies, drip point concentration should be uniform even near tower wall
- Vapor velocity should be kept low to avoid distributor entrainment:
              - Cf < 0.4 ft/sec
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 29: Liquid Distributor Types
- Pan Distributors (PAN): Riser tube distributors consisting of flat tray with equally spaced orifices; top and bottom
  - Best for clean liquids in towers 2-10 ft diameter of variable liquid rates
  - Prone to plugging, undesirable for high vapor rates
- Pipe Orifice Header (POH): piping network with orifice holes
  - Gravity Fed: Very good distribution
  - Pressure Driven: Ideal for heat transfer
  - Both types (gravity/pressure) are bad with large liquid rates
- Trough Distributors (NTD): utilizes overfilling, adjacent boxes (troughs) to irrigate liquid
  - Best for low to medium liquid rates
  - Lacks widespread distribution to tower walls
  - V-Notch Distributors (VND): uses V-shaped notches in place of holes to prevent solids blockage
- Spray Nozzle Headers (SNH): POH but with downward facing nozzles
  - Great for heat transfer
  - Poor for high separation demands; misting increasing entrainment
- PAN Distributor
- Pipe Orifice Header
- Spray Nozzle Header
- NTD: VND^
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 30: Liquid Distributor Type Selection
- PAN: Pan
- POH: Pipe Orifice Header
- NTD: Notched Trough
- SNH: Steam Nozzle
- VND: V-Notch Trough
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 31: Liquid Collectors
- 3 main types:
  - Deck: tight liquid seal but high pressure drop
  - Trough: moderate in both pressure drop and leakage, limited to larger towers
  - Vane: best used for vacuum applications, prone to leaks
- Collectors are not dependent on liquid rates
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 32: Support Plates
- These suspend the packing beds in the tower
  - Weight is a function of packing, liquid volume, and operating pressure surge
    - Weight can limit the bed height (usually limited by flow maldistribution)
- These perforated plates can be flat or have risers:
  - Risers are better for higher vapor and liquid rates; lower pressure drop
  - Plates be designed to not bottleneck packing capacity (vapor & liquid)
  - Pressure drop due to packing congestion in plate risers can be significant
- Larger Diameter towers often require support grids underneath these plates
- Risers 
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 33: Pressure Drop Across Packing Supports and Redistribution Plates
- Saddle packing is more prone to blockage than ring packing
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 34: Redistribution Heuristics
- Ideally, a single bed could be used throughout the height of the tower
  - Unfortunately, maldistribution is correlated with increasing bed depth, requiring collections and redistribution.
  - Liquid migrates towards tower walls as it flows down packing, especially prominent near entrance of vapor
- Redistribution Heights (Allowable Packing Heights):
  - Raschig Rings: 3 Tower Diameters
    - Typical Max Packing Bed Height: 15 ft
    - Estimated 20% of liquid is on walls at 10ft depth
  - Saddle Packings: 5-10 Tower Diameters
    - Typical Max Packing Bed Height: 20 ft
- ◂ Contents   ·   Tower Internals: Distribution and Support   ·   #

### Slide 35: Design and Evaluation Methods
- Absorption Feasibility Analysis
- Design/Evaluation Methods (Most Used)
- Selection of Design/Evaluation Method
- Method Classifications
- Performance Evaluation: HTU/NTU
- Gas and Liquid Diffusivities
- Design: HTU/NTU Method
- Performance Evaluation: Kremser Method – Steps
- Performance Evaluation: Edmister Method - Steps
- Performance Evaluation: HTU/NTU Method
- Kremser Method: Design
- ◂ Contents   ·   Design and Evaluation Methods   ·   #
- Back to Table of Contents

### Slide 36: Absorption Feasibility Analysis
- Perry’s section 14 mentions graphical method using operating lines and equilibrium data
  - Necessary for HTU/NTU
  - Recommended for EQ Methods
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 37: Design/Evaluation Methods (Most Used)
- Equilibrium Methods (EQ)
  - Kremser Method
    - Assumes no heat of absorption; applicable for lean gases (<10 mol%)
      - Often used for hydrocarbon and natural gas applications
  - Edmister Method
    - Incorporates impure solvents and entrainment of lean oil, best for rich gas
      - Also used for hydrocarbon systems
  - Each EQ Method can be used to:
    - Evaluate existing tower (Performance Evaluation)
      - Use number of trays to determine absorption
    - Size a new tower (Design)
      - Use absorption target to determine number of trays
- Rate-Based Methods: HTU/NTU Method
  - Applicable for all gas concentrations
  - Used for Performance Evaluation and Design
- All of these are shortcut methods
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 38: Selection of Design/Evaluation Method
- For hydrocarbons, choice of Kremser/Edmister comes down to heat of absorption significance which is correlated, although not defined, by the concentration of absorbate.
  - For optimization of multi-component hydrocarbon systems, the Smith-Brinkley method should be considered
- For inorganic species, HTU/NTU method is best.
- Method selection is independent of design vs performance evaluation intentions; the same equations are used, just rearranged
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 39: Method Classifications
- Kremser, Edmister, and HTU/NTU methods are undoubtably the most popular for absorption applications  these are all shortcut methods
- Methods are classified according to their mathematical rigor and their equilibrium convergence
  | MODEL EXAMPLES | Equilibrium  (ideal thermodynamics) | Rate-Based (non-ideal thermodynamics that account for mass transfer resistances |
  | Shortcut  (incomplete math) | Kremser, Edmister | HTU/NTU |
  | Rigorous (complete stage-by-stage math) | MESH, RadFrac | Maxwell-Stefan Rate Models |
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 40: Performance Evaluation: HTU/NTU
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 41: Gas and Liquid Diffusivities
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 42: Design: HTU/NTU Method
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 43: Performance Evaluation: Kremser Method – Steps
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 44: Performance Evaluation: Edmister Method - Steps
- Steps
- Assume theoretical stages, operating temperature and pressure
- For required component recovery, get absorption factor from figure 
- Select initial moles absorbed, temperature rise of lean oil, and lean oil rate
- Establish tower material balance from table 1
- Calculate liquid/vapor ratios at top and bottom
- Estimate top/bottom temperatures from table 2
- Obtain top/bottom K values
- Calculate absorption factors for each component at top/bottom
- Calculate absorption factors for each component (overall)
- Get fraction absorbed for each component from figure
- Calculate moles of each component absorbed
- Compare this result to assumed total moles absorbed (step 3), adjusting oil rate as needed
- Legend: Select value, extract value, calculate value
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 45: Performance Evaluation: HTU/NTU Method
- Mass balance around Initial section in terms of vapor concentration
  - gas compositions are easier to measure - gas chromatography, infrared (IR), non flashing, uniform composition, etc.
- HOG : physical efficiency of the packing
- NOG : difficulty of the separation
- Vapor flow rate (V) is a function of tower diameter
- Z: packing height required to achieve separation
- ◂ Contents   ·   Design and Evaluation Methods   ·   #
- Correlation choice at high pressure (TEG contactor, 70 bar):
- Onda a_w (Perry's Table 5-24-C) is the default: within ~20% of Perry's HETP rule
- Bravo–Fair is invalid here: a_e exceeds a_p
- Check every model height against Perry's HETP rule

> Speaker notes: Sources (added 2026-10-26): Perry's 8th Table 5-24-C (Onda) and 5-24-D (Bravo-Fair); Perry's 9th Sec 14 HETP rules Eqs 14-156, 14-159, 14-161 (glycol x1.5, Strigle lambda). At 70 bar the Bravo-Fair effective area exceeds the dry area (a_e/a_p > 1), so it is out of range; Onda's wetted area lands within ~20% of Perry's rule. Detail: Glycol Dehydrator\Contactor Sizing\Contactor Sizing - Findings.md.

### Slide 46: Kremser Method: Design
- ◂ Contents   ·   Design and Evaluation Methods   ·   #

### Slide 47: References
- Mass Transfer Coefficient Correlations
  - Structured Packing:
    - Bravo, Fair, and Rocha correlation [Chem. Eng. Progr. 86(1), 19 (1990); Ind. Eng. Chem. Res. 35, 1660 (1996)]
    - https://pubs.acs.org/doi/pdf/10.1021/ie00016a010?ref=article_openPDF
  - Random Packing:
    - Bravo and Fair correlation [Ind. Eng. Chem. Proc. Des. Dev. 21, 162 (1982)]
    - Invalid at high pressure (a_e > a_p at 70 bar); Onda a_w is the default
  - Perry’s Table 5-24 provides correlations:
    - Sherwood/Holloway (Random), Onda (Random), Reiss (Random), etc.
- Applied Process Design, Volume 2 (Ludwig)
- ◂ Contents   ·   Appendix: Mass-Transfer Correlation References   ·   #
- Tray efficiency (bubble cap): AIChE Bubble Tray Design Manual, Perry's 9th Eqs 13-72 to 13-78, then Eqs 14-137 and 14-135; O'Connell (Fig 14-9) is off chart for TEG
- Maldistribution: Moore & Rukovena (Perry's Fig 14-63); Lockett & Billingham f_max (Eq 14-162)
- Back to Table of Contents

> Speaker notes: Sources (added 2026-10-26): Perry's 9th Sec 13 pp.13-38 to 13-39 (AIChE N_V, N_L), Sec 14 p.14-47 (Eqs 14-135 to 14-137), Fig 14-9 (O'Connell); GPSA Sec 20 (tray efficiency 25-30%); Kean, Turner & Price, Oil & Gas J. Sept 23 1991 (25%, some operators 33%). Perry's 9th pp.14-66 to 14-68 (Moore & Rukovena Fig 14-63; Lockett & Billingham Eq 14-162 and f_max guidelines).
