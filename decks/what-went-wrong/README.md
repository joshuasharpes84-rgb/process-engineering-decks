# What Went Wrong

26 incident case studies from Kletz with root cause lessons.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/what-went-wrong/
- **Download the .pptx (460 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/What-Went-Wrong-Takeaways.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 27

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: What Went Wrong Takeaways
- Joshua Sharpes

### Slide 2: Compressed Air Hazards (12.1)
- Lubricating oil for air compressors has the potential to oxidize and deposit formed reaction product on the discharge (delivery) line of compressor. A thick deposit layer has the potential to catch fire.
- Best practices to avoid delivery line deposit buildup:
- Suction filters are kept clean
- High temperature alarm on delivery line
- Avoid low rates for extended periods of time (MORE lubrication leak through at lower pressure)
- Discharge piping should not have traps
- Lubricant type change
- There are also non-lubricated compressors

### Slide 3: Nitrogen Blanketing Tanks (5.6.3)
- Purpose of N2 blanketing is to eliminate O2 presence for flammable liquid service
  - PCV should be at roof level on horizontal line to reduce condensation of liquid that would isolate tank
  - Proper N2 supply should be confirmed by operations weekly
  - Proper inerting reduces sparks formed by splashing feeds

### Slide 4: Don’t Assemble it Incorrectly – Air Louvers (27.5)
- Air louvers should close with a downward rotation to deflect entrance of rainwater
- Incorrect installation could reduce furnace performance.

### Slide 5: Changes Made to Handle Abnormal Situations (25.1.4)
- HF Puget Sound Refinery 1998 (case 1): Coker blockage was allowed to cool for several hours but indicators did not capture core temperature of hot material which spilled upon head removal, killing several people
- MOC process was disregarded as operations personnel took too much initiative
- Technical support was limited
- Instrumentation placement was misleading

### Slide 6: A Dust Explosion in a Duct (30.9)
- Aluminum casting facility in Huntington, IN in 2003.
- Dust of dryer-incinerator duct settled over time due to low vapor velocity (or larger duct area)
- Ignition from dryer startup ignited dust and blew open duct, killing one and injuring several.
- No duct filters were in place to remove dust

### Slide 7: Furnace Tube Ruptures (10.7.2)
- Heating medium flow can drop for many reasons.
- When it does, fuel gas to the furnace must be truly isolated with a  control scheme that
  - Blocks flow with primary control valve based on heating medium flow indication
  - Employs safety interlock using secondary valve based on fuel gas flow reading to ensure blockage
- Improper isolation of fuel gas during normal operation leads to tube rupture as heat is not removed.
  - Burners must continue operation else firebox explosion, an event more catastrophic (breakage of shell vs tube), is inevitable.

### Slide 8: Corrosion Sends a Column Into Orbit (28.5)
- Amine absorber tower split open sending tower airborne and flammable contents into BLEVE, killing 17 and damaging overhead aircraft.
- Investigation found weld treatments were inadequate to protect against hydrogen embrittlement resulting in circumferential weld around base.
- Kletz mentions incompetence of operating company and overreliance on contractor resulted in mismanagement of tower

### Slide 9: Backflow through Pumps
- Check valves are inherently unreliable and thus should be put on frequent PM schedules, used in duplicate fashion with varying models, and should be accommodated with isolation valves in standby/shut down operations.
- One example: oil went through single-broken NRV from 15psig tank to atm tank, overfilling through tank’s vent.
  - Design philosophy is important to understand and convey to operators to increase hazard awareness

### Slide 10: Empty Plant That is Out of Use (29.6)
- For vessels not in use for several months, it is best to keep empty. Residual contents have the potential for unwanted phenomena
- UK Nuclear Plant, 1973: One residual sludge reacted and emitted vapors out of tank upon startup.
  - Such residual potentials should be evaluated and addressed with mitigation strategies such as washing. Inherently, plant should reduce product variety/inventory entirely.
  - Standard washout procedures for shut down and start up are usually advised

### Slide 11: When does a space become confined? (24.5.2) (Nitrogen asphyxiation)
- Union Carbide, St. Charles, 1998. 48” pipes were venting nitrogen to protect catalysts. Contractors inspected the end of the large open-ended pipe without entering but needed better visibility and thus requested that blanket be held between them and the pipe end which effectively moved the confined space boundary. 1 died and one was injured.
  - Such procedural improvisations should be reviewed, and for personnel to know the necessity of revision, they should first have intuition of hazards*.
    - *A confined space boundary is not a fixed entity; it can be formed and removed intervention
  - Personal air monitors for oxygen content would be wise practice as blanketing of pipe-ends was insufficient reminder of N2 presence.

### Slide 12: Every Possible Error (11.9) – Entry to Vessels
- Pheonix Fuel Terminals – 1984. Contractor entered toluene storage tank that was not gas-freed without self-breathing apparatus. He was asphalted and fire crew, who cut open tank with hot equipment, ignited vessel. 2 people died and 15 more were injured.
- Entry into vessels required permits to work which ensure:
  - Vessel is purged of flammable toxic vapors and acceptable conditions are verified
  - Vessel is isolated of any contents with slip plates, double block and bleed, and line disconnection methods
  - Vessel atmosphere is monitored before and during work
  - Contractors are given SBAs for hazardous atmospheres

### Slide 13: Stack Explosions (6.1.d)
- (unknown site), stack explosion occurred when flare stack could not be completely isolated with figure-8 plate on blowdown line as existing steam purge on this line was preventing plate closure.
  - Operator decided to replace steam purge with nitrogen purge. The nitrogen cooled the flare steam, condensing it, creating the backflow of air into flare stack, with, which the presence of leaking hydrocarbon, ignited.
- Process change should have been evaluated; nitrogen is often assumed harmless (incorrect), but even so, its impact on the process certainly was not.

### Slide 14: Ammonia Explosion (19.1)
- A Chicago meat packing plant exploded in 1968, killing 9 people and injuring 72, as the result of an ammonia explosion.
- Gasoline was incidentally hit after a truck crash which ignited and pressurized and ammonia tank. While the ammonia tank discharge the contents, these contents were directed to the floor above the gas fire, which eventually ignited.
  - It is important to know the flammability limits of a substance along with the ventilation strategies in combination with the discharge method
  - Venting a high LEL substance into a confined space without proper ventilation can lead to an exceedance of even high LELs.

### Slide 15: A Leak Caused By Surge Pressure (34.4)
- BP, UK, June 2000. Leaking steam valves during maintenance filled road dip which eventually overflowed, rapidly condensing elevated trapped steam causing water hammer to rupture piping.
  - Fast condensation of steam (condensate was much cooler than trapped steam) created vacuum void which high pressure steam filled instantly.
  - Section 6-40 of Perry’s (Hydraulic Transients) mentions’ water hammer specifics

### Slide 16: Hydrogen Produced from Corrosion (16.2.a)
- Sulfuric acid is highly corrosive which can result in the presence of hydrogen. An incident led to the accumulation of hydrogen in the vapor space of a non-vented tank which, when ignited, lifted the tank upward.
- The roof-to-shell weld should be the weak point (frangible roof) so an explosion vents upward. Here that weld was stronger than usual, so the tank split at the base and was thrown 15 m.
  - The base carries the highest hydrostatic and fill/empty cycling stresses; a base failure also releases the contents
- Fit a vent at the highest point so hydrogen cannot accumulate under the roof (Kletz Fig. 16-1)
- Relieving conditions of tanks are not only assessed from abnormal static material conditions but also abnormal charging methods
  - Consider what happens when higher pressure compressor is used.

### Slide 17: Dead-Ends (9.1.1)
- ICI Ammonia plant in UK, 1970. Plant vessel had designed weep holes to allow for leakage of ammonia. Weep holes were under thick insulation and so exact location of holes was not clear, this resulted in misinterpretation of leak method as corrosion was occurring, leading to vessel failure.
  - Fugitive leaks are hard to detect. To ensure leak source, holes of this design should be accessible so that emission test (such as bubbling next to source) can be carried out
  - Abnormalities in equipment features such as these can get lost in translation over time. Unique designs should be eliminated, if possible, through inherently safer design practices.

### Slide 18: Floating Roof Tanks (5.5)
- Wales, UK Refinery 1983, crude oil floating roof tank catches fire when high winds damage roof of tank which was not addressed. Hot carbon deposits dislodged from a nearby flare when the flare load was increased due to a compressor malfunction which ignited tank’s leaking vapors. Fire caused roof to sink which steamed developing pockets of water on roof, entraining tank’s oil into a nearby dike, abruptly extending the fire and injuring several fire fighters.
  - Roof maintenance should have been completed, oil diverted to another tank
  - Flare load and performance of flare should have been evaluated as this carbon deposit presence was abnormal
    - Solids presence could have been linked to compressor failure
  - Tank equipment file should have been used to recognize storm drains on roof and communication relayed with fire team to recognize transient hazard of oil entrainment
    - This is a doable task when an emergency is isolated to one piece of equipment

### Slide 19: Static Electricity from Powders and Plastics (15.3)
- There was incident (specifics unknown) where dried powder produced static electricity which, when pressurized as the result of a vacuum reduction, led to the decomposition of that powder.
  - Another incident occurred in Japan where powder was heat as the result of tightened impeller packing, resulting in explosive decomposition
- Static Discharge is a difficult hazard to navigate but here are mentioned strategies from GEDPS in the context of powders
  - Conduction materials (packing)
  - Elimination of pinch points with rounded vessels – leads to congestion
  - Grounding of components
  - Reduce particle attrition through PSD reduction

### Slide 20: Relief Valves, Vents, Flame Arrestors, and Similar Items (14.2.4)
- Failures due to flame arresters are responsible for 10-20 tank explosions every year.
- Arresters are prone to choke if not cleaned out adequately which leaves tank not only prone to explosion but also to vacuum.
  - Cleaning should be dependent on arrester element.
  - API RP (recommended practices) 2028 specifies that flame arresters should be tested on annual basis and even more frequently for dirtier services. RBIs can increase this frequency (API 580/581)

### Slide 21: Lack of Knowledge (22.1)
- Itabashi, Japan, 1963. Runaway reaction occurred when heating coil of tank corroded and leaked steam into reactor, heating contents for extended period of time. Operator knowledge was that reaction only occurs at higher temperature.
- Lab tests should not be used as the only means in which a reaction/process can occur. Kinetics are just that; time dependent – a reaction can occur at a lower temperature; it just takes longer.
- Engineers are responsible for interpreting lab results not as procedural law but as data – a portion of a highly dynamic scenario.

### Slide 22: Carbon Dioxide Can Ignite A Flammable Mixture (19.4)
- Alva Cape Tanker, NY, 1966 (Page 89 of NFPA Fire Journal). Carbon dioxide inert cooled a tank which formed carbon deposits. These solid deposits collected static charge and ignited the flammable naptha inside of the tank since the tank had not been completely purged of air.
- There was another incident that occurred because of a thermal difference with the inert (another slide mentions nitrogen condensed steam in a flare header); any change in a substance's temperature presents hazards that should be evaluated.
- Static charge was accumulated on solid carbon deposits due to triboelectric charging, a phenomenon more common in heterogenous mixtures due to greater variety in charge interfaces.
- -Refer to Process Safety notes on IPad

### Slide 23: The Longford Explosion (26.2)
- Longford Refinery (Exxon) in Austrillia, 1998. Plant shutdown caused exchanger to equilibrate to lower-than-design temperature. Operators started plant back up despite observing ice on exchanger. Exchanger failed, leaked igniting vapors. 2 dead.
- Lack of Process knowledge among operators was apparent, but behind this were organization changes that left operators in a position to fail. The isolated nature of the plant incentivized engineers/admin personnel to move to Melbourne plant, function as remote resource.
- Additionally, plant found it plausible to expand operator responsibilities in congruence with shorting headcount. Having operators substitute engineers leaves plants vulnerable to situations such as this.

### Slide 24: Feyzin (8.1.1)
- French Refinery (TotalEnergies), 1966. Spherical LFG tank was being drained, valve broke, loss containment, liquids ignited, multiple tanks exploded and caught fire. 18 dead.
- Tanks burst (BLEVE) because liquid is unavailable to absorb heat; pressure ratings decrease as metal gets hot, relief protection is ineffective
- Spherical Tank Leak Fire Prevention:
  - EIV on drain line,
  - limit manual valve size,
  - bottom portion of tank and connections are fully welded,
  - combustible gas detectors
- Spherical Tank Leak Fire Mitigation:
  - fire resistance insulation,
  - deluge on top of tank for cooling,
  - remotely operated depressurization line,
  - slope ground,

### Slide 25: Mists Can Explode (19.5)
- Refinery in UK, 1970. Oil tanks were being cleaned out, contractor decided to use steam in place of hot water for initial wall cleaning agent, followed by kerosene spray as secondary cleaning agent. Fire/explosion followed, 3 killed.
- Contractor procedure was agreed verbally, should be documented. Contractor training should be provided on relevant hazards of operations performed. Contractors should go through proper channels with any modifications/improvisations.
- Sources of ignition are inevitable with contractor work; this is established in work permits. Heating Sources should be LOTO’d

### Slide 26: Water (12.2)
- Water, when mixed with a hot medium, will vaporize explosively. This has happened in several applications with hot oil transfers.
  - The Jakob Number, Ja, is quantifies the relative amount of sensible (super) heat a liquid receives with its vaporization:
    - The higher the Ja, the greater the bubble radius (and subsequent volume/pressure)
  - One example  I have encountered is the vaporization of water with Dowtherm-G reboiler. The transient nature of this operations left cold water in the pot which vaporized led to massive pressure fluctuations which ultimately accelerated Stress-corrosion cracking (SCC)

### Slide 27: Over pressuring With Liquid (5.2.1)
- Great Britian Plant, 1982. 80m3 fiber glass storage tank burst when plastic liner was incidentally left on nozzle.
- Storage tanks are often fitted with top nozzles to relieve liquid at the maximum fill rate
  - A nozzle for liquid relief should be greater than vapor relief (larger dP for vapor)
