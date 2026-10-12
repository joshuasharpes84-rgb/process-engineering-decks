# Centrifugal Pump Sizing

Single-stage radial-flow centrifugal pump sizing from Karassik: speed, NPSH and suction specific speed, impeller and collector geometry, performance-curve prediction, and axial thrust.

- **Interactive tool:** https://jsharpes-portfolio.netlify.app/#cps-calc
- **Download the .pptx (89 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Centrifugal-Pump-Sizing.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 37

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Centrifugal Pump Sizing
- Joshua Sharpes
- Source: Pump Handbook (Karassik) – Chapter 2.1.1 (Paul Cooper)

### Slide 2: Overview
- Here is overall workflow for conceptualization to installment of Pump:
- Operating Conditions (Q, H, T) → Fluid properties are defined
- Pump Type is Selected
- Selected Pump Type is Sized → This is what this presentation covers
  - Limited to Single-stage, radial-flow designs (no mixed- or axial-flow) :
    - 1000< NS < 2733 : This Workflow
    - NS < 1000 : Regenerative or partial-emission centrifugal (different workflows)
    - NS > 2733 : Mixed/Axial Flow (different workflows)
- Sized Pump is Purchased from Vendor
- Sized Pump is Installed

### Slide 3: Workflow
- Select highest allowable impeller speed, N
- Determine NPSHₐ → NPSHᵣ
- Determine Impeller Speed from Required Specific Suction Speed, Nₛₛ
- Determine Specific Speed (NS ) → Ensure in Range (1. Stage, Radial Flow)
- Figure 12:   NS   Head Coefficient → Impeller Radius using Figure 12
- Determine Impeller, Collector Geometry (1st pass H, Q)
- Verify H, Q through Performance Curve Prediction
  - Manual Computation + CFD
- Adjust Impeller parameters for convergence of H
- Ensure Axial Thrust Stability  Implement Mechanisms, if necessary
  - For Mechansims, repeat Performance Curve Generation

### Slide 4: Impeller Speed, N
  | Number of Motor Poles | Motor/Impeller Speed (rpm) |
  | 2 | 3600 |
  | 4 | 1800 |
  | 6 | 1200 |
  | 8 | 900 |
- Available configurations
- Back to Workflow

### Slide 5: Specific Speed, NS

### Slide 6: NPSH
- Step 1: Determine NPSHₐ using process conditions:
  - NPSHₐ = Hₛ + Hₕₛ − Hf − Hᵥₚ
    - where s = suction, hs = head space, f = friction, and vp = vapor pressure
- Step 2: Determine NPSHᵣ using NPSHₐ heuristic:
- Back to Workflow

### Slide 7: Nₛₛ→ Cavitation
- Back to Workflow

### Slide 8: Impeller Design (2.29-2.39)
- Complete impeller portions in following order:
- Impeller Eye Radius
- Exit Radius
- Exit Width (or Hub Radius)
- Hub, Shroud Profiles
- Blade Construction
- Back to Workflow

### Slide 9: Impeller Design Workflow
- Back to Workflow
- Size Shaft Radius from Torque/Efficiency
- Size Eye Radius by finding impeller eye coefficient through iteration
- Determine Impeller Radius using Figure 12
- Determine Exit Width using Figure 12
- Craft 1st-Pass Blade Geometry (Hub/Shroud Profile) using leading edge velocity target
- Finalize Blade Geometry:
  - Blade Angles using velocity targets
  - Blade Count  using diffusion factor target
  - Surfaces of Revolution using root-mean-square streamline target
  - Leading/trailing Edge Loci using fluid dynamic heuristics

### Slide 10: a) Impeller Eye Radius
- Size rₛ (shaft) from the duty, before the eye:
  - Torque from power:  M = P / Ω ,  P = ρgQH / ηₚ   (first-pass ηₚ from Anderson’s chart, Fig. 10 — needs only Q and Ωₛ)
  - Solid shaft in torsion:   rₛ = ( 16 M / π Sₛ )^(1/3)  ,   Sₛ = allowable shear stress
    - rₛ = 0 for overhung pump
  - Add a keyway derate (≈ 1.1–1.2×); under API 610 a shaft-deflection / stiffness limit usually governs instead
- Back-solve φₑ from the required suction specific speed (Eq. 50):
  - ΩSS = √ π φₑ(1 − rₛ²/rₑ² )/ (τ/2)^(3/4) — where τ  is selected via Table 1 (Gongwer; Stripling–Acosta for inducers) from prior Figure 25 inducer analysis
    - φₑ < 0.3 for NS  < 12,000
      - φₑ < 0.1 for inducer design
- Solve for eye radius (Eq. 49):
  - rₑ = [ Q / (π·Ω·φₑ·(1 − rₛ²/rₑ²)) ] ^(1/3)
- Back to Workflow

### Slide 11: b) Impeller Exit Radius
- Source: Karassik
- Back to Workflow

### Slide 12: c) Exit Width
- First, determine Exit Flow Coefficient using figure 12
- Next, apply the openness factor to correct for blockage:
  - ε ≈ 0.8–0.9 — accounts for blade thickness and boundary-layer buildup on the hub/shroud; higher ε for larger machines
- Determine exit width, b2
- Back to Workflow

### Slide 13: d) Hub, Shroud Profiles
- Match the meridional flow area at the blade leading edge to the eye area π(rₑ² − rₛ²) — or slightly larger for blade blockage — then grow it smoothly to the exit area 2πr₂b₂
- Set the shroud's minimum radius of curvature Rₛₕ ≈ half the eye's radial opening — limits the leading-edge velocity V₁,ₛₕ (design target V₁,ₛₕ/Vₑ ≈ 1.25); too sharp a turn raises NPSH₃%
- Shape the hub profile after the shroud, from the specified meridional area distribution — a radial-outflow hub should become essentially radial over its outer extent; adjust the shroud and repeat if not
- High-specific-speed, axial-flow, or inducer impellers: hub is often conical or reverse-curved (small radius at inlet, larger at outlet); shroud is often conical or cylindrical
- Back to Workflow
- Source: Karassik

### Slide 14: e) Blade Construction
- i. Leading/trailing edge loci — shroud LE at/near the eye plane (prevents separation); hub LE set back along the hub profile (avoids excessive twist); TE locus normally straight and axial, more radial at higher specific speed
- ii. Surfaces of revolution — construct blade coordinates on the hub, mean (rms streamline – Fig 14.: ψ = 0.5 – equal shroud/hub spacing), and shroud;
- iii. Inlet blade angles — set βb,1 ≈ flow angle βf,1 from the inlet velocity triangle (U1, Vm,1, any prewhirl Vu,1), plus a small allowance for blade thickness and off-design flow
- iv. Outlet blade angles — set from the required Vu,2, corrected for slip:
  - Pfleiderer's empirical method (Table 2  -assume vaned diffusers present); solved iteratively with blockage
- v. Number of blades — sized via solidity to limit blade loading:
  - σ = nb·ℓ/(2πr2): ~1.8 keeps diffusion factor D = 1 − W2/W1 + ΔWb/(2W1) below the 0.6 NACA loss-onset limit
- vi. Blade shape —conformal-transformation method (sketch smooth ‘grid-lines,’ transform to the physical surface); build on hub/mean/shroud, then add blade thickness
- Back to Workflow
- Source: Karassik
- 2= outlet
- 1 = inlet

### Slide 15: Collector Design (2.40 – 2.45)
- Collector is defined as effluent of impeller which converts velocity to static pressure while directing fluid to discharge piping.
  - Collector always consists of Volute (a), which expands the flowing fluid through increasing AT  - too much/little area causes excessive head losses; critical to stay near BEP
  - Within the pump casing, Vaned Diffusers (b) are often used to further aid this process especially for higher impeller speeds (>150 ft/s tip)
  - Return passages (c) are used for multi-stage pumps
- Back to Workflow

### Slide 16: Collector: Volutes
- Setup:
  - Volute cross-section is built outward from a "base circle" r₃ touching the tongue (cutwater), offset from the impeller exit r₂ by Gap B (≈4–15% of impeller radius — higher for volutes than diffusers, and for higher-energy pumps)
  - Area Aᵥ grows with angle θ from 0 at the tongue to Aₜ at the throat T, sized so rVᵤ = const around the periphery (Worster) — holds static pressure uniform at BEP
    - One-dimensionally rₜVₜ ≅ r₂Vᵤ,₂; enlarged slightly in practice to offset friction loss (Eq. 61): rₜVₜ ≅ (0.9–0.95)·r₂Vᵤ,₂
- Off-BEP the volute's casing line no longer matches the impeller's H-Q line at the throat, driving radial thrust — pressure rises tongue→throat below BEP (opposite above), then drops sharply back across the tongue
  - Large pumps: a double volute (two throats 180° apart, joined by a back channel) cancels radial thrust across the flow range
- To find acentric profile:
  - Aᵥ(θ): solve from rVᵤ = const, or use the simpler straight-line Aᵥ vs. θ — the extra area this adds near the tongue offsets the higher friction loss there
  - Cross-section transitions low-and-wide near the tongue (height ≪ b₃) to near-square at the throat (height ≈ bₘₐₓ); too low an aspect ratio raises loss. Throat to discharge: conical diffuser (~7° divergence, exit area up to 2×Aₜ) — collector pressure rise ≈ 20–25% of stage head
- Back to Workflow

### Slide 17: Collector: Vaned Diffusers
- Rotationally symmetric — unlike a volute, minimal radial thrust across the whole flow range, not just at BEP
- Preferred over a (rare) vaneless diffuser: shorter radial distance, can diffuse axially or inward, and exit flow angle α₂ is usually too small for stall-free vaneless diffusion anyway
- Similar to a multi-throat volute, but more prone to off-design instability if not shaped correctly; b₃ set slightly larger than b₂ to tolerate axial positioning tolerance
- Gap B (r₃ − r₂) acts as a short vaneless prediffuser — substantial pressure recovery happens before the throat (Station 4); throat area is larger than a volute’s, allowing more diffusion ahead of it (Eq. 62): rₜVₜ ≅ 0.8·r₂Vᵤ,₂
- Fully-vaned throat-to-exit channel does the bulk of the diffusion — sized to avoid stall: ~11° included angle, ℓ/w₁ ≈ 4, Aₑₓ/Aₜ ≈ 1.8
  - Constant-thickness (curved) vanes allow a smaller rₑₓ/r₃ than thicker “island” vanes, at some performance cost
- Vane count nv: use only a few more than impeller blades nb (nb rarely > 7); avoid nb − nv (or multiples, to 3rd order) = 0, 1, or — at low orders — 2, which excites blade-vane pressure pulses
- Back to Workflow

### Slide 18: Predicting Performance Curves (2.45 – 2.54)
- Two objectives: generate H, P curves at constant N (BEP → runout, shutoff); verify pump/system stability
- Two anchor points bound the curve: BEP (Table 3 efficiencies) and shutoff (Eq. 65–67); a non-recirculating branch connects them
- Two paths to get there:
  - Computational Math(1D/empirical) — builds directly on the impeller geometry from a)–e)
  - CFD — full viscous solve; required for the stall kink, recirculation shape, and NPSHr-Q
