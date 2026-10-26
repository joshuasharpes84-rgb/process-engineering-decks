# Rules of Thumb

Cross-equipment heuristics: control valve authority, PSV relief scenarios, pump BEP/efficiency tradeoffs, and heat exchanger simulation methods.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/rules-of-thumb/
- **Download the .pptx (2 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Rules-of-Thumb.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 43

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Rules of Thumb
- Joshua Sharpes

### Slide 2: Valve Authority
- Control Valves should be contributing to 50-60% of system pressure drop to have adequate control of that fluid

### Slide 3: Heat Exchanger Temperature Approach
- Cooling Towers: Cooling water should experience anywhere from a 10-40F rise.
  - <10F  Oversized exchanger/lack of throttle
  - >40F  Undersized exchanger/excessive throttle
- Condensers: similar to cooling towers
  - Cooling Water: ∆20-30F
- Reboilers:
  - Steam: ∆ 30F – 50F
  - Hot Oil: ∆ 50F – 100F

### Slide 4: Heat Exchanger Temperature Approach Location (Countercurrent Exchangers)
- Continuing off last slide, the location of the minimum temperature approach in the exchanger is correlated to the effective heat capacity of the stream:
  - For a 1/1 pass countercurrent exchanger, the more sensible fluid will reach the minimum approach at the opposing stream’s inlet

### Slide 5: High-Pressure Entry into Low-Pressure System (Breakthrough)
- API 521 Establishes the following evaluation pathway:
  - Is direct equipment able to tolerate increased pressure?
    - 10/13 rule for exchangers
  - If no: does LP side have existing relief path? Is it rated for breakthrough flow?
  - Existing relief inadequate  size PSV for new rate

### Slide 6: Vapor Blowdown
- To blowdown a vessel in case of fire; the operating pressure should be lowered to whichever is lower:
  - %50 of Design Pressure
  - 100 psi
- This should be done in <15 min, per API 521 4.6.6.3

### Slide 7: NPSH Cavitation Margin
- To avoid cavitation, NPSHa  should be significantly greater than NPSHr. The exact clearance is correlated to fluid viscosity:
  | Condition | Recommended NPSH margin over NPSHr |
  | Clean cold water, non-critical service | 1.1–1.2× (HI minimum) |
  | Hydrocarbons, hot water near boiling | 1.2–1.3× |
  | Viscous fluids | 1.3–1.5× |
  | Slurries, erosive service | 1.5–2.0× |
  | Critical service, no spare | 2.0× |

### Slide 8: Pump Thermodynamic Assumptions
- Pumping can be assumed to be:
  - Adiabatic: process is fast  no heat lost to surroundings. All energy goes into temperature rise of fluid
    - Less applicable for viscous, low flow, cryogenic operation
  - Isentropic (Reversible): assumes no friction, turbulence, or dissipation
    - Less realistic than adiabatic assumption but necessary for simple Thermodynamic Coefficient Derivation (see example problem)
    - Assumption is less applicable for low efficiency operation, multiphase (cavitation, slurries), and high-pressure ratios

### Slide 9: Pump True Efficiency
- This should be prefaced: Reliability takes precedence over energy consumption – a shutdown will undo any accumulated savings
  - Typically, single stage centrifugal pumps have BEPs from 65-95%
  - It is best to be slightly on low-flow side of BEP for a given impeller diameter
  - BEP best supports reliability but requires higher overall discharge rate – more power - due to excessive recycle flow
    - Operating significantly away from BEP imposes reliability problems
  - Beyond a fixed impeller, fixed speed assumption:
    - VFDs can be implemented for variable power
    - Impeller size can be altered
  - In chemical plants, energy consumption is dominated by heating sources and compression:
    - For more moderate operating conditions,  pump electricity consumption is proportionately higher

### Slide 10: PSV Chattering
- Typically, single PSV chatters if
  - Set pressure is exceeded  AND
  - Relieving rate <25% of governing relieving rate
- Several ways to address this:
  - Orifice is too large: confirm design basis and decrease area
  - Inlet PSV piping has dP >3% OR Backpressure exceeds 10%: piping modifications
  - Set pressure is frequently exceeded: Pilot-operated PSV selection
- Single PSV design good but still chattering?  switch to multiple PSVs
- All of this to say, valve could just need maintenance

### Slide 11: Tower Reflux and Boil-up Operation
- For complete condenser, temperature set point is the bubble point of the mixture  ensure complete condensation but no subcooling
  - To avoid cavitation in reflux, accumulator is kept elevated relative to pump centerline
  - Advanced control schemes involve accumulator pressure controller cascading temperature setpoint to adjust for composition (and bubble temperature) changes
- For partial boil-up of tower sump (typical for distillation), temperature set point is also the bubble point of mixture
  - Secondary temperature measurement of first stage vapors used for setpoint change in the case of composition change

### Slide 12: Steam Reboiler Operation
- Vertical orientation = fast dropout of liquid to reduce tube film buildup
  - Ufilm < Udrop   See condenser presentation
- Heat of vaporization release is proportionately higher than otherwise sensible changes
- These reasons are why saturated steam is fed to the top of vertical, countercurrent, 1/1 reboilers for most distillation tower services

### Slide 13: Heat Exchanger Simulation ProcessSource: Heat Exchanger Handbook (HEHB)
- For a geometrically defined exchanger, the streams are put together and assumed outlet conditions
  - Outlet properties are a function of heat capacity ratios (and/or latent heat for phase change)
- Segmented approach is used to model increments in exchanger
  - Properties are iterated along linear temperature curve
  - Temperature curves are adjusted based on heat transfer (a function of exchanger geometry)
- Flow, Pressure Drop Correlations:
  - Tube Side:
    - Nusselt : Dittus-Boelter
    - Pressure Drop: Darcy-Weisbach (tubes) + Nozzle/Entrance/Exit Losses
  - Shell Side: See Correlation Selections
    - Nusselt: Bell-Delaware Method (or Kern, Wills-Johnston)
    - Pressure Drop: Bell-Delaware Method (or Kern, Wills-Johnston)
      - (entrance, exit, crossflow, window losses)

### Slide 14: Separation Efficiency (N) Pressure Dependency
- Increasing tower pressure requires higher reboiler temperature
- Increasing temperature raises saturation pressures of both light and heavy keys (LK, HK)
  - By Clapeyron relationship (differential form), P_sat_HK raises at faster rate, reducing alpha
  - Number of stages increases as relatively volatility (ratio of saturation pressures) approaches 1
- Increasing tower pressure will disproportionately increase required number of stages for azeotropic mixtures
  - Conversely, tower pressures have little effect on wide-boiling mixtures

### Slide 15: Absorption Factors & Efficiency
- For performance evaluation (Kremser/Edmister), initial guess for absorption factor must be provided:
  - 1.2 < Ai  < 2.0 is typical:
    - Lower Ai  requires more trays; harder separation
- Estimation of efficiency for Kremer-Design can be taken from Figure 8-29 (Ludwig) which depends on Henry’s Constants (also use Fig.13-3 in Seider):
  - Absorber efficiency: 30 – 50 %

### Slide 16: Trayed Tower Sizing (13.6 of Seider)
- Tray Diameter is selected to avoid flooding
  - Vapor Velocity (flux) is selected to be 75-85% of flooding limit for trayed towers
    - Where Uf  is is vapor velocity (Souders-Brown Equation for single stage)
- Tower height is dependent on tray diameter (& # of trays):

### Slide 17: Separation Process Selection (1/2)
  | Separation process | Feed condition & approx. mass fraction of key component | Separating agent, force field, or gradient | Normal feed capacity, kg/s | Key process advantages | Key process limitations |
  | Distillation | Liquid and/or vapor; 10⁻³–0.95 | Heat transfer | 10⁻³–10³ | Simple flowsheet, low capital investment, easily scalable, most widely used | Needs adequate relative volatility and thermal stability of components; low energy efficiency |
  | Azeotropic distillation | Liquid and/or vapor (dictated by azeotrope) | Liquid entrainer plus heat transfer | 10⁻²–60 | Breaks azeotrope; operates at normal temperature and pressure; easily scalable | System more complex; requires recovery of entrainer; increased capital investment |
  | Extractive distillation | Liquid and/or vapor; 10⁻²–0.95 | Liquid solvent plus heat transfer | 10⁻²–60 | Handles low-relative-volatility mixtures; normal temperature and pressure; easily scalable | Requires compatible solvent with high recovery; system more complex; increased capital investment |
  | Absorption | Vapor; 10⁻²–0.95 | Liquid absorbent | 10⁻²–30 | Good for recovery of soluble gases; moderate capital investment | Requires low-cost solvent and recovery system; cross-contamination |
  | Stripping | Liquid; 10⁻²–0.75 | Stripping vapor | 10⁻²–30 | Strips volatile component from liquid; simple operating conditions | Requires recovery of volatile component; involves cross-contamination |
  | Extraction | Liquid | Liquid solvent | 10⁻³–18 | Great flexibility in selective solvents; easily scalable | Mutual solubilities of other components; cross-contamination; solvent loss |
  | Crystallization | Liquid | Heat transfer | 10⁻³–18 | Single processing step at low temperatures; low energy requirements; large capacity variation | Staging not easy; may require purification; limited to certain crystallizing components |
  | Microfiltration | Liquid | Microporous membrane | 10⁻¹–1 | Low-pressure separation of suspended solids and fine particles | Membrane fouling; concentration polarization; limited selectivity |
  | Ultrafiltration | Liquid; 3×10⁻⁵–4×10⁻² | Microporous membrane | 10⁻²–1 | Wide variety of membranes with range of selectivities | Membrane fouling; concentration polarization |
  | Reverse osmosis | Liquid; 7.5×10⁻⁴–4×10⁻² | Nonporous membrane | 10⁻²–5 | Effective for dissolved solutes; relatively energy efficient | Requires repressurization of retentate stages; tends to foul with fouling fluids |
  | Pervaporation | Liquid; 5×10⁻⁴–0.25 | Nonporous membrane | 10⁻³–1 | High selectivity for dilute components | Low flux; requires downstream condensation of permeate |
  | Adsorption | Vapor or liquid; 2×10⁻³–2×10⁻¹ | Solid adsorbent | 10⁻³–30 | High selectivity for low-concentration streams; good for gas purification | Requires recovery sequencing; needs high selectivity and easy regeneration |
  | Electrical field and gradient separation | Vapor or liquid | Centrifugal, electric force field, or thermal gradient | Generally very low | Effective when electrical or gradient forces enhance the separation | Generally restricted to low flow rates; high equipment cost and complexity |

### Slide 18: Separation Process Selection (2/2)
  | Separation process | Feed condition & approx. mass fraction of key component | Separating agent, force field, or gradient | Normal feed capacity, kg/s | Key process advantages | Key process limitations |
  | Settling and sedimentation | Liquid or gas with solid; 10⁻²–0.4 | Gravitational | 10⁻³–2×10³ | Separation based on gravitational field; large capacity; low capital and maintenance costs | Poor separation; dusty; high filtrate loss; requires large differences in density; poor with slurry mixtures |
  | Flotation | Liquid and solid; 5×10⁻⁴–4×10⁻³ | Adsorbent gas and surface activity | 10⁻²–4×10² | Useful in solid-solid separation; large capacity range | Separation based on selective gas-bubble attachment; high operating cost to attain suitable particle size |
  | Centrifugation | Solid-solid or liquid-solid; 4×10⁻³–0.3 | Centrifugal force field | 10⁻⁴–10⁻¹ | High separation efficiency | High capital and energy costs; limited capacity; discharge difficult |
  | Drying | Wet solid; 0.5–0.99 | Gas and/or heat transfer | 5×10⁻⁴–2 | Final drying of solids once most liquid has been removed | Staging inconvenient; may require parallel units; high energy requirement |
  | Evaporation | Liquid | Heat transfer | 10⁻¹–30 | Used when relative volatility is high (>20) | Low thermal efficiency |
  | Condensation | Vapor | Heat transfer | 10⁻¹–30 | Recovery of less-volatile components in vapor; condensation of vapor | Appropriate coolant required |
  | Filtration | Liquid-solid or gas-solid; 10⁻²–0.75 | Pressure gradient plus porous filter | 10⁻⁶–10³ | Good solid-liquid separation of fibers, pulps, granules, slimes; low capital cost | High operating cost; often batch operation; poor with toxic or hazardous materials |

### Slide 19: Reflux Ratio: Actual to Min
- Most literature have vague estimates:
  - This value approaches 1 for increasing number of stages over Nmin
- Exact value is based on empirical results: dependent on distillate quality and reboiler energy

### Slide 20: K Factors (Separation)
- The K value for a component is dependent on
  - Gas Ideality: nominally pressure dependent.
  - High pressures require fugacity coefficient
  - Liquid Ideality: dependent on bonds and temperature.
  - Chemical Bonds: significant attraction or repulsion alter activity coefficients
  - Temperatures: supercritical temperature require Henry’s law constant substitution for vapor pressure
  - Concentration: infinite dilution, like supercritical temperature, requires use of Henry’s constant
- *unfavorable solubility results in xi  substitution for γi

### Slide 21: Efficiency of Liquid-Liquid Extraction (Column Towers)
- Notoriously difficult to estimate E0  as it is dependent on multiple fluid properties: interfacial tensions, viscosities, etc.
- Best practice is to estimate Ntheoretical  through Hunter-Nash Method and then use HETS
  - Height is more appropriate since vessels are continuously spaced (opposed to discrete stages)
- HETS can be estimated from Table 8.5 (Seider)
  - HETS is known  to correlate with tower diameter
- And column height:
- ^HETS = 2 – 4 ft   for Dtower  = 3 – 4 ft

### Slide 22: Gas Membrane Separation - Mixing
- Perfect mixing is unrealistic but necessary assumption for lack of simulation software.
  - Membrane area is sized according to uniform flux behavior in mass balance derivations
    - See Peters Chapter 15
- More advanced models utilize 1-D differential equations
  - Extremely advanced models (polarization, non-uniform flow distribution) required simulation software with 3-D DiffEQs

### Slide 23: Adsorption – Langmuir Models

### Slide 24: Adsorption: Bed Height Approximation
- Collins developed this technique which uses isotherm symmetry to predict length of unused bed:
      - Where larger f indicates adsorption effectiveness of mass transfer zone, MTX
  - Which is then totaled to saturated portion of bed, LES, to determine total length, L:
- See Peters textbook, section 15 for LES, LUB equations

### Slide 25: Dryer Selection
- Moisture content is  main criteria for dryer selection:
  - It varies throughout drying process; sometimes multiple stages required
  - Phase is observable through yield stress vs moisture content curve
- Additional criteria:
  - Flow Rate
  - Particle Size
  - Heat-sensitivity
  - Attrition Resistance

### Slide 26: Multiple Flow Control Valves
- These need to be in parallel
  - If they are in series; will compete even in the presence of branch-lines
    - If the branch line is not flow controlled and is a larger portion (X) of the total flow, then series arrangement is acceptable

### Slide 27: Compressor Efficiency Estimates
- Polytropic Efficiency, η, is approximately 70-80%
- η  increases with flow rate and pressure ratio

### Slide 28: Adsorption Regeneration Selection: PSA vs. TSA

### Slide 29: Molecular Sieve Allowable Pressure Drops

### Slide 30: Payback Period
- Typically, a pack back period of 5 years is deemed the maximum tolerable period for investment screening
  - Some companies use ROI, NPV, or Discounted Cash Flow RR:

### Slide 31: Minimum Acceptable Rate of Return
- Companies select mar based on project risk: higher risk requires higher return
- Pump replacement
- New PE unit w/ unfamiliar tech.
- New carbon capture technology
- Examples

### Slide 32: Viscosity Distinguishment for Equipment Selection
- Most classifications are vague; folklore. Here is best establishment that draws from multiple resources:
  | Tier/ Viscosity |
  | Low: <100 cP |
  | Medium: 100-1,000 cP |
  | High: 1,000 – 500,000 cP |
  | Very High: > 500,000 cP |

### Slide 33: Tube Side Pressure Drop
- Typically, pressure drop in tube side is dominated by straight tube losses: roughly 20-30% of total pressure drop losses
  - Source: Coulson/Richardson Engineer Surveys

### Slide 34: Dry (Gaseous) Corrosion Protection
- Most common is Alloying (Passivation)
  - Since corrosion is inevitable, having that corrosion produce the protection layer for future corrosion is inherently sustainable:
    - Material produces its own coating
  - PBR (Pilling-Bedworth Ratio) measures the oxides ability to adhere to metal surface and block diffusion (a function of porosity) gaseous reactants to that surface
  - Sometimes, promoters are added to boost this film buildup
- Next most common method is Protective Coating
  - Selection is limited as most thermally degrade

### Slide 35: Condensation S/T Allocation
- Run through these criteria until allocation and orientation is defined
- Fouling is first criteria: (1) Severity of either method and (2) method type
  - For severe fouling:
    - Particulate: tube-side, orientation depending mixture composition
    - Liquid-Film: shell-side, horizontal
- Condensation extent is second:
  - Partial Condensation: Shell-side
- Mixture composition is third:
  - Multi-component: vertical
- If none of these apply: shell-side, horizontal is default

### Slide 36: Shell-side h, ∆P Correlation Selection (See Prior Slide)
- Potential options are Kern, Bell-Delaware, and Wills-Johnston
  - These methods differ by leakage estimation technique
- Kern: least accurate -- best for first-pass estimation
  -  Assumes complete cross-flow, no baffle/tube leakage
- Bell-Delaware: moderately accurate -- best for well-defined geometries
  -  Implements adjustment factors to estimate leakage:
    - Baffle-window, tube-baffle, shell-baffle, bundle-shell leakages are all considered
  - Aspen uses this method w/ its own modifications for adjustment factors
- Wills-Johnston: most accurate -- best for rigorous simulation
  -  Uses flow path (bundle, window, etc.) to converge iterations on solution
- All three methods compared in Problem 14-6 of Peters:
  | Method | h_s (W/m²·K) — mine / book | dP_s (Pa) — mine / book |
  | Kern | 3352 / 3369 | 16,414 / 16,420 |
  | Bell-Delaware | 2917 / 3080 | 9,382 / 9,481 |
  | Wills-Johnston | 2986 / 3004 | 4,055 / 4,103 |
- ∆P  is much more sensitive to leakage assumptions

### Slide 37: Internal Reboilers
- Internal Reboilers should only be considered for tower diameters greater than 6 feet in diameter
- Potential option for brownfield retrofit to get additional duty
  - Downside: significantly lower heat transfer coefficients, difficult maintenance/monitorization.

### Slide 38: Tower Ambient Heat Losses
- These are typically 1-3% of Reboiler Duty
  - Up to 5% for colder climates

### Slide 39: Tower Simulation Convergence
- Selection between Stage-by-stage (SS) and Simultaneous-Correction (SC) is dependent on bubbling point range:
  - Check critical temperatures – any below operating temperature Simultaneous-correction
  - Check Kmax / Kmin ratio; >50 requires SC. <50 still might require SC. <10 for SS
- SC solves for every variable in system of equations at once (vector form), requiring exponentially more calculations  This will slow down large process simulations
  - In practice, Aspen uses hybrid to dynamically select approach based on how many convergences are needed to solve process user.
- SS = one stage temperature at a time, SC = all stage temperatures at once

### Slide 40: Turbine to Compressor Ratio
- For Centrifugal Compressors, typically 2-3 compressor barrels are allocated per turbine shaft, driven by steam.
  - This helps

### Slide 41: Pump Work in Steam (Rankine) Cycles
- Typically negligible: only 1-3% of net work.

### Slide 42: Centrifugal Pump Lifetime
- Leading failure modes of Pumps:
  - Mechanical Seals (1-3 yrs)
  - Bearings (1.8 – 2.9 years)
  - Wear Rings (2 - 4 years)
  - Impeller Damage (months – indefinitely)
  - Shaft/Sleave
  - Couplings/Alignment (2-5 years)
  - Vibration
  - Process Upsets
  - Driver (motors)
- Mean-time between failures (any type) is 2-3 years.

### Slide 43: Centrifugal Pump PMs
- Following items are typically addressed during Pump Preventative Maintenance:
- Lube Oil Changes
- Vibration Routes
- Alignment Checks
- Seal-support Checks
