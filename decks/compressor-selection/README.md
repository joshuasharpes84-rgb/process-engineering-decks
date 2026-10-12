# Compressor Selection

Centrifugal, reciprocating, rotary, and axial compressor types — performance tradeoffs, vacuum service, and driver selection criteria.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/compressor-selection/
- **Download the .pptx (277 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Compressor-Selection.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 14

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Compressor Selection
- Joshua Sharpes
- Sources:
- Perry’s
- Chemical Engineers’ Condensed Encyclopedia of Process Equipment

### Slide 2: Contents
- Compressor Background
- Compression Basics
- Compressor Selection
  - Centrifugal Compressors
  - Reciprocating Compressors
  - Rotary Compressors
  - Axial Compressors
  - Fans and Blowers
  - Ejectors
  - Vacuum Applications

### Slide 3: Compressor Background
- Compressors are used for:
  - pneumatic conveying of combustion air
  - pipeline transport of process fluid
  - delivery of compressed air to instruments
  - circulation of process fluids’
- Positive Displacement and Continuous are 2 main types:
  - PD uses volume reduction for intermittent flow
  - Continuous employs dynamic action for uninterrupted flow

### Slide 4: Compression Basics (1/3)
- Main tradeoffs of compression are pressure ratio and capacity
  - Higher pressure ratios (POutlet/ PInlet) also limit the capacity operating range
- Operating range is the difference between the Surge Point (min flow) and the Choke Flow (max flow)
  - Inadvertent surge point transgression results in catastrophic failure of compressor
    - Common practice is to limit operating range to reduce chance of reaching surge point

> Speaker notes: Operating Parameters -> non-ideality -> 
Need to go from operating parameters. Then talk about ideal vs nonideal compression scenarios. Then list contributions towards efficiency. Heuristics should be portioned throughout these steps.

### Slide 5: Compression Basics (2/3)
- Ratio of heat capacities (k) is equivalent to inverse of molecular degree of freedom:
  - It is easier to compress higher molecular weight gases (see next slide)
- Polytropic case (n>k) uses n in place of k to consider non-idealities; higher temperature rise compared to adiabatic case:
-  Higher n = greater temperature rise

### Slide 6: Compression Basics (3/3)
- For any compressor scenario, head, efficiency, and power are used to gauge performance
- Polytropic Head is the energy consumption of the pump:
- Polytropic Efficiency compares real compression to ideality:
- Polytropic Power is the rate of energy consumption:
- Depending on the type, speed, and construction of compressor, efficiency ranges from 65-90%

### Slide 7: Compressor Selection
- Compressor selection is primarily based on capacity and head requirements 
  - Additional parameters for consideration:
    - Reynolds Number, NRe
    - Specific Speed, Ns
    - Specific Diameter, Ds
    - Flow Coefficient, ф
    - Pressure Coefficient, Ψ

### Slide 8: Centrifugal Compressors [Continuous, Dynamic]
- High compression ratios, low flow rates
- Multiple stages are used for lower power input
- 3 types of impeller blades, backward-curved are most common
  - Blade impacts flow coefficient
- Surges at min flow, chokes at max flow

### Slide 9: Reciprocating Compressors [Positive Displacement]
- High pressure ratio, low flow
  - Discharge gas temperature is what limits pressure ratio
    - Lubricant can degrade and parts can thermally expand
- Single- or multi-stage options; multi-stage requires interstage coolers
- Single- or double-acting rods
  - Double has compression chambers on both sides of reciprocating motion
- Typically ~80% efficient
- Rod Packing Failure presents overpressure scenario of housing piece
- PSV required on vent piping

### Slide 10: Rotary Compressors [Positive Displacement]
- Straight Lobe Type
- Screw Type
- Sliding Vane Type
- Liquid Pison Type

### Slide 11: Axial Flow Compressors [Continuous, Dynamic]
- Low head, high flow
  - Small operating ranges
- Characterized by short, orthogonal blades that decrease in height along flow path
- Used for gas turbines and airplanes

### Slide 12: Fans and Blowers
- These are sometimes used interchangeably, as in picture ->
- Primary difference between these is delivery pressure difference:
  - Fans: <0.5 psi
  - Blowers: <1.5 psi
- Axial Flow Fans are most common type of fan:
  - Ideal for high flow rates and low-pressure applications such as general recirculation/exhaust
- Centrifugal Blowers are most common type of blower:
  - Delivery pressure, temperature, and efficiency are primarily dependent on blade selection (radial, forward and backward-curved options)
  - Single and multistage options
  - No cooling required (Ratio ~ 3.5)

### Slide 13: Ejectors [Continuous]
- Compressor alternative that uses steam to rapidly displace gas, creating vacuum.
- Two main ejector types:
  - Steam jet ejector: single steam nozzle
  - Booster jet ejector: multiple steam nozzles for higher velocity and greater vacuum
- Ejectors are comprised of steam nozzle that injects steam concurrently with process gas through mixing section and diffuser element
  - Diffuser element throttle flow to convert kinetic energy into pressure; reverts system back to positive pressure
- Ejectors are low maintenance and low cost with tradeoff of environmental concerns

### Slide 14: Vacuum Applications
- Different compressors can pull lower pressures  requires lower operating temperature:
  - Sealing fluid must be kept in liquid phase – bottlenecks suction pressure
    - This is why rotary oil-sealed is much better than rotary water-sealed