- Recommended workflow: finalize the design via Computational math, predict/validate the full curves via CFD
- Back to Workflow

### Slide 19: Computational Math: BEP Anchor
- Ideal (Euler) head ψi from the outlet velocity triangle (Blade Construction) isn't the real head — three component efficiencies convert it (Table 3)
  - ηHY (hydraulic): ηHY = ηI − ζc(ψi/2 + φi²/2ψi)
    - impeller loss ηI ≈ 0.90–0.95; collector loss ζc ≈ 0.2–0.3 (ψi/2 term predominates)
    - shortcut (Jekat): ηHY ≈ 1 − 0.8/[Q(gpm)]^(0.25) — works well at all specific speeds per practical experience
  - ηm (mechanical): driven by disk friction — ηm = 1 − (Cm/2)·ηp/(Ωs²ψ^(5/2))
    - Cm ≈ 0.085/(Ωrt,2²/ν)^(0.2) — typically Cm = 0.004 at Re = 4.3×10⁶
  - ηv (volumetric): ring/neck-ring leakage — ηv ≈ 1/(1 + 5[(δ/rR)(re/r2)²/(Ωs²ψ)])
    - clearance ratio δ/rR ≈ 0.001–0.002
- Real BEP values: H = ηHY·Hi,   P = ρgQH/(ηHY·ηm·ηv)
- Shortcut check: Anderson's overall-efficiency correlation (Fig. 10) as a first-pass cross-check without the full breakdown
- Back to Workflow

