# Absorber Heuristics

Trayed vs packed selection, flooding correlations, distributors, Kremser, Edmister, HTU/NTU.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/absorber-heuristics/
- **Download the .pptx (459 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Absorber-Heuristics.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 40

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Absorber Selection, Design, and Performance Evaluation
- Joshua Sharpes

### Slide 2: References
- Ludwig, Process Design for Chemical and Petrochemical Plants, Volume 2
- Perry’s Handbook 9th Edition
- Rules of Thumb for Chemical Engineers

### Slide 3: Contents
- Absorption Applications (link to other presentation)
- Trayed vs Packed Towers (Table 11, ch 6 seader seps,
  - Pressure Drop estimations (fig 12/13)
  - Liquid Loading (Table 6)
- Packing Type Selection
- Distributor Selection (14-71)
- HETP Calculation and Estimation
- Design and Performance Evaluation Methods
  - Kremser
  - Edmister
- Tower Retrofits (table 12 and fig 23)

### Slide 4: Absorption Applications
- See prior Presentation
- Main Applications:
  - Packed Towers (Wet Scrubbers)​:  numerous, these are most common type
  - Agitated Vessels​: batch reactors (HCl/ H2O and NH3/H2O)
  - Bubble-plate Towers​: SO2, HCl 
  - Cooler Absorbers​:  SO3, HCl, HF, and NO2
  - Spray Towers​: SO2, quench towers, odor control
  - Venturi Scrubbers​: extremely high affinity pairings
- Packed
- Trayed
- No Internals
- Tray Absorber

### Slide 5: Solvent Selection
- Theoretically, high solute-solvent solubility is desirable for every pairing
  - However, lower solubility pairings may be desired due to downstream regeneration benefits
    - OpEX for disposing/replacing solvent >> CapEX absorber
- Typically, high solubility is des

### Slide 6: Tower Internal Purposes
- Internals increase contact surface area which increase absorption per volume  Greater efficiency
- Generally, increasing specific area is unnecessary for
    - high affinity solute-solvent pairings
    - Low absorption demands
  - …and is undesirable for high ∆Habs (best to use vessel with internal coils/jacket)

### Slide 7: Trays vs Packing (rules of thumb)
- Most absorbers have Fp < 0.1 and are therefore packed
  - Exceptions include systems with high heat of absorption or scrubbing of highly volatile components – these require higher L
- Trays are prone to:
- Foaming
- Entrainment
- Higher Pressure Drop
- Packing is prone to:
- Plugging from scaling
- Corrosion (higher surface area and more pinch points)
- This diagram should be used for both new and exiting towers with potential retrofit in mind

### Slide 8: Packing: Structured vs Random Rules of Thumb
- Structured Packing (Table 14-14) is better for:
  - Larger towers: Diameter >3ft
  - Lower liquid holdup (Lower Liquid Rates: 0.02 < Fp < 0.3)
  - Lower pressure drop
- Random Packing (Table 14-13) is better for:
  - Small Towers : Diameter <3ft
  - Higher Liquid Holdup (Higher Liquid Rates: 0.3 < Fp < 0.5)
  - High pressure process
- These heuristics are under the assumption of adequate liquid distribution and non-restrictive internals

### Slide 9: Performance Characterization of Trays and Packing
- Material Legend:
- M = Metal, C = Ceramic, P = Plastic
- Performance Hierarchy:
- S. Packing > R. Packing > Trays
- Affordability Hierarchy:
- Trays > R. Packing > S. Packing

### Slide 10: Navigating Packing Charts: Structured Packing
- Size or Number:
- Number corresponds to surface area
  - 350Y  ap = 350 m2/m3
- Letter Corresponds to corrugation angle:
  - Y-type: 45̊
    - Denser, higher pressure drop
  - X-type: 60̊
    - More porous, lower pressure drop

### Slide 11: Packing Checklist
- Ensure following heuristics, shown in upcoming slides, are met:
  - Liquid Loading is between Minimum (MWR) and Maximum
  - Operating Range is established  Efficiency ensured
  - Pressure Drop is kept low enough
  - Packing height achieves required separation: connect with EQ and Rate Methods

### Slide 12: Liquid Wetting Rates: Min & Max
- Maximum is dependent on packing size:
- Minimum is dependent on packing specific area, at:
  - Newer model incorporates surface material:

### Slide 13: Absorber Operation  Ensure Selected Packing is Appropriate
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

### Slide 14: Why we typically operate within 60-80% of loading range…
- Flow Parameter, X
- From previous slide:
- Capacity Factor, Cs

### Slide 15: Allowable Pressure Drop: Random Packing
- For Standard Distillation (Random Packing), Allowable pressure drop is largely dependent on operating Pressure:
  - Medium Pressure: 0.40 – 0.60 in/ft
  - Higher Pressure: 1.5 – 2.0 in/ft
- For Absorption, Allowable Pressure Drops Are Lower:
  - 0.1 – 0.4 in/ft for non-foaming systems
  - 0.25 – 0.4 in/ft for moderate foaming systems
- Structured Packing:

### Slide 16: Predicting Flood Point with Pressure Drop (1st method)
- To determine the actual pressure drop, select constants from table:

### Slide 17: Predicting Flood Point with Pressure Drop (2nd method)
  - In addition to the heuristics, following correlations should be used:
    - Pressure drop that usually results in flooding:
    - Gas Flow Rate  that usually results in flooding:
      - Sherwood-type Correlation for Gas Flow Rate 
- Despite identical notation, Packing Factor ≠ Flow Parameter

### Slide 18: Packing Factors FP
- These quantify capacity and pressure drop of packing: lower is better
- These can be found through either charts (predetermined by vendor, Table 9-26) or through characteristic equations:
- Effective surface area of packing increases with settling and breakage during operation:
- As much as 70% for ceramic materials
- at  is the initial, manufactured surface area of the material

### Slide 19: Retrofitting Costs and Installation Methods
- Example: A 30ft tower with  tray  packing swap would cost about $50k
- Not shown are factors for labor, packing spacing, and removal.
- Installation of Packing Material:
- Structured Packing is much more expensive as material needs to be stacked by hand
- Random Packing is dumped into bed onto support, preferably with the use of a metal cone for more dense dispersion.

### Slide 20: Absorption Feasibility Analysis
- Perry’s section 14 mentions graphical method using operating lines and equilibrium data
  - Necessary for HTU/NTU
  - Recommended for EQ Methods

### Slide 21: Liquid Distribution
- A tower is not just packing/trays, devices are needed to ensure necessary irrigation of liquid throughout these contacting volumes:
  - Liquid Distributors: most important device in tower, required for any external liquid stream introduction
  - Liquid Collection Devices: necessary for change in tower diameter; rectifying section is often smaller than stripping section
  - Liquid Re-distributors: required for any separate section of packing

### Slide 22: Liquid Distributor Heuristics
- Liquid Distributors directly impact the efficiency of the packing
  - Poor distribution leads to flow maldistribution throughout tower
  - Maldistribution increases with bed depth as liquid begins to flow down tower walls
- Flow uniformity is much more important than number of distribution points (Drip Points)
- Void space between distributor and packing should be no greater than 12 inches  reduce impact of falling liquid
  - 18-36 inches for spray nozzles in vacuum applications
- Distributor performance drops due to fouling, vapor presence, etc:

### Slide 23: Liquid Distributors: Drip Points
- More drip points are required for Smaller Packing (component pieces) and Lower Liquid Load
- Despite maldistribution tendencies, drip point concentration should be uniform even near tower wall
- Vapor velocity should be kept low to avoid distributor entrainment:
              - Cf < 0.4 ft/sec

### Slide 24: Liquid Distributor Types
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

### Slide 25: Liquid Distributor Type Selection
- PAN: Pan
- POH: Pipe Orifice Header
- NTD: Notched Trough
- SNH: Steam Nozzle
- VND: V-Notch Trough

### Slide 26: Liquid Collectors
- 3 main types:
  - Deck: tight liquid seal but high pressure drop
  - Trough: moderate in both pressure drop and leakage, limited to larger towers
  - Vane: best used for vacuum applications, prone to leaks
- Collectors are not dependent on liquid rates

### Slide 27: Support Plates
- These suspend the packing beds in the tower
  - Weight is a function of packing, liquid volume, and operating pressure surge
    - Weight can limit the bed height (usually limited by flow maldistribution)
- These perforated plates can be flat or have risers:
  - Risers are better for higher vapor and liquid rates; lower pressure drop
  - Plates be designed to not bottleneck packing capacity (vapor & liquid)
  - Pressure drop due to packing congestion in plate risers can be significant
- Larger Diameter towers often require support grids underneath these plates
- Risers 

### Slide 28: Pressure Drop Across Packing Supports and Redistribution Plates
- Saddle packing is more prone to blockage than ring packing

### Slide 29: Redistribution Heuristics
- Ideally, a single bed could be used throughout the height of the tower
  - Unfortunately, maldistribution is correlated with increasing bed depth, requiring collections and redistribution.
  - Liquid migrates towards tower walls as it flows down packing, especially prominent near entrance of vapor
- Redistribution Heights (Allowable Packing Heights):
  - Raschig Rings: 3 Tower Diameters
    - Typical Max Packing Bed Height: 15 ft
    - Estimated 20% of liquid is on walls at 10ft depth
  - Saddle Packings: 5-10 Tower Diameters
    - Typical Max Packing Bed Height: 20 ft

### Slide 30: Design/Evaluation Methods (Most Used)
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

### Slide 31: Selection of Design/Evaluation Method
- For hydrocarbons, choice of Kremser/Edmister comes down to heat of absorption significance which is correlated, although not defined, by the concentration of absorbate.
  - For optimization of multi-component hydrocarbon systems, the Smith-Brinkley method should be considered
- For inorganic species, HTU/NTU method is best.
- Method selection is independent of design vs performance evaluation intentions; the same equations are used, just rearranged

### Slide 32: Method Classifications
- Kremser, Edmister, and HTU/NTU methods are undoubtably the most popular for absorption applications  these are all shortcut methods
- Methods are classified according to their mathematical rigor and their equilibrium convergence
  | MODEL EXAMPLES | Equilibrium  (ideal thermodynamics) | Rate-Based (non-ideal thermodynamics that account for mass transfer resistances |
  | Shortcut  (incomplete math) | Kremser, Edmister | HTU/NTU |
  | Rigorous (complete stage-by-stage math) | MESH, RadFrac | Maxwell-Stefan Rate Models |

### Slide 33: Performance Evaluation: HTU/NTU

### Slide 34: Gas and Liquid Diffusivities

### Slide 35: Design: HTU/NTU Method

### Slide 36: Performance Evaluation: Kremser Method – Steps

### Slide 37: Performance Evaluation: Edmister Method - Steps
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

### Slide 38: Performance Evaluation: HTU/NTU Method
- Mass balance around Initial section in terms of vapor concentration
  - gas compositions are easier to measure - gas chromatography, infrared (IR), non flashing, uniform composition, etc.
- HOG : physical efficiency of the packing
- NOG : difficulty of the separation
- Vapor flow rate (V) is a function of tower diameter
- Z: packing height required to achieve separation

### Slide 39: Kremser Method: Design

### Slide 40: References
- Mass Transfer Coefficient Correlations
  - Structured Packing:
    - Bravo, Fair, and Rocha correlation [Chem. Eng. Progr. 86(1), 19 (1990); Ind. Eng. Chem. Res. 35, 1660 (1996)]
    - https://pubs.acs.org/doi/pdf/10.1021/ie00016a010?ref=article_openPDF
  - Random Packing:
    - Bravo and Fair correlation [Ind. Eng. Chem. Proc. Des. Dev. 21, 162 (1982)]
  - Perry’s Table 5-24 provides correlations:
    - Sherwood/Holloway, Onda, Bravo/Fair, Reiss, etc.
- Applied Process Design, Volume 2 (Ludwig)
