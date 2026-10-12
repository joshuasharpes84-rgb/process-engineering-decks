# Inherently Safer Design

ISD strategies applied unit-by-unit across reactors, columns, HXs, dryers, and piping.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/isd/
- **Download the .pptx (453 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Guidlines-of-Engineering-Design-for-Process-Safety-ISD.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 17

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Strategies for Inherently Safer Design
- Joshua Sharpes
- Source

### Slide 2: Process Safeguarding Practices
- Hierarchy of practices based on effectiveness towards reducing risk:
- Initial Capital and Reliability decrease the more active the approach
- Operating Cost and Complexity increase the more active the approach
- Ideally, engineers incorporate considerations early in design process to minimize the number of active modifications for operating group
  - This practice is referred to as Inherently Safer Design

### Slide 3: Inherently Safer Design
- Strategies are implemented from top-to-bottom with the goal of addressing the root cause
- This shows how initial section of technology is critical; engineers in both design and operations should aim to make changes more inherent

### Slide 4: Basic Process Control Strategies (BPCS)
- It is best to incorporate a centralized control system so that operations can identify and mitigate deviations from normal operating conditions
- DCS should have alarm management system to prioritize deviations based on their criticality

### Slide 5: Tank Reactor ISD
- Uncontrolled, runaway reactions are the biggest hazard for this unit operation. Passive design solutions for different reactor types:
  | Event | (Potential) Passive Solution |
  | Constituent overcharge | appropriately sized surge tank |
  | Heating medium leak | external heater |
  | Loss of agitation | external agitation by means of circulation |
  | Excessive heating | selection of medium with maximum temperature (steam vs hot oil) |
  | Insufficient residence time | flow-limiting orifice on feed line |
  | Insufficient upstream mixing | implementation of static mixer |

### Slide 6: Continuous Reactor ISD
- Likewise, here are strategies to mitigate runaway reactions for continuous reactors (PFR, packed bed, etc.):
  | Event | (Potential) Passive Solution |
  | Back flow of constituent | PD pump to ensure flow |
  | Maldistribution of flow | Smaller diameter – division into tubes |
  | Catalyst Impurities | Pre-treater unit |
  | Insufficient Cooling | Smaller diameter – division into tubes |

### Slide 7: Mass Transfer ISD
- Applies to absorbers, strippers, distillation towers, etc.
  | Event | (Potential) Passive Solution |
  | Excessive Vapor Flow (Flooding) | Liquid knockdown device such as demister, cyclone |
  | Accelerated corrosion due to pure component state from excessive/insufficient separation | Metallurgy designed for single phase liquid. |
  | Plugging due to entrained internals | Protective screens on inlets |
  | Poor vapor flow distribution | Smaller tower diameter |

### Slide 8: Heat Transfer Equipment ISD
- Most safety concerns result from leaks, ruptures, and trapped material:
  | Event | (Potential) Passive Solution |
  | Buildup of Reactive Material (Sludge) | Evaluation of reaction hazards under assumption of unsuspecting material presence |
  | Cooling Tower Emissions | Tube Leak Prevention Measures |
  | Exceedance of Temperature Range | Material of construction selection from freezing and superheating consideration |
  | Buildup of Non-condensables | Nozzle vent (usually on shell) |
  | Fouling | Vaporization control, exchanger type, higher tube velocity, no U-tubes, larger area |
- TUBE LEAK PREVENTION:
- Thermal difference reduction
  - Multiple exchangers
  - Heat Throttle
- Proper sealing (welding)
- Floating heads
- Erosion Resistance
- Corrosion Resistance
- 10/13 Rule:
- Low-P side-should be 10/13 of high-P side so PSV is not required in case of rupture

### Slide 9: Dryer ISD
- Biggest hazard of solids drying is combustible dust
  | Event | (Potential) Passive Solution |
  | Combustible Dust Presence | Eliminate attrition with smooth conveying, install dust knockdown device (freeboard, filters, etc.), increase velocity/suspension of duct flow |
  | Inadequate Ventilation | Properly sized dampers, damper close prevention, |
  | Flammable Vapor Presence | Proper inerting, proper ventilation, change heat medium potential (hot oil -> steam), proper drainage of condensed vapors (slopes and low point drains) |
  | Scaling | Smooth, geometric consistent surfaces of designs. |
- Multicomponent vapor mixtures present greater flammability hazards as LEL/MEC and MIE are all reduced.
  - Moreso, deflagration index is higher as regions of volume are more likely to have ideal stoichiometric ratio

### Slide 10: Centrifugal (and PD) Pump ISD
- Deadheading and cavitation are primary concerns:
  | Event | (Potential) Passive Solution |
  | Cavitation | Minimize resistance on suction line, double seal, higher absolute pressure upstream,  elevated supply tank, blanketing supply vessel |
  | Deadheading | Recirculation line, discharge piping pressure rating, non-decomposing material |
  | Seal Abrasion | Filter/cyclone/strainer to reduce solid presence, seal flush fluid, diaphragm pump selection, seal-lease pump design |
  | Backflow | Check valve, recirculation line, higher design pressure of supply tank, elimination of parallel pump design, PD pump selection, |
  | Bearing Failure | Oil mist lubrication |
  | Blocked Outlet (PD Pump) | Discharge piping rating, recirculation line |

### Slide 11: Compressor ISD
- Includes centrifugal, reciprocating, rotary types
  | Event | (Potential) Passive Solution |
  | Liquid Carryover | Properly sized disengagement vessel, wet compressor selection, inlet heaters, |
  | Surge (Low Flow) - Centrifugal | Discharge piping rating, discharge piping material of construction (abrasion resistance), PD compressor selection,  Supply system rated for higher pressure, |
  | Overheating | Interstage cooling, cool seal flush fluid, PD compressor selection, wet compressor selection,  inerting, low temperature operation |
  | Overspeed | Solid rotor selection (opposed to built up), |
  | Leakage on Suction | Positive pressure design, sealed system (vacuum), |
  | Contamination | Treatment of seal flush fluid |

### Slide 12: Solid/Fluid Separator ISD
- Centrifuges, Cyclones, Filters, etc.
  | Event | (Potential) Passive Solution |
  | Residual Pyrophoric Content | Slicers to remove contents |
  | Flammable Mixture | Nitrogen interting, nonflammable solvent, wet separator to remove powder stuck on walls, grounding equipment, conductive solvents/additives, fire retardant filter bags, elimination of free parts (screws, bolts, etc.) |
  | Centrifuge Vibration | Flexible utility hoses for isolation, |
  | Blocked Pressure Relief | Flow-sweeping inlet piping |
  | S&T Exchanger: High Tube dP | Tubes need to be rated appropriately to avoid radial stresses |
  | Deflagration Mitigation (NFPA Standards) | Deflagration Venting, suppression systems |
  | Bag House Filters Fires | Reduce operating temperatures |
  | Filter Plugging | Bypass line w/ LOTO, |

### Slide 13: Solids Processing and Handling ISD
- Includes Conveyer Belts, Pneumatic Conveying, Screw Conveyers, etc.
  | Event | (Potential) Passive Solution |
  | Flammable Dust Atmosphere | Nitrogen inerting,  particle size increase,  dense (vs dilute) phase conveying,  bag filters,  ignition source elimination,  outbound bearings of rotary valve,  pelletize form phase (opposed to granule, powder), Grounding components (MIE) Antistatic belt on conveyer Minimize headspace (MAWP in mind) |
  | Explosion | Isolation of upstream equipment with rotary valve, deflagration venting, |

### Slide 14: Fired Equipment ISD
- Includes Process furnaces, boilers, incinerators
  | Event | (Potential) Passive Solution |
  | Tube Rupture | Thicker tubes,  clean process fluids (avoid settling, sulfur attack), stack damper clamp,  tube material.  Clean fuel (no salts or oxygen) – indicated by LHV avoid process flow maldistribution, |
  | Lack of Oxygen | Natural draft louver clamp, back up fan, stack damper clamp, firebox designed for min pressure, |
  | Low Fuel Burning (explosion risk) | Knock out pots/coalescers (liquid fuel), increase stack height (lower ground concentrations in incinerators), continuous pilots for all burners – supply from main fuel line, |
  | High Fuel Heating Value | Avoid incineration, upstream fuel separator, |
  | Waste Gas Backflow to Manifold | Avoid incineration, use of knockout pot for buffer, |
  | High Fuel Gas Pressure | Wider turndown ratio for burners, |

### Slide 15: Piping Systems ISD
  | Event | (Potential) Passive Solution |
  | Overpressure – Loss of Containment | Minimize fittings (lower dP), Minimize flange connections, sweep bends for PRV inlets, CSO’s for PRVs, duplicate PRVs, eliminate dead legs, |
  | Erosion | Sweep Bends (solids), minimize velocity (diameter), metals reduction in pneumatic system (solids/vapors), elimination of hard bends (90 degree), greater pipe thickness, |
  | Corrosion | Material of construction, paints/coatings (CUI), |
  | Vibration | Elimination  of liquid/vapor flow of alternating regimes, pulsation dampener installation, throttling positioned next to vessel entrance, sufficient piping support, |
  | Plugging | Adequate tracing, sloped lines, sufficient velocities to avoid settling, flushing connection for solids valves, |
  | Incidental Loss of Containment | Incompatible hose fittings, latch hands for valves, elimination of fire-prone long bolts on flanges, |
  | Exothermic Reaction/ Static Discharge | Elimination of faulty tracing by embedding insulation, ground all piping for solids/vapor flow, |
- 40% of LOC incidents are through pipework. Use ASME B.31 standards for piping.

### Slide 16: Loading, Unloading, and Drumming ISD
  | Event | (Potential) Passive Solution |
  | Ignitable Vapors | Reduction of splash/dripping, external grounding, reduction of pallet/bag size, |
  | Vapor Emissions from Liquid Pools | Diking of lost material, |
  | External Fire | Adequate Spacing of Tanks, Diking of lost material, |
  | Warehouse Equipment Collisions | Adequate sized warehouse, audible transfer equipment (forklifts), |
  | Loss of Containment | Storage device greater than transport device, hard piping, reduction of pallet/bag size |
  | Vessel Rupture | Design pressure of transfer pump does not exceed downstream apparatus (piping and tanks), flow restriction orifice, elimination of utility dependence (freezing potential), |
  | Contamination | Incompatible hose fittings, elimination of manifolds, |
  | Reaction of Materials | Reactive materials stored in separate areas, elimination  of additives or emulsion agent dependence, elimination of mixing dependence, |

### Slide 17: Utilities Overview
- Heat exchanger leakage is a two-way problem: heat transfer fluid can foul and leak to furnace tube rupture or contamination of process. Cooling water can lead to decomposition of process fluid, or flammable atmosphere near cooling tower.
- Nitrogen is the most dangerous material at a chemical plant. Interchange between it and air leads to asphyxiation in many unassuming scenarios.
- Uninterrupted power supply (UPS) is critical for executing ESD procedure of plant when main power fails.
  - Lack of flow and lack of ability to detect the resulting consequences is exponentially problematic
  - Electricity itself is a heating utility: tracing is all over plant
- Steam is evidentially a critical temperature control agent, but it also used as a purging agent, critical for ESD strategies.