### Slide 20: Computational Math: Shape of the Curve
- Non-recirculating branch (Q slightly < QBEP → runout): re-run the velocity triangle at each Q holding the exit relative flow angle βf,2 fixed (slip velocity Vs locked from BEP)
  - → ideal H, P vs Q; apply the same Table 3 losses → real H-Q, P-Q
- Shutoff anchor (Q=0):
  - Hs/o = [kimp(Ut,2² − Uh,1²) + kex·U2²] / 2g — centrifugal term (kimp≈1) + recirculation “pitot” term (kex≈0.2±0.1, driven by Gap B = (r3−r2)/r2)
    - ψs/o typically exceeds ½ (Stepanoff: 0.585)
  - Shutoff power coefficient P̂s/o = Ps/o/(ρΩ³r2⁵) — Mockridge's correlation (Fig. 23): wider impellers (larger b2/D2) recirculate more → higher P̂s/o
- BEP + shutoff + non-recirculating branch shape → complete 1D-predicted H-Q, P-Q curve
- Convergence (closes workflow step 7): predicted H at BEP vs. target H — mismatch adjusts φe/ψ (BEP head level), blade angle/slip (Vu,2), or b2 (flow coefficient) → back to a)–e)
- Limit: doesn't reliably capture the recirculation-driven kink near shutoff on high-σ curves, and gives no NPSHr-vs-Q
- Back to Workflow

