# Apollo Root Cause Methodology

Four-step Apollo RCA: problem definition, reality chart, effective solutions, implement and track.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/apollo-rca/
- **Download the .pptx (258 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Apollo-Root-Cause-Methodology.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 13

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Apollo Root Cause Analysis Methodology
- Joshua Sharpes

### Slide 2: Contents
- Step 1: Define the Problem
- Step 2: Create a Reality Chart
- Step 3: Identify Effective Solutions
- Step 4: Implement and Track Solutions

### Slide 3: Glossary
- Primary Effect: the problem you want to prevent from recurring; the first point on the Reality Chart (Step 1 "What")
  - Event-based Problems: a specific occurrence with a definable when and where, e.g. an incident, release or equipment failure
  - Rule-based Problems:
- Action: a momentary cause, the trigger, that acts on an existing condition to produce the effect
- Condition: a cause that exists over time (design, state, environment) and must be present for an action to cause the effect
- Cause: an action or condition that exists in the same time and space as the effect; every effect has at least one of each (2nd and 4th C&E principles)
- Evidence: sensed or inferred information that validates a causal relationship; intuition and emotion are not evidence

### Slide 4: Step 1: Define the Problem
- This includes 4 main components:
  - What: this is the primary effect – the first point on the reality chart map
  - When: this is the time and date primary effect took place
    - Relative timing of causes and conditions
  - Where: location of primary effect
  - Significance: why this problem matters; how is the primary effect impactful to the organization?
    - Can be in terms of health, revenue, liability, safety, environment, etc.
- Step 1: Define the Problem

### Slide 5: C&E Principles (Chapter 3)
- First: Cause & effects are the same
  - The continuum can be reversed; fear of tomorrow can cause the events of today
- Second: Each effect has at least two causes in the form of actions and conditions
  - An action cause can not occur without a condition cause & vice versa
- Third: Causes & effects are part of an infinite continuum of causes
  - since the continuum of cause/effect expands infinitely, the starting point is only relative:
    - Why am I so happy today?  Big bang theory billion of years ago
    - What will happen if I stop going to the park?  altered university entropy in 1000 years
- Fourth: an effect exists only if the causes exist in the same space and time frame
  - Yesterday’s cause is today’s effect for today’s cause
- Step 1: Define the Problem

### Slide 6: Cause & Effect Applications
- This lineage of causation is applicable to more than just Apollo RCA:
  - Fault Tree Analysis (FTA) uses C&E to generate logic diagrams for explanations of top events (consequences)
  - FMEA (Failure and Effect Mode Analysis) uses C&E to list failure modes of equipment
  - LOPA (Layer of Protection Analysis) uses C&E to tie initiating events to consequences
- Many Hazard Evaluation Procedures employ this technique:
  - C&E is critical for both safety investigations and analysis
- Step 1: Define the Problem

### Slide 7: Step 2: Create a Reality Chart
- Step 2: Create a Reality Chart
- Build left to right. Validate each proposed causal relationship before extending the chart.
- PRIMARY EFFECT
- The problem to prevent from recurring
- PROPOSED CAUSES
- Identify the action + condition
- SUBSEQUENT CAUSES
- Ask “why?” and extend one layer
- CAUSE PATH ENDING
- Stop when an ending criterion is met
- NOTE SOLUTIONS
- Capture options at path endings
- WHY?
- WHY?
- WHY?
- THEN
- EVIDENCE
- Sensed or inferred information that validates this link
- EVIDENCE
- Sensed or inferred information that validates this link
- • More info needed
- • Desired condition
- • Don’t have control
- • New primary effect
- • More productive cause path
- OUTPUT
- Specific solution ideas tied to the path ending
- PLACE EVIDENCE DIRECTLY UNDER EACH CAUSE LAYER
- ACTION + CONDITION causes must exist in the same time and space as the effect.
- Build left to right. Validate each proposed causal relationship before extending the chart.
- PRIMARY EFFECT
- The problem to prevent from recurring
- PROPOSED CAUSES
- Identify the action + condition
- SUBSEQUENT CAUSES
- Ask “why?” and extend one layer
- CAUSE PATH ENDING
- Stop when an ending criterion is met
- NOTE SOLUTIONS
- Capture options at path endings
- WHY?
- WHY?
- WHY?
- THEN
- EVIDENCE
- Sensed or inferred information that validates this link
- EVIDENCE
- Sensed or inferred information that validates this link
- • More info needed
- • Desired condition
- • Don’t have control
- • New primary effect
- • More productive cause path
- OUTPUT
- Specific solution ideas tied to the path ending
- PLACE EVIDENCE DIRECTLY UNDER EACH CAUSE LAYER
- ACTION + CONDITION causes must exist in the same time and space as the effect.

### Slide 8: Step 2: Create a Reality Chart - Causes
- Causes are both action and conditions which interact with each other
- Identifying an action or a condition as a cause by concluding:
  - Same time frame as effect
  - Interaction relevance with effect
    - This requires listing all potential causes and ranking them according to relevance
- Step 2: Create a Reality Chart

### Slide 9: Step 2: Create a Reality Chart - Evidence
- Acceptable Evidence Types:
  - Sensed: directly perceived by observer
  - Inferred: known by repeatable causal relationships, should always be verified
- Non-acceptable, but potentially useful evidence
  - Intuitive and Emotional evidence should never be directly used to verify anything. However, these can be used to lead to acceptable evidence types through further investigation
- The purpose of evidence is to validate that causes are indeed related to the effect through a causal relationship
- Step 2: Create a Reality Chart

### Slide 10: Reality Chart Example: Sulfuric Acid Tank Explosion
- PRIMARY EFFECT
- Acid tank thrown 15 m (50 ft) through the building roof
- Sensed: tank found on open ground nearby
- ACTION
- Hydrogen ignited in the tank vapor space
- CONDITION
- Tank split at the base/wall weld, not the roof seam
- Sensed: failure at base weld
- ACTION
- Welders working nearby supplied the ignition source
- CONDITION
- Hydrogen accumulated under the conical roof
- CONDITION
- Roof/wall weld stronger than usual: explosion not foreseen in design
- CONDITION
- Slight corrosion of the tank by acid produced H₂
- Inferred: acid + steel → H₂
- CONDITION
- No vent; only an overflow pipe down to grade
- SOLUTION
- Hot-work permit with gas test of nearby vapor spaces
- CAUSE PATH ENDING
- Desired condition: tank is in acid service
- SOLUTION
- Vent at the highest point (Kletz Fig. 16-1)
- SOLUTION
- Make the roof-to-shell seam the weak point (frangible roof)
- Read left to right, asking "why?" at each box: every effect has an action (orange) and a condition (blue). Each path stops at a cause path ending; solutions target the systemic conditions rather than the incidental action.
- Incident: T. Kletz, What Went Wrong? 5th ed., §16.2(a).
- Step 2: Create a Reality Chart

### Slide 11: Step 3: Identify Effective Solutions
- An effective solution is a solution that meets the solution criteria:
  - Prevent recurrence; this is effectiveness
  - Be within your control; this is practicality
  - Meet your goals and objectives; this is completeness
  - Not cause other problems; this is non-mitigative
- The best solutions are often applied to conditional causes since action causes are often incidental (more unpredictable)
  - Conditional causes can often be addressed with systemic solutions
- Solutions should be specific actions
  - Not performed in the future
  - Not redundant of past actions
- Step 3: Identify Effective Solutions

### Slide 12: Methods to Improve Solutions
- Be Creative
  - Solutions are often not obvious: this requires nontraditional thinking
- Improve Your Thinking
  - Conventional wisdom limits creative thinking
  - Arrogance is blinding - test your own knowledge
  - Admit “I do not know” when thought process has stalled.
    - Recalibrate with new approach
  - Start with extreme solution and downsize it until it is practical
- Tapping Available Resources
  - Use group synergy – encourage crazy ideas, allowing people to elaborate
- Using Our Brains
  - Sleep on the problem, this allows the subconscious brain to work
- Step 3: Identify Effective Solutions

### Slide 13: Step 4: Implement and Track Solutions
- Utilizing periodic reviews, solution progress should be tracked.
- Track profitability of result, this impacts future decision making, including more Apollo Root Cause
- Step 4: Implement and Track Solutions
