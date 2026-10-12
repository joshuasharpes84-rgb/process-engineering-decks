# Engineering Protection Layers

Protection layer hierarchy, SIS/SIL, pressure relief, flare systems, and fire protection.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/protection-layers/
- **Download the .pptx (243 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Engineering-Protection-Layers-Safeguards.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 15

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Chapter 7: Protection Layers (Safeguards) - GFEDPS
- Joshua Sharpes
- Chapter 7 (Protection Layers) is used for design-phase risk reduction and overall safeguard philosophy.

### Slide 2: Engineering Protection Layer Hierarchy
- Engineering Layers of Protection effectiveness are ranked according to effectiveness:
  - Inherently Safer Design (Most Effective): elimination of hazards
  - Control: Automated control of hazards
  - Supervisory: Operator control of hazards
  - Preventative: ESD strategies
  - Mitigative: redirect to Emergency containment vessel (ECV), Flare Header, Dike, Etc.
  - Barrier: Distance, proximity to plant/community population
  - Limitation: Fire fighting, foam knockdown
  - Response (Least Effective): Plant, Community

### Slide 3: Electrical Hazards (7.1)
- Primary concern of electrical equipment is potential to ignite vapors – reason for electrical area classification/division (ANSI standards derived from NFPA 70)
  - Class I/II/III: Flammable Atmospheres, Dust Atmospheres, Fiber Components, respectively.
    - Division I/II: Classification atmosphere is always present, Classification atmosphere is abnormally present, respectively
  - Classification/Division can vary throughout a complex
    - Engineers perform hazard area classification (HAC) – performed initially during FEL-2/3 with potential modification during MOC
- Purging is often impractical as it O2 levels become prerequisite for startup which is why it not often used
- Intrinsic Safety of devices is defined by ANSI/ UL 913
- Static Electricity is mitigated with structural grounding, limited tank fill rates, and lightning rods.

### Slide 4: Instrumented Safety Systems (7.2) (Definitions)
- SIS, a type of IPL, is used separately from BPCS in most industrial control systems
- An automatic SIS/ESD performs an SIF, which are each assigned SILs based on respective PFD
  - There are also manual SISs which have higher PFD (and are always SIL1)
  - Each SIF must contain: Field Sensor, Logic Solver, Final Elements
- ANSI / ISA 81.00.01 / IEC 61511 provide the following
  - Safeguard validation for IPL accreditation
  - Recommended SIL determination methods (Namely LOPA)
  - SIS Life cycle process (hazards analysis, engineering, operation, maintenance, etc.)
  - SIL PFD criteria and verification process
- LOPAs, are performed by implementing IPLs (manual and SIS) to close risk reduction gap. SILs each have risk reduction factors to contribute to this gap closure

### Slide 5: Pressure Relieving Systems (7.3)
- Common overpressure scenarios: Equipment failure (block valve, air fan, reflux pump), thermal expansion (blocked liquid, fire), tube rupture, loss of utilities (instrument air, cooling water, power), runaway reaction, vacuum (ejectors)
- Rotating equipment discharge piping should be rated for deadhead/surge (centrifugal pump, compressor recycles and blowers)
- Rupture disks shield corrosive fluid, balanced bellows manage high backpressure, pilot-operated relief devices for close pressure margins
- DIERS methodology should be employed for phase selection of flow and runaway reaction modeling
- API 2000 should be used for low pressure tanks prone to vacuum, API 520 for dedicated overpressure systems
- Effluent handling system height and destination are a function of material hazards at relieving conditions

### Slide 6: Equipment Isolation/Blowdown (7.4)
- Emergency Isolation Valves (EIVs) can be operated manually/ automatically and locally/remotely for following purposes:
  - Isolate tanks with large amount of flammable material from process
  - Isolate compressor to avoid high temperature excursion
- Depressurization is used to mitigate fire situations where rupture can occur due to high temperature creep despite pressures being under PRV set points
  - This technique should be used as last resort and under precautions:
    - Starting point is typically 50% of design pressure of 100 psig (whichever is higher) and depressurization should take no longer than 15 minutes
    - Low pressure effect on materials need to be considered, additional hazards can arise.
  - Ideally, cooling mechanism to tank such as auto-cooling through retention of fluid in the tank which acts as a heat sink vs vessel

### Slide 7: Effluent Disposal Systems - Flares (7.5.1-2)
- Flare Systems (ANSI / API Std 521) are the most common means of containing flammable contents.
  - Stacks have notoriously high temperatures and resulting radiative heat fluxes, worker safety is important design factor (500 Btu/ft2)
  - Design case of stack capacity is based on common cause failure
  - Operating pressure of flare is based on this max relief rate
  - Two-phase vessels (KO Pots) are required to reduce liquid carryover which perturbs flare stack combustion
    - Liquids can be vaporized with hot loads from other reliefs
  - Water seal drums are between these KO pots and flare stacks to prevent flashback and ingress of oxygen into flare header
    - Freezing of seal drum water is concern, need heat tracing
  - Pilot gas is often loss due to high winds to lack of fuel gas (blocked filter)
  - Oxygen ingress is primarily through low combustion (stack vacuum), or purge gas effect (buoyancy difference or gas/air), or seal drum freezing
    - Layers of protection include purge gas, molecular seal on flare tip, and seal drum
  - Steam is used in flare stack to emit smokeless effluent
    - Regulations (Federal, state, local) are primarily concerned with normal and design rates
  - LP Flares for tank vent headers are common; back flow is extremely hazardous

### Slide 8: Effluent Disposal Systems – Blowdown Systems (7.5.3)
- Equipment Drainage Systems such as sumps are used to drain acceptable amounts of material, per its flammability and toxicity
- Disengaging Drums in cooling water systems are used to separate accumulated organics as the result of defects such as tube failure
- For individual or cumulative relief effluents lines, Quench Drums can be used to cool and knockdown the VOCs as a precursor to the downstream KO Pots
  - Water is usually quench fluid; compatibility should be ensured

### Slide 9: Effluent Disposal Systems – Incineration and Vapor Control Systems (7.5.4-5)
- Permissible burning is regulated by EPA standards such as 40 CFR 761.70
- Waste heat is often recycled for applications such as waste heat boilers
- Because temperatures of vessel much be limited  (per design standards and regulations),
  - CO formation results in cold operations and NOx results in operations too hot, thus the EPA temperature range of 850-1300C is often cited
- Incinerators are used for liquid/solid waste
  - Surge tanks are employed to provide a buffer to allow for a constant feed rate
  - Material compatibility must be ensured, fires are common.
  - Adequate provisions should be provided for inoperable incinerators
- Thermal Oxidizers are used for off-gas disposal
- Vapor Control Systems are used to collect off-gasses from storage and transfer operations.
  - One example is refrigeration of VOC

### Slide 10: Emergency Response Alarm Systems (7.6)
- Air monitoring for detection of fires and toxic, flammable, and high/low temperature fluids is often done at plants discretion based on technique feasibility:
  - Some vapors are lighter than air, minutely concentrated, or possibly confounded with other metrics
  - Fires can be monitored with smoke alarms or IR sensors
- Emergency Response systems should include
  - backup power,
  - accessible EIVs,
  - automated external communication,
  - remote operating stations,
  - security/air monitoring for proximity definition,
  - personnel accountability,
  - evacuation routes to shelters,
  - designated response leaders

### Slide 11: Fire Protection (7.7)
- There are several modes of burning:
  - Hydrocarbon Burning
  - Solid materials
  - Combustible Metals
  - Pyrophoric Material
  - Electrical Equipment
- Regardless of mode, fires need adequate extinguishment, burning  control, exposure protection, and ideally prevention of the fire altogether
- Fire fighting agents must be adequate supplied in coordination with hazard evaluation findings:
  - Water: used from/for hydrant, mist spray system, deluge, dilution,
  - Foam: smothering of emulsifying systems
  - CO2: compressed solution is released which cools flame upon vaporization and displaces oxygen due to density difference
  - Clean Agents: Inert gases and halocarbons used in closed systems
  - Dry Agents: powders that are dispersed on small spill fires

### Slide 12: Deflagration and Detonation (7.8) – Flame Arrest
- Deflagration arresters due to not need pressure impact protection and are typically placed on end of line of nozzle of tank
- Detonation arresters are subjected to splitting air flows preceding the flame which can mechanically damage system.
  - Run-up distance and pipe diameter both impact arrester performance and reliability
- Bidirectional arresters are necessary for lines tying into manifolds
- Arrester Elements (matrices) quench the flames while allowing gases to permeate
  - Numerous elements available

### Slide 13: Explosion Suppression (7.9)
- Oxygen Concentration Reduction is an inherent safeguard where inert gas is charged to achieve Limiting Oxygen Concentration (LOC)
  - This is only way to address Detonation
- Deflagration Pressure Containment is where tank design pressure is selected appropriately. System can be designed to withstand deformation in addition to the rupture prevention, but this requires thicker vessel walls.
- Explosion Venting involves release of built-up pressure through operation of vents
- Isolation Devices include
  - Suppressant Barriers rapidly employ extinguishing agents in vent piping
  - Fast-acting valves
  - Material Chokes such as rotary valves
  - Liquid Seals
- Deflagration + Detonation
- Deflagration

### Slide 14: Specialty Mitigation Systems (7.10)
- Water curtains and steam snuffing are employed depending on operating temperatures
- Mechanical Interlocks are employed to eliminate operation and ensure containment:
  - LOTOs
  - Electrical Switches: forward and reverse contacts
  - Process interlocks
- Inhibitors, quench and dump systems are used to cool and dilute solutions

### Slide 15: Effluent Handling Systems (7.11)
- Drainage control is critical in the case of fires
  - Dikes must allocate material based on composition and subsequent hazards
  - Containment is dependent on capacity – severity of fire. Rainwater can impact this
  - Reactivity of materials is critical – should be considered in plant layout design
  - Topography impacts drainage system design including sumps, trenches, pits
- Relevant standards include NFPA 30