### Slide 21: CFD: Purpose and Method
- Two uses: fast steady-state sweeps during design iteration vs. high-accuracy customer-facing curves
- All CFD solves RANS — impeller in the rotating frame (centrifugal + Coriolis terms), volute/diffuser stationary (Ω=0); turbulence closure via eddy-viscosity models
- Accuracy hinges on how the rotor–stator interface (impeller ↔ volute/diffuser) is handled:
  - Circumferential averaging / mixing-plane — cheapest, accurate near BEP only
  - Frozen-rotor — steady, ~5% accuracy from 80–120% BEP (per cited case)
  - Full unsteady — most expensive; needed to capture shutoff, recirculation, stall kink
- Workflow mirrors Computational math: iterate geometry with fast steady CFD each pass, finalize with unsteady CFD
- Back to Workflow

### Slide 22: CFD: NPSHr via Cavitation Modeling
- NPSHr-vs-Q is the one curve Computational math (Table 1 / Nss sizing) can't directly produce across the full flow range
- Requires a two-phase model layered on the RANS solve: volume-of-fluid (VOF) + Rayleigh–Plesset bubble growth + non-condensable gas accounting; thermal equilibrium assumed
- Validated case: boiler feed pump impeller — CFD cavity length & H-vs-NPSH curve matched test closely across σ = 2gNPSH/Ue² = 0.65 (near inception) down to 0.20 (3% head break-off)
- Same approach applies to inducers (head-vs-Nss at the design point)
- Back to Workflow

### Slide 23: Predicting Axial Thrust (2.51–2.54)
- Net force arises because the back shroud of a closed impeller runs near discharge pressure over its full area while the front (eye) side sees only suction pressure — net axial force pushes the impeller toward suction
  - Sidewall-gap fluid spins at Vu ≈ Ωr/2 (no-leakage case); this swirl sets up a centrifugal pressure drop from impeller OD down to the wear-ring seal, so the loaded pressure profile isn't flat (Table 4)
  - More inflow leakage → more swirl → steeper OD-to-ring pressure drop; back-side outflow (multistage crossover) enters the gap at small radius with little swirl, so its pressure stays closer to OD pressure — net effect is more thrust toward suction than the pressure-loaded areas alone suggest
- Quick estimate, linearized pressure distribution (Table 5):
  - T ≈ (π/4)(D2² − DR²)(p2 − ps) − ρQVz,1
    - DR = wear-ring (seal) diameter, p2 = impeller-OD static pressure (≈75–80% of stage Δp); momentum term ρQVz,1 small for radial impellers, grows for mixed-flow
- Ring wear over pump life increases clearance → increases leakage → increases net T; unequal front/back ring wear makes even a nominally “balanced” double-suction impeller's thrust uncertain
- Off-BEP below QDR, diffuser/volute backflow invades the sidewall gaps and cancels or reverses gap swirl → large, sometimes side-switching thrust excursions — this recirculation-driven thrust instability, not H-Q curve shape, is the real axial stability risk
- Back to Workflow

### Slide 24: Axial Thrust Balancing: Two Mechanisms
- Single-stage closed impellers cut the net thrust predicted above with one of two mechanisms — both work by lowering back-shroud pressure rather than sizing up the thrust bearing
- Balancing holes + rear wear ring
  - A second wear ring is added on the back shroud (mirroring the front/eye ring); holes drilled through the shroud inside that ring connect the back sidewall gap directly to the low-pressure eye
  - Leaks the high back-shroud pressure forward to suction, cutting the pressure-loaded back area down to the ring diameter — largely cancels the imbalance
    - Cost: adds a parallel leakage circuit → directly reduces ηv (slide 19) since the recirculated flow does no useful work
