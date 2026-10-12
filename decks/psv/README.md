# PSV Sizing — API 521

Overpressure scenarios, governing scenario selection, valve sizing, and vapor depressuring.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/psv/
- **Download the .pptx (523 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/PSV-API-521.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 51

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: PSVs – API 521/520
- Joshua Sharpes

### Slide 2: Standards
- API 520: Hardware
  - Part 1: Sizing and Selection
    - Takes relieving conditions (rate, phase, etc.) from API 521 and determines valve type and size
  - Part 2: Installation
    - Determines inlet/outlet piping size
    - Determines installation and maintenance practices
- API 521 Pressure Relieving and Depressuring Systems:
  - Covers Operation of PSV
  - Determines most credible and governing scenario
  - Determines required effluent handing system

### Slide 3: Typical Workflow
- Use API 521 to identify Credible Scenarios
  - Identify Credible Scenario with largest required relieving rate: this is Governing Scenario
    - For this scenario, determine the necessary effluent handing system (this will impact the PSV selection)
      - Use API 520 Part 1 to determine PSV type and size
        - Use API 520 Part 2 to determine PSV installation and maintenance practices

### Slide 4: Terminology
- Common Cause Failures (CCFs): these are inherent failures that impact multiple elements of a system – biggest example is utility failure of instrument air

### Slide 5: Credible Scenario Identification
- Equipment containing a substance is liable to buildup pressure above the operating limits (MAWP) due to operation abnormalities
- These operation abnormalities are known as overpressure scenarios
  - Defined as exceedance of Maximum Allowable Working Pressure
- Most common overpressure scenarios:
  - Exterior Fire, Closed Outlet, Chemical reaction, Thermal Expansion, etc.
  - Complete List in Table 1
- Overpressure, if not prevented or mitigated, can result in loss of containment (LOC)

### Slide 6: Complete List of Overpressure Scenarios – Table 1

### Slide 7: Overpressure Protection Philosophy (API 521)
- Use the following guidelines to navigate overpressure scenario identification, verification, and prioritization:
  - Hierarchy of Protective Measures (4.2.1): Ensure that safeguards are prioritized so that measures can be implement to reduce the need for PSV
    - Engineering Controls: pressure relief (PSV, blowdown)
    - Administrative Controls: pressure prevention (EIV)
  - Use of Administrative Controls if Corrected Hydrotest Pressure Not Exceeded (4.2.2): Ensure that (1) administrative controls are in place, if possible and (2) that administrative controls do not result in exceedance of the hydrotest pressure
  - Double Jeopardy (4.2.3): The simultaneous occurrence of two or more causes of overpressure is not a basis of design
  - Latent Failures (4.2.4): Existing, hidden failures of system components (instrumentation) are not double jeopardy but are considered in the relieving rate of the scenario
    - Assume instrumentation does what we do not want it to do – FC Heat Throttle Valve is wide open
  - Operator Error/Effect of Operator Response (4.2.5): Typical Operator response varies between 10 and 30 minutes
  - Role of Instrumentation in Overpressure Protection (4.2.6): Instrumentation is generally** not a substitute for PSVs:
    - Common Cause Failures (CCFs) make instrumentation unreliable (higher PFDs, lower SILs, lower number of IPL credits, etc.)
    - Instrumentation is a preventative measure, PSVs are a preventative measure
    - **A High-Pressure Protection System (HPPS) SIS can be granted PSV substitution if it has SIL > 3 (ISA standards)

### Slide 8: Determination of Individual Relieving Rates (4.3)
- General Philosophy (4.3.1): good engineering judgement is required; blind adherence to standards is unacceptable
  - Overpressure is the result of energy input from sources of
    - Heat: results in thermal expansion
    - Pressure: directly increases the pressure
- Effects of Pressure, Temperature, and Composition (4.3.2):
  - Composition impacts vaporization and heat capacity
  - Abnormal compositions should not be assumed if the result of another overpressure scenario cause
- Dynamic Simulation (4.3.3): desired for transient pressure scenarios (heat exchanger tube rupture) where relief load requirements rapidly change

### Slide 9: Individual Overpressure Causes and Their Relieving Loads (4.4)

### Slide 10: Closed Outlets (4.4.2)
- Manual and Automatic Block Valve inadvertent closure raises pressure
- For manual valves, administrative controls (4.2.1) such as Car Seals circumnavigate PSV requirement
  - PSV might still be required for high operating temperatures since corrected hydrotest pressure will drop below max source pressure:
    - Pmax Source> Pcorrected   PSV Required
      - See ASME Section VIII: Boiler and Pressure Vessel Code
      - See ASME Section B31.3: Process Piping
- Example: PD Pump Discharge Blockage

### Slide 11: Cooling or Reflux Failure (4.4.3)
- Relieving rate is the excess vaporization (lost condensation) that occurs at maximum normal operating conditions
  - Composition (and vaporization) can change due to failure
  - Double Jeopardy prevents assumption that unrelated event caused failure which would alter relieving conditions
- Notable cases:
  - Total and Partial Condenser Failure
  - Air Cooler Fan Failure
    - Louver Failure
  - Overhead Circuit (Reflux Pump)
  - Pump-around Circuit
  - Side stream Reflux Failure
  - Absorbent Flow Failure
  - Accumulation of Noncondensables

### Slide 12: Entrance of Volatile Material Into System (4.4.6)
- Inadvertent mixing resulting in direct contact can superheat cold fluid past its Superheat Limit Temperature (SLT) which results in Rapid Phase Transition (RPT)
- RPT involves homogenous (bulk) vaporization of liquid volume rather than traditional heterogenous (film) vaporization
  - Results in supersonic shockwave – not relieved by PSV
- RPTs must be avoided through inherently safer design (ISD)
  - only reliable method to address occurring RPT is through containment using thick vessel walls – extremely impractical

### Slide 13: Overfilling (4.4.7)
- When rising liquid level in the tank reaches high alarm; required Operator response time is critical as it impacts need for PRD:
  - < 10 min. response required: PSV strictly required
  - 10 to 30 min. response required: PSV required at company discretion
  - > 30 min. response required: PSV typically not required for this scenario
- In addition to operator response, level instrumentation needs to be evaluated for:
  - Failure Mode Diversity (BPCS vs SIS)
  - Operating Range (should include HH to MAWP level)
    - Out of Range Reading Message
  - Liquid Density Changes
- Overfill effluent can be relieved to either:
  - Atmosphere (5.8.2.4)
  - Flare
  - Low Pressure Disposal System (in-process)

### Slide 14: Failure of Automatic Controls (4.4.8)
- Notable Initiating Events:
  - Control Loop Failure
  - Utility Failure (CCF)
  - Choke Valve Trim Failure
  - High Pressure Let-down Failure
- Failure of both control and normally closed manual bypass is considered Double Jeopardy (DJ)
  - A normally open bypass valve should be considered in capacity calcs
- Failure of multiple parallel inlets is DJ unless CCF exists (utility failure)
- Relieving Capacity is determined by evaluating which case, turndown to normal max throughput, results in highest excess capacity
  - Often this is the turndown case because of the higher upstream pressure
  - Control scheme knowledge is necessary for mass balance evaluation
  - Abnormal operating conditions during relief iteratively impact valve coefficients

### Slide 15: Abnormal Process Heat or Vapor Input (4.4.9)
- Heat input generates vapors and should be calculated based on
  - Clean exchanger surfaces – no fouling
  - Full exchanger capacity
    - Only documented mechanical stops (limit stops) are counted for capacity reduction credit
- Check Valve Failure (Backflow) can either be
  - Complete: maximum back flow, often results in greatest relieving load
  - Severe or Normal: less flow than max – unique dynamic still has potential to cause
    - two-phase relief because of entrainment due to lesser heating
    - runaway reaction due to lesser concentrations
    - flow induced vibration (FIV) on piping
- Reciprocating Compressor Packing Rod Failure leaks vapors into low pressure distance piece
  - Requires PSV on distance piece vent line sized for vapor flow corresponding to annular gap in packing

### Slide 16: Internal Explosions or Transient Pressure Surges (4.4.10)
- Internal Explosions are either of deflagrating (subsonic pressure wave) or detonating (supersonic) nature:
  - PSVs should not be used for either (response too slow)
  - Detonations should be addressed with preventative rather than mitigative (relieving) systems
  - Explosion relief systems, governed by NFPA 68, include rupture disks and explosion vent panels
- Transient Pressure Surges (3 primary mechanisms)
  - Water Hammer & Steam Hammer: PSVs are too slow  use pulsation dampeners, surge valves, etc.
  - Condensate-induced Hammer: elimination of dead legs with pipe sloping, draining, and steam traps are necessary. PSVs are too slow to address this
  - See Section 7.9 of Guidelines for Engineering Design for Process Safety for more technologies

> Speaker notes: Fast Pressure Rise Dynamic of Explosion  Accumulated Pressure > Relieving Pressure

### Slide 17: Chemical Reaction (4.4.11)
- DIERS methodology + API 520 Pt 1 is used for selection of reaction upset scenario to determine relieving conditions and vent size
  - Literature and adiabatic calorimetry tests are referenced
- Reaction upsets are classified as:
  - Tempered: condensable products absorb heat
  - Gassy: off-gas products raise pressure
  - Hybrid: Both
- Reaction upset pathway is critical; extreme temperatures can embrittle metal, altering MAWP for PSV
  - Often, set point is put significantly below MAWP due to fire and fast dynamic  reference Pressure vs Time Curve
- Depending on the rate of reactions, PSVs might be ineffective. Alternatives should be employed:
  - De-inventorying (Emergency Containment Vessels)
  - Inhibitor Charge
  - ESDs
  - Quench
  - Depressurization

> Speaker notes: (rates might

### Slide 18: Hydraulic Expansion (4.4.12)
- Liquid blocked in is prone to thermally expand from utility or process heating
  - Some heat sources have slow dynamics allowing for administrative controls credit
- Liquid flow often requires a small nominal valve size as the lift drops the pressure significantly
  - For the prominent case of two-phase flow, DIERS methodology should be used (HEM/NME methods) for sizing
- Relief rate (liquid flow) is proportional to thermal expansion coefficient of liquid, av
          - (SI Units)
- Piping-only systems are evaluated slightly different

### Slide 19: Fires (4.4.13)
- API 521 covers process vessel fires while API 2000 (low pressure tanks) is for tank farms
  - Size and layout of larger tanks gives more favorable relieving conditions – hence the standard differences
- Open pool fire, confined pool fire, and jet fires are the three types of fires with varying heat fluxes – jet fire being the most intense
  - Greater heat flux = faster failure of metal material
  - Often, open pool fires are assumed (jet fires would be addressed with ISD)
  - Jet fires are often impractical to defend against – best to address source of fire
- Golden Rule = anything above 25 ft is untouchable by fire
- Wetted vs Non-wetted have two different heating dynamics
  - Liquid solution carries away heat – not the case with non-wetted
- Relief Load is typically greater for boiling liquid than expanding vapor
- Relief Service is typically vapor, only two-phase in the case of runaway reactions or foamy materials

> Speaker notes: Relief Service is only two phase initially then vapor at steady state

### Slide 20: Heat Transfer Equipment Failure (4.4.14)
- S/T Exchanger Tube rupture results in high pressure fluid raising pressure of low-pressure side
  - A single, complete rupture of single tube at the backend of the tube sheet is assumed
  - 10/13 Rule is applied to bypass need for PSV for steady state conditions
    - Pdesign, LP Side   >  10/13*Pdesign, HP Side
  - 10/13 Rule might be inapplicable for dynamic case - PSV too slow to act
    - More common for liquid full low-pressure side and violent flashing cases
- Unique Systems:
  - Double Pipe Exchangers: failure is largely due to erosions, thinning of inner pipe
  - Plate & Frame Exchangers: failure is typically due to pitting, cracking, corrosion
  - SRU Waste Heat Exchangers: Heavy duty S/T exchanger w/ high pressure differential – difficult due to solids presence & toxic vapors
    - Best practice is to avoid PSV need through precarious operating and maintenance practices

### Slide 21: Utility Failure (4.4.15)
- Three Types of failures:
  - Local
  - Intermediate: Selective failure which can lead to higher relieving case
  - Total Power Failure
- Utility failures often have domino effect:
  - Lead to other API 521 scenarios
- Loss of Heat often results in light-end carryover
  - Especially for Series Fractionation services
- Instrument Air Failure prevents valves from reaching designated failure position

### Slide 22: Overpressure During Maintenance (4.4.16)
- Often, PSVs are isolated leaving vessels without protection
  - Conservation vents are often relied upon as temporary relief
- Maintenance activities/deviations that result in overpressure:
  - Steaming/Purging
  - Vaporization/reaction of sludge
  - Blocked isolation valves
  - Introduction of high-pressure vapor
  - External fire scenario (usually dismissed)

### Slide 23: Guidance on Vacuum Relief (4.5)

### Slide 24: Guidance on Vacuum Relief
- While vessels are less susceptible to vacuum than tanks, evaluation should still be performed
- Exchangers: tube dP can be breached due to vacuum
- Causes of Vacuum:
  - Volumetric Outflow: pump-out, siphoning, drainage, blocked vents
  - Energy-induced Phase Change: condensation, absorption/adsorption, reaction
- Prevention of Vacuum:
  - Equipment Rating: more difficult with larger vessels – require vacuum rings
  - Instrument Protection System: gas-introducing regulator
    - Calculations for induction rate are complex due to transient nature
  - Relief System: only applicable for low-pressure equipment
    - Introduction of air into high-pressure system is infeasible
  - Operating Procedures

### Slide 25: Vapor Depressuring (4.6)

### Slide 26: Vapor Depressuring Overview
- Depressuring required for scenarios:
  - Ongoing Leakage – reduce driving force of leak
  - Fire – increase failure time of vessel walls
- PSVs can’t depressure for these scenarios since neither will exceed PSV set pressure
- Many PSV alternatives are available:
  - Rupture Disks: unlike PSVs, these heat with vessel walls
  - Manual Intervention: response time is dependent on pressure/material
  - Automatic Controls: SISs, ESDs
    - One SIS is a Fire and Gas (F&G) detectors directly detect flame

### Slide 27: Vapor Depressuring Design
- Design Calculations
  - Vessel/Piping Rupture pressures
  - Time to reach rupture pressure
  - Tolerable/Actual amount of flammable material released upon rupture
  - Brittle failure temperature: Isentropic expansion of gas volume reduces temperature
  - Potential for inoperable valves due to broken internals
  - Cost of incident
- Design Constraints:
  - Flare capacity – this handles relief
  - Vessel Internals can fail due to high dP from rapid flow of material
  - Thermal stresses due to temperature changes
  - Rotating equipment failure due to excess rates (lowered backpressure)
- Additional Design Consideration:
  - Inaccessibility of controls during fire: Fireproofing and backup utilities should be used

### Slide 28: Blowdown Example
- 4.6.6 specifics that operating pressure must be reduced to either (1) half of design pressure or (2) 100 psig in 15 min; whichever is lower
- Ammonia tank needs (MAWP = 350) needs to reach 100 psig

### Slide 29: Vapor Flows (4.6.7)

### Slide 30: Vapor Flows
- Vapor blowdown rate (4.6.6.3) – Equation 24 - is the sum of the
  - Vapor generated by fire (f)
  - Vapor expanded during pressure reduction (density (d) expansion)
  - Liquid flash (v) due to pressure reduction
    - Fire (f):
    - Density (d):
    - Flash (v):
- More Rigorous calculations available
- Notation

### Slide 31: Relief System Design Documentation (4.7-4.8)

### Slide 32: Relief System Design Documentation (4.7)
- Serves as design basis for relevant Management of Change
  - Eliminates potential redundancy
- Every overpressure scenario is listed:
  - Non-credible scenarios are dismissed due to system nature, credits, or double jeopardy  - rationale should be provided
  - Credible scenarios are provided with rationale and evaluations
  - Most credible, governing scenario is identified
- Credits for operator intervention, check valves, vessel insulation, protective instrumentation and drainage are outlined
- Unit operating capacity is listed
  - What if the capacity of unit is increased?  Relief load changes
- PSV Data sheet should be included
  - This applied to equipment-included PSVs (lube oil for reciprocating pumps)
- Piping, effluent system, valves, and admin controls are listed

### Slide 33: Flare Header Design Documentation (4.8)
- Includes:
  - Every overpressure scenario that leads to relief flow into flare system:
    - Initiating Events of scenarios
    - Consequences of scenarios
    - Pressure profiles of scenarios
    - Relief loads and relief load elimination credits (KO Pots, etc.)
    - Backpressure limits
  - Configuration of flare header network: backpressure and pressure drop to flare are critical
  - PSV datasheets for flare header tie-ins
  - Flare system capacity rationale – maximum relieving case due to CCF

### Slide 34: Special Considerations for Individual PRDs (4.9)

### Slide 35: Special Considerations for PRDs
- VLE approach results in flashing across the valve which leads to choking
  - Choking: volumetric expansion  maxes velocity  increases backpressure above limit  Chatters valve  decreases effective PSV capacity
- Solids formation is also possible: mechanism not well understood
- PSVs for vapor service should be positioned to avoid liquid entrainment
- Multiple, staggered PSVs are used when governing scenario demands are too great
  - This setup allows for  better accommodation of lower relieving cases  reduces chattering
  - Built-up backpressure is evaluated for both valves opening

> Speaker notes: A large, single PSV chattering will significantly perturb system pressure
Slight valve lift = massive flow

### Slide 36: Disposal Systems (5)

### Slide 37: Disposal System Selection: Fluid Properties
- Fluid properties of specific effluent at relieving conditions are evaluated first:
  - NFPA HAZ01 is the best resource for flammability
  - Phase of material should be known
  - Toxicity levels require special disposal system (neutralization, absorption, reaction)
- If not routed to atmosphere, effluent is likely to be disposed to shared system: need to know adjacent effluents:
  - Mixing of streams causes reaction, phase change; all of which have the potential to rupture or render system ineffective for relief
  - Water in downstream KO pot is potentially reactive
  - Mixed materials have the potential to emulsify

### Slide 38: Disposal System Selection: Options
- Non-volatile liquids can be discharged to sump or closed vessels
- Condensable vapors should be sent to quench drum/cooling system
- Low temperature fluids, especially those that boil at low pressures, leave piping susceptible to embrittlement
- Line must be heat traced for viscous/slurry effluents
- Sometimes, recovery valves are used to recovery expensive materials by re-routing to process

### Slide 39: System Design Load (5.3)
- Common contingencies and their relieving load are compared: largest results is design load
  - Phase of relief load is important; an extremely high flow rate of saturated vapor could theoretically be completely condensed
  - Load reduction credits can be applied which consider protective measures (HIPS, operator intervention, BPCS) and their PFD levels
- CCFs are often utility-related and these utility failures are not independent from each other
  - Moreso, partial failures have the potential to results in greater relieving loads than total failures
- Fires have the potential to overpressure multiple vessels depending on extent

### Slide 40: System Arrangement (5.4)
- For Single-PRD disposal system, design basis must be greater than PRD effluent design basis (Table 8)
  - PRD Type matters: Pop-action PRDs have higher instantaneous relieving rates    
- Multiple-PRD disposal allocation depends on:
  - Pressure: required backpressure
  - Combability: avoid reaction, formation, and undesired phase change
  - Location: impractical to route across plant

### Slide 41: Piping (5.5)
- ASME B31.3 standards are followed with addition of API 521/520
- Backpressure (Built-up and Super-imposed) should not interfere with relieving capacity
  - Line sizing is performed, knowing backpressure constraints, using isothermal or adiabatic models to avoid choke flow
  - PSV type matters: Bellowed valves have higher BP tolerances
- Piping that is too large is prone to drop-out of liquid phase, accumulation
- Modeling software is highly recommended for two phase flow simulation:
  - Aspen HYSYS
  - SuperChems (ioMosaic)
  - FlaReNet (DNV)
  - And more

### Slide 42: Effluent Flow Modeling: Isothermal
- Effluent pressure drop calculations are assumed to be either adiabatic or isothermal. Here is isothermal graphical method:
- dP increases w/:
- smaller diameter
- Increasing molecular weight
- Source equations are available

### Slide 43: Effluent Flow Modeling: Adiabatic
- Critical mass flux is dependent on gas compressibility (ratio of heat capacities)
- Source equations are available within API 521

### Slide 44: Effluent Flow Modeling: Adiabatic vs Isothermal
- These models represent the endpoints of the realistic behavior
- Real behavior is somewhere in between these two results
- The best practice is run both approaches and resort to more rigorous model if either gives concerning result
  - Could also just redesign system, if possible
  - Most modeling software have both capabilities

### Slide 45: Additional Models: Ideal vs Non-ideal Gas
- Fanno Lines Pressure drop is a method for Ideal Gas estimation: used for low pressure applications
  - IDG models often give higher-than-actual pressure drops
- Rigorous, incremental models are required for non-ideal gas to analyze varying compressibility

### Slide 46: Effluent Model Classification
  |  | Adiabatic | Isothermal |
  | Ideal | High velocity, reduced state | Low velocity, reduced state |
  | Non-ideal | High velocity,  near-critical state | Low velocity, near-critical state |
- Rules of thumb for model selection:
- Velocity governs thermal behavior
- Critical conditions govern ideality
- Low velocity is typically defined as M < 0.7
- For more indiscrete conditions  run multiple models, take average of results

### Slide 47: Mixed-Phase Fluids (5.5.10)
- Homogenous Equilibrium Method (HEM) is employed to estimate built-up backpressure or max tailpipe length under assumptions:
  - No Slip: phase velocities are equal
  - VLE: phases are at same temperature
- Reference pressure and isenthalpic flash data are needed to compute volumetric expansion of solution
- NO Choked flow should be confirmed; otherwise, equation parameters are altered (and chattering is possible)

### Slide 48: Mechanical Design (5.5.11) & Acoustic Fatigue (5.5.12) of Disposal System
- Entire temperature range of relieving cases should be considered for potential embrittlement
- Adequate piping support should be given using  ASME B31.3
- Two-phase flow can induce slug flow  Vibration potential
  - See Annex H (informative) for more info
- Vibration is predicted using Sound Power Level:
  - Higher sound levels correlate to internal weld fatigue
- To avoid Vibration, good practices for disposal design include:
  - Reduce mass flow rate (pressure drop)
  - Thicker piping
  - Minimize fittings (high stress points)
  - Full wrap welds for pipe support

### Slide 49: Flare Header Design Temperature (5.5.13) & Reaction Forces (5.5.14)
- Max/min relieving temperatures to flare are dependent on PRV contingencies
  - Direct fire to flare is only impactful occasionally: usually insulation is provided if severe
  - Flashing of low-BP liquids is most common cause of low T extreme; embrittlement vulnerability
- Hydraulic forces from rapid reaction dynamic can damage piping & PRD
  - Especially common for unsupported, poorly-anchored, and incorrectly installed systems
- Reaction force is calculated in API 520 Part 2

### Slide 50: Piping Support, Sloping, Draining, Heat Tracing (5.5.15-18)
- Supports should be placed in anticipation of compressible fluids and re-directed liquid slugs (another reason for minimal fittings)
- Piping needs to be tied into header from above  drip points are provided for low-sitting PSVs whose piping must rise
  - Piping is ideally sloped downward to avoid liquid pockets (0.25” per 10’)
  - Angles of entry tie-ins are ideally minimized
- Viscous, solidifying flow should be heat traced to prevent blockage

### Slide 51: Disposal to a Lower-Pressure System (5.6)
- Economical route: requires no additional equipment
- Often used for liquid relief
- Example: PD pump discharge relieves back to high-pressure feed tank
  - Minimal impact on feed tank: fluid is subcooled
    - Still serves as contingency for feed tank PSV
  - Prime example of Closed Outlet
