# Equilibria Approach Selection

Decision workflow for selecting a thermodynamic property method -- Classical (gamma-phi), EOS (phi-phi), or Hybrid -- gated on electrolyte presence, liquid-phase ideality (UNIFAC), and pressure vs ~10 bar. Validated against 11 real petrochemical process families from the Meyers Handbook.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/eos-selection/
- **Download the .pptx (0 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Equilibria-Approach-Selection.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 11

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Equilibria Approach Selection
- Joshua Sharpes

### Slide 2: Sources
- Properties of Gases and Liquids – Poling
- Don’t Gamble With Physical Properties for Simulations – Eric Carlon

### Slide 3: Scope
- Model chemical production process unit operations containing vapor and liquid phases
  - Operating conditions limited from cryogenic to supercritical
- Solutions contain multiple components w/ variety of molecular integrations. Therefore, for simplicity:
  - Pseudo-component modeling is deferred to EOS selection – need raw components of mixture for approach selection
  - Neglect Solids

### Slide 4: Background: Equilibria Approaches
- Two approaches exist: Classical (Gamma-Phi) and EOS (phi-phi)
  - Classical Approach utilizes activity coefficients to model highly non-ideal liquids while comparing vapor phases to ideal gases through departure functions:
    - Best for:
      - Non-ideal liquid solutions: electrolytes, polar fluids, azeotropes
      - Low Pressure Vapors
  - EOS Approach uses selected equation that assumes vapor, liquid phases are a function of system properties
    - This presentation covers this approach
    - The equation selection is based on fluid properties, but iteration within the EOS does not directly account for changes in fluid properties
    - Best for:
      - Pseudo-Ideal Liquids
      - High Pressure Vapors
  - In rare cases, methods from both will needed w/ Hybrid Approach
    - highly non-ideal liquid (Classical) AND high pressure vapor (EOS)

### Slide 5: Approach Selection Considerations
- Electrolytes [E]:
  - Electrolytes always require a Classical Approach; Ionic bonds are the strongest
- Liquid Phase Ideality [I]:
  - Impactful bonds such as H-Bonding, Charge Transfer , and Lewis Acid/Base all lead to γ deviation
    - More ideal favors EOS, Less ideal favors Classical/Hybrid
- Pressure [P]:
  - Only Classical approach is pressure-sensitive; EOS covers all pressure ranges

### Slide 6: Approach Selection Workflow
- Eliminate non-applicable substances:
  - Pseudocomponents  Relegate to Chao-Seader / Grayson-Streed / Braun K-10 packages  (outside of this workflow
  - Solids
- Evaluate Electrolytes:
  - Qualitative: Solute/Solvent Pairing Identification
  - Quantitative (PubChem): Dielectric Constants, Donor Numbers, pKa values
- Evaluate Liquid Non-ideality
  - Run UNIFAC to evaluate Polarity, H-bonding, and MW-size mismatching
  - Charge Transfer Complexation: qualitative (PubChem), quantitative (Kamleft-taft)
  - Lewis/Acid Base Pairing: qualitative (HSAB), quantitative (DN, AN)
- Evaluate Pressure (>10 bar)

### Slide 7: Approach Selection: Electrolytes [E]
- Qualitative Screen:
  - Identifies components as acids, bases, and salts through PubChem
    - Obtains CAS number, molecular structure, and SMILES structure
    - Runs returned name against known chemical family list
    - Identifies end-group pka values
- Quantitate Analysis:
  - DN-Veto + pka:
    - pKa and dielectric constants pulled for components
    - Thresholds for significant dielectric constants are modified by Gutmann donor number (DN) and bulky ion presence
    - Thresholds are vetoed if they are mischaracterized in the context of the solution (a solvent misclassified as solute, visa versa)
- Entire workflow: Electrolyte Identification - Screening Methodology.pdf

### Slide 8: Approach Selection: Liquid Phase Ideality [I]
- Molecular interactions worth consideration:
  - Polarity: evaluate quantitively w/ UNIFAC (Dortmund)*
  - H-Bonding: evaluate quantitively w/ UNIFAC (Dortmund)*
  - Charge Transfer Complexation :
    - evaluate qualitatively w/ end-group identification (PUBCHEM from Electrolytes but w/ SMARTS pattern)
    - then proceed to quantification w/ Kamlet-Taft
  - Lewis Acid/Base Pairing:
    - evaluate qualitatively w/ Hard-Soft Acid Base Theory (HSAB),
    - then proceed to quantification w/ Gutmann Donor Number (DN) & Acceptor Number (AN)
  - MW Size-Mismatch: evaluate quantitatively w/ UNIFAC (Dortmund) **
- Solution can have different bonds and thus competing gamma results:
  - Likewise results should be additive (deviation in the same direction)
  - Competing results should prompt gamma evaluation through entire operating composition range
- Bonds not considered:
  - Metallic: Liquid-metal is outside this scope
  - Covalent: covalent is
  - Dispersion Forces
- *Reactive Groups w/ no UNIFAC Data (e.g. HCl, Cl2): use KT + DN/AN. Can get preliminary UNIFAC estimates by removing inert species
- ** Reactive Groups w/ no UNIFAC Data: Flory-Huggins Molar Volume Ratios

### Slide 9: Approach Selection: Pressure [P]
- Low Pressure (<10 bar) systems assume ideal vapor  Classical Approach is best since no vapor consideration
- High Pressure (>10 bar) systems cannot assume ideal vapor  Hybrid approach required

### Slide 10: Approach Selection: Established Workflow

### Slide 11: (no text)