- Pump-out (back) vanes
  - Radial ribs on the back shroud spin the sidewall-gap fluid up toward full impeller speed (Vu → Ωr) instead of the natural ≈Ωr/2
  - Higher swirl → steeper centrifugal pressure drop from OD to hub → lowers back-shroud pressure without an added through-hole leak path
    - Cost: parasitic disk-friction power (adds to Cm, slide 19) instead of a volumetric loss — trades ηv for ηm
- Balancing holes are simpler/cheaper and field-serviceable but bleed ηv; pump-out vanes avoid the leak path and clogging risk but cost more in ηm — high-energy single-stage pumps often use both together
- Balancing drums/disks solve the equivalent problem for multistage rotors (Section 2.2) — out of scope per slide 2's single-stage limit
- Back to Workflow

### Slide 25: Table 1: NPSHR Correlations
- Used as part of
- Cavitation Check (NSS)
- a) Impeller Eye Radius

### Slide 26: Table 1: NPSHᵣ — Symbol Glossary
- τ  —  cavitation (Thoma) parameter = NPSH / (Ue²/2g)
- Ωss  —  dimensionless suction specific speed
- NPSH, NPSH3%  —  suction margin; the value at 3% head break-off (the "required" NPSH)
- Ue / Ve  —  impeller-eye peripheral speed / eye through-flow (axial) velocity
- φe  —  eye flow coefficient = Ve/Ue  (printed as δe in the scanned table)
- rs, re  —  shaft radius and impeller-eye radius
- k1, k2  —  Gongwer constants: 1.4 / 0.085 (large pumps), 1.69 / 0.102 (typical pumps)
- V1,sh, W1,sh  —  absolute and relative inlet velocity on the shroud streamline
- Vθ,1  —  inlet tangential velocity (prewhirl); the correlations assume Vθ,1 = 0
- n  —  velocity-ratio exponent in the Gongwer form
- U1,1 ≈ Ue  —  blade speed at the shroud inlet
- φs, βb,1,sh  —  inducer inlet flow coefficient and inducer blade angle at the shroud (part b)
- Symbols as they appear in Table 1 (previous slide).

### Slide 27: Table 2: Pfleiderer’s slip formula
- Used as part of e) Blade Construction

### Slide 28: Table 2: Pfleiderer’s Slip Formula — Symbol Glossary
- Vs  —  slip velocity = p·Vθ,2
- Vθ,2  —  actual (finite-blade) exit tangential velocity
- Vθ,∞,2  —  ideal exit tangential velocity for infinitely many blades
- p  —  Pfleiderer slip factor = ψ′ r2² / ∫ nb r dm
- ψ′  —  Pfleiderer coefficient = a·(1 + sin βb,2)
- a  —  vane-system constant: 0.6 vaned diffuser; 0.65–0.85 volute; 0.85–1.0 vaneless diffuser
- βb,2  —  impeller exit blade (metal) angle
- nb  —  number of impeller blades
- r1, r2  —  blade inlet and exit radii
- r, m  —  radial and meridional coordinates along the blade (dm = dr in the worked example)
- U2  —  impeller exit (tip) speed
- μ  —  slip coefficient = Vs/U2 = p·Vθ,2/U2
- Symbols as they appear in Table 2 (previous slide).

### Slide 29: Table 3: Component Efficiency Expressions
- Source: Karassik
- Back to Workflow

