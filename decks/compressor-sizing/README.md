# Compressor Train Sizing

Compressor train sizing: pressure ratio and capacity tradeoffs, staging and interstage cooling, and polytropic/isentropic efficiency.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/compressor-sizing/
- **Download the .pptx (36 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Compressor-Train-Sizing.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 10

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Compressor Train Sizing
- Joshua Sharpes

### Slide 2: Background
- See other presentation for Compressor Selection

### Slide 3: Compressors + Coolers
- Higher pressure ratios result in higher temperatures:
  - Thermal Expansion of Parts
  - Lubricant Degradation
- Intercoolers are usually required on the discharge of the compressor
- Must find max temperature for individual compressor
  - Determines energy balance that will dictate cooling requirements.
- These dictate max stage temp

### Slide 4: Sizing Workflow
- Specify Flow Rate & Stage-wise Adiabatic Head
  - Note that head is non-linear with stage addition  This is incentive for more stages
- Select Compressor Type(s): See “Compressor Selection” Slideshow
- Get estimated compressor (polytropic) efficiency at these  operating conditions using:
  - Empirical Correlation (Rule of Thumb)
  - Scale known equipment using friction factor ratios
  - Estimated using Correlation Charts (Centrifugal Compressors: Balje)
- Use estimated efficiency to calculate polytropic coefficient, n, to predict temperature rise:
- Compare Tout, Tmax : More Stages?  Back to step 1 (w/ 1 additional stage)
- Calculate Polytropic Head/Power for each stage
- Is (Polytropic) Power Consumption of Compressor Train Unacceptable?  Back to step 1 (w/ 1 additional stage)
  - Use Payback Period Method for crude profitability analysis (5 yrs is max)
- Select/size intercoolers. If temperatures differ significantly, repeat workflow (Step 1 w/ this amount of stages)
- Contact Vendor for actual efficiencies, power consumptions for value refinement
- Compressor Selection

### Slide 5: Compressor Efficiency: Empirical Correlation
- Polytropic Efficiency, η, is approximately 70-80%
- η  increases with flow rate and pressure ratio

### Slide 6: Compressor Efficiency: Scale-Up Method
- Casey and Robinson developed a method to scale-up:
  - Where Bref   is the friction losses at reference conditions and f is the friction factor
- The friction factors for a compressor can be found using equations 23, 24 located in Appendix 1 of this document.

### Slide 7: (Centrifugal) Compressor Efficiency: Balje Chart
- Calculate Specific speed and specific diameter using Adiabatic Head
- Use Chart to Determine ηc

### Slide 8: Typical Maximum Allowable Discharge Temperatures (Tallow )
  | Compressor Type | Max Temperature Ranges (F) | Notes |
  | Reciprocating | 300 - 350 | Presence of flammable gases such as Hydrogen will drop this value |
  | Centrifugal | 392 - 446 | API 617 + Industry Practice |
  | Rotary | 212 - 350 | Heavily dependent on oil type |

### Slide 9: Payback Period Calculation
- Where V = manufacturing CFCI
- Ax  =   non-manufacturing CFCI
- Aj  = annual cash flow
- V + Ax  = Total Fixed Capital Investment
- Where mar = min. acceptable return (%)
- N  =   evaluation period of project (yr)

### Slide 10: Intercooler Selection/Sizing
- See Presentations:
  - Exchanger Design/Rating/Simulation