### Slide 30: Table 3: Component Efficiency — Symbol Glossary
- Hydraulic efficiency
- ηHY  —  hydraulic efficiency = 1 − ΣLi / Δ(U Vθ)
- ηI  —  impeller hydraulic efficiency ≈ 0.90–0.95
- ζc  —  collector loss coefficient — fraction of V2²/2 not converted to static pressure (≈ 0.2–0.3)
- ΣLi = Limp + Lc  —  total loss = impeller loss + collector loss
- Δ(U Vθ)  —  Euler specific work across the impeller
- ψi, ψi,2  —  ideal (Euler) head coefficient = Vθ,2 / U2
- φi, φi,2  —  ideal flow coefficient = Vm,2 / U2
- V2  —  absolute exit velocity; Vθ,2, Vm,2 are its tangential and meridional parts
- U2  —  impeller exit (tip) speed
- Q  —  flow rate (gpm in shortcut b, m³/s in the SI form)
- Limp  —  deeper impeller-loss model = k·W1²/2 + f·(W̄²/2)·(ℓ/Dh)
- k, f  —  incidence (shock) loss coefficient; pipe-type friction factor
- ℓ, Dh  —  passage length; passage hydraulic diameter
- W1  —  relative velocity just upstream of the blades (rms streamline)
- W̄²  —  mean-square relative velocity along the passage
- ε  —  surface roughness (assumed size-independent in shortcut b)
- Mechanical efficiency
- ηm  —  mechanical efficiency = 1 − (PDF + PB&S) / Ps
- Ps  —  shaft (input) power
- PDF  —  disk-friction power = (Cm/2)·ρΩ³rt,2⁵
- PB&S  —  bearing & seal power (usually the smaller loss)
- Cm  —  two-sided disk-friction coeff. ≈ 0.085 / (Ω rt,2²/ν)0.2; ≈ 0.004 at Re = 4.3×10⁶
- Ω, Ωs  —  angular velocity; dimensionless specific speed
- rt,2  —  impeller tip radius
- ν, Re  —  kinematic viscosity; rotational Reynolds number
- ρ, g, ΔH  —  fluid density; gravity; head rise
- ψ  —  head coefficient
- Qs  —  dimensionless flow = Q / (Ω rt,2³) = Ωs² ψ3/2
- ηp  —  overall pump efficiency (appears in the shaft-power relation)
- Volumetric efficiency
- ηv  —  volumetric efficiency = Q / (Q + QL)
- QL  —  ring / neck-ring leakage flow
- δ, rR  —  wear-ring radial clearance and radius; δ/rR ≈ 0.001–0.002
- re, r2  —  impeller eye and exit radii
- factor 5 → 10  —  when leakage occurs across both the front and back rings
- Symbols as they appear in Table 3 (previous slide).

### Slide 31: Table 4: Predicting Axial Thrust
- Back to Predicting Axial Thrust

### Slide 32: Table 4: Leakage Effects on Axial Thrust — Symbol Glossary
- T  —  net axial thrust = (TB − TF)·ηstgs − Tslv
- TB, TF  —  back-shroud and front-shroud pressure forces
- Tslv, ηstgs  —  shaft-sleeve thrust; number of stages
- T = ∫ 2πr·p dr  —  pressure force integrated over a shroud face
- p, p2  —  local sidewall-gap pressure; impeller-OD pressure
- po, pi  —  gap pressure at the outer / inner radius
- r, ro, ri  —  gap radius and its outer / inner limits
- Vθ,gap  —  gap swirl velocity (Ωr/2 with zero leakage → Ωr at full wheel speed)
- Ω, ρ  —  angular velocity; fluid density
- Φlkg  —  leakage coefficient = Qleakage / (Ω r2³)
- Qleakage  —  sidewall-gap leakage flow = f(ℓ, δ, Ω, ν, Δpring)
- finflow, foutflow  —  gap-swirl vs. radius functions for inflow / outflow leakage
- fwidth  —  gap-width factor = (√(A²+A) − A)/0.5,  with A = 1/(5 s/r2)
- s, Δpring  —  axial gap width; pressure drop across the ring
- ℓ, δ, ν  —  leakage-path length; radial clearance; kinematic viscosity
- Symbols as they appear in Table 4 (previous slide).

### Slide 33: Table 5: Approximate Axial Thrust Calculation
- Back to Predicting Axial Thrust

### Slide 34: Table 5: Approximate Axial Thrust — Symbol Glossary
- THRUST  —  F7 + F6 + F5 + F4 − F3 − F2 − F1 − FM,I + FM,II
- F1 … F7  —  axial pressure force on each impeller surface band (1 = inner … 7 = outer)
- pj  —  pressure acting on band j
- rj,i, rj,o  —  inner and outer radius of band j
- Fj,const  —  uniform-pressure force = pj·π(rj,o² − rj,i²)
- Fj,var  —  linear-p(r) correction = ⅓π rj,o² [2 − rj,i/rj,o − (rj,i/rj,o)²]·(pj,o − pj,i)
- pj,o, pj,i  —  pressure at the outer / inner edge of band j
- FM,I, FM,II  —  momentum-flux forces in / out = ρ Q Vz,I  and  ρ Q Vz,II
- Vz,I, Vz,II  —  axial velocity of the flow entering / leaving
- Q, ρ  —  flow rate; fluid density
- po  —  reference (suction) pressure on the sketch
- Symbols as they appear in Table 5 (previous slide).

### Slide 35: Variable Glossary (1 of 2): Duty, Geometry & Kinematics
- Duty & speed
- Q  —  volumetric flow rate (capacity); gpm or m³/s
- H  —  total head developed by the pump; ft or m
- T  —  process fluid temperature (T also = net axial thrust on Slides 23–24 / Tables 4–5)
- N  —  impeller rotative speed; rpm
- Ω  —  impeller angular velocity; rad/s (= 2πN/60)
- f  —  AC line frequency (60 Hz in the US)
- #Poles  —  motor pole count (with f, sets N)
- NS  —  specific speed, US dimensional form = N·√Q / H3/4
- Ωs  —  specific speed, dimensionless ("universal") form
- BEP  —  best efficiency point; QBEP = design flow
- shutoff / runout  —  zero-flow (Q = 0) and maximum-flow ends of the curve
- NPSH & cavitation
- NPSHa  —  net positive suction head available (set by the system)
- NPSHr  —  NPSH required by the pump — the 3% head-drop value (NPSH3%)
- Hs  —  static suction head
- Hhs  —  suction-vessel head-space (gas) pressure head
- Hf  —  suction-line friction head loss
- Hvp  —  fluid vapor-pressure head
- Nss  —  suction specific speed = N·√Q / NPSHr3/4
- ΩSS  —  suction specific speed, dimensionless form
- τ  —  cavitation (Thoma) parameter = NPSH / (Ue²/2g); picked from Table 1
- σ  —  cavitation number = 2g·NPSH / Ue² (Slide 22) — distinct from blade solidity σ
- Impeller geometry
- rs  —  shaft radius (= 0 for an overhung impeller)
- Ss  —  allowable shaft shear stress
- M  —  shaft torque = P / Ω
- re  —  impeller eye (inlet) radius
- Ve  —  eye through-flow (axial) velocity
- Ue  —  eye peripheral speed
- φe  —  eye flow coefficient = Ve / Ue (< 0.3 typical; < 0.1 with an inducer)
- r2  —  impeller exit (OD) radius; D2 = exit diameter
- b2  —  impeller exit (discharge) width
- r1  —  blade leading-edge (inlet) radius
- r3  —  volute base-circle / diffuser-inlet radius
- rt  —  volute or diffuser throat radius
- ε  —  openness (blockage) factor on exit width ≈ 0.8–0.9
- Rsh  —  shroud minimum radius of curvature
- hub / shroud  —  impeller drive-side and eye-side walls
- Velocity triangles  (1 = inlet, 2 = outlet)
- U  —  blade peripheral speed (U1, U2; Ut,2 tip, Uh,1 hub-inlet)
- V  —  absolute fluid velocity; Vm meridional, Vu or Vθ tangential
- W  —  fluid velocity relative to the blade (W1, W2, W1,sh)
- Vu,1  —  inlet prewhirl (tangential component ahead of the blade)
- βf / βb  —  flow angle / blade (metal) angle, at inlet and outlet
- α2  —  absolute flow angle leaving the impeller into the collector
- Vs  —  slip velocity = Vθ,∞,2 − Vθ,2
- μ  —  slip coefficient = Vs / U2
- p  —  Pfleiderer slip factor (Table 2)
- Blades & passage
- nb / nv  —  number of impeller blades / diffuser vanes
- ℓ  —  blade chord / passage streamline length
- σ  —  solidity = nb·ℓ / (2πr2); ≈ 1.8 target
- D  —  diffusion factor = 1 − W2/W1 + ΔWb/(2W1); keep < 0.6
- ΔWb  —  blade-to-blade (loading) velocity difference
- ψ  —  rms-streamline parameter (0.5 = equal hub/shroud spacing); also head coefficient
- Dh  —  passage hydraulic diameter
- Every variable used across the deck (1 of 2). See also Tables 1–5 symbol glossaries.

### Slide 36: Variable Glossary (2 of 2): Collector, Performance, Losses & Thrust
- Collector
- collector  —  volute + optional vaned diffuser; converts velocity head to static pressure
- volute  —  single spiral collecting passage (always present)
- vaned diffuser  —  ring of vanes in the casing; added at high tip speed (> ~150 ft/s)
- return passage  —  crossover to the next stage (multistage only)
- Gap B  —  radial gap, impeller OD → collector = (r3 − r2) / r2
- θ  —  volute wrap angle (0 at the tongue → 360° at the throat)
- tongue / cutwater  —  the volute lip that splits the flow
- Av(θ)  —  volute cross-sectional area vs. wrap angle
- AT / Aex  —  volute or diffuser throat area / collector exit area
- r·Vu = const  —  Worster free-vortex rule for sizing Av(θ)
- Vt  —  throat velocity; rtVt ≅ (0.8–0.95)·r2Vu,2
- b3 / bmax  —  collector inlet width / maximum section height
- Station 4  —  diffuser throat station
- double volute  —  twin throats 180° apart; cancels radial thrust across the flow range
- Performance-curve prediction
- H–Q, P–Q  —  head- and power-vs-flow curves at constant N
- ψi  —  ideal (Euler) head coefficient from the outlet velocity triangle
- Hi  —  ideal (Euler) head; real H = ηHY·Hi
- φi  —  ideal flow coefficient = Vm,2 / U2
- non-recirc. branch  —  BEP→runout curve from repeated velocity triangles (βf,2 fixed, Vs locked)
- Hs/o  —  shutoff (Q = 0) head
- ψs/o  —  shutoff head coefficient (> ½; Stepanoff ≈ 0.585)
- kimp  —  centrifugal-term coefficient in Hs/o (≈ 1)
- kex  —  recirculation "pitot"-term coefficient (≈ 0.2 ± 0.1), driven by Gap B
- Ut,2, Uh,1  —  impeller-tip and hub-inlet peripheral speeds
- P̂s/o  —  shutoff power coefficient = Ps/o / (ρΩ³r2⁵) (Mockridge, Fig. 23)
- RANS  —  Reynolds-averaged Navier–Stokes (the CFD equation set)
- frozen-rotor / mixing-plane  —  rotor–stator interface treatments in CFD
- Component efficiencies  (Table 3)
- ηp  —  overall pump efficiency = ηHY·ηm·ηv
- ηHY  —  hydraulic efficiency (real head ÷ Euler head)
- ηI  —  impeller hydraulic efficiency ≈ 0.90–0.95
- ζc  —  collector loss coefficient — fraction of V2²/2 not recovered (≈ 0.2–0.3)
- ηm  —  mechanical efficiency (set mainly by disk friction)
- Cm  —  disk-friction torque coefficient ≈ 0.004 at Re ≈ 4.3×10⁶
- ηv  —  volumetric efficiency = Q / (Q + QL)
- QL  —  internal (wear-ring) leakage flow
- δ, rR  —  wear-ring radial clearance and radius; δ/rR ≈ 0.001–0.002
- Limp, Lc, ΣLi  —  impeller, collector, and total hydraulic losses
- Δ(U Vθ)  —  Euler specific work across the impeller
- Ps, PDF, PB&S  —  shaft, disk-friction, and bearing & seal power
- ν, Re  —  kinematic viscosity; Reynolds number
- ρ, g  —  fluid density; gravitational acceleration
- Axial thrust  (Slides 23–24, Tables 4–5)
- T  —  net axial thrust force (pushes the impeller toward suction)
- p2  —  impeller-OD static pressure ≈ 75–80% of stage Δp
- ps, Δp  —  suction pressure; stage differential pressure
- DR  —  wear-ring (seal) diameter
- Vθ,gap  —  swirl velocity of sidewall-gap fluid (≈ Ωr/2 with no leakage)
- Φlkg  —  leakage coefficient = Qleakage / (Ω r2³)
- Qleakage  —  sidewall-gap leakage flow
- QDR  —  flow below which diffuser/volute backflow invades the gaps
- finflow, foutflow, fwidth  —  Table 4 gap-swirl correction functions
- F1…F7  —  axial pressure force on each impeller surface band (Table 5)
- Fj,const, Fj,var  —  uniform-pressure and linear-pressure parts of Fj
- FM,I, FM,II  —  momentum-flux forces in / out = ρQVz,I, ρQVz,II
- Vz,1  —  inlet axial velocity (momentum term ρQVz,1)
- balancing holes + rear ring  —  bleed back-shroud pressure to the eye (costs ηv)
- pump-out (back) vanes  —  spin the back gap up to Ωr to cut back-shroud pressure (costs ηm)
- balancing drum / disk  —  multistage thrust balance (out of scope)
- Every variable used across the deck (2 of 2). See also Tables 1–5 symbol glossaries.

### Slide 37: References
- Sources: Pump Handbook – Chapter 2.1.1 (Design Procedure)
