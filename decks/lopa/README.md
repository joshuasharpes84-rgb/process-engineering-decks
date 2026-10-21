# Layer of Protection Analysis

LOPA methodology: initiating event frequency, independent protection layers, enabling conditions/conditional modifiers, and target mitigated risk.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/lopa/
- **Download the .pptx (507 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Layer-of-Protection-Analysis.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 53

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Layer of Protection Analysis
- Joshua Sharpes
- Source: Layers of Protection Analysis Simplified Risk Assessment CCPS

### Slide 2: Audience
- For understanding of this presentation, viewers should have moderate familiarity with:
  - Chemical Plant operations
    - Equipment, instrumentation/controls, personal
  - PSM purposes
    - Process safety risk
- …and light familiarity with:
  - Engineering protection layers
  - LOC scenarios

### Slide 3: Chapters
- Introduction
- Overview of LOPA
- Estimating Consequence Severity
- Developing Scenarios
- Identifying Initiating Event Frequency
- Identifying Independent Protection Layers
- Determining the Frequency of Scenarios
- Using LOPA to Make Risk Decisions
- Implementing LOPA
- Using LOPA for Other Applications
- Advanced LOPA Topics

### Slide 4: Glossary (High Level)
- Scenario: cause-consequence pairing
  - Cause/Initiating Event: event that leads to the undesired consequence
  - Consequence: measure of the expected effects of a loss event in terms of personnel impact, environmental damage, and loss of business.
    - This is triple bottom line – people, planet, profit.
    - Loss Event: event that can lead to consequence if not addressed w/ mitigative safeguard
- Probability of Failure on Demand (PFD): likelihood of device/method failing when dependent upon.
- Frequency: number of events occurring/yr
  - Applied for Initiating Event, Consequence components
- Risk Reduction Gap: the difference between tolerable risk and actual risk of scenario
  - Risk Reduction Factor (RRF): IPL factor that serves as credit to close this gap

> Speaker notes: Ipl definition needed in addition to other terms more frequently mentioned

### Slide 5: Introduction – Chapter 1
- Back to Table Contents

### Slide 6: History of LOPA (1.2)
- American Chemistry Council published Responsible Care Process Safety Code of Management Practices the late 80s in effort to formalize practice for evaluating safeguards
- CCPS Standards were developed in the late 90s which began to
  - Develop semi-quantitative tool for industry use
  - Establish Safety Instrumented Function (SIF) classification for Safety Integrity Level (SIL) determination
  - Reduce scenarios that would need QRA
- ISA (US) and IEC (International) standards were being developed simultaneously for exact SIL calculation based on SIF classification
  - These standards are what is used today
- Up until these developments, plants would implement informal or formal, but inconsistent, methods for closing their risk reduction gaps which resulted in over-reliance on the process design phase outcomes

### Slide 7: Use of LOPA in the Process Life Cycle (1.3)
- Design phase during drafting PFDs/P&IDs
  - Can be used to modify inherently safer design (ISD)
- Modifications to an Existing Process throughout lifecycle
- Identification of safety critical equipment that require periodic testing and maintenance
- Determination of acceptable risk
- Operator actions and responses

> Speaker notes: Timescale vs tangible actions

### Slide 8: Overview of LOPA – Chapter 2
- Back to Table Contents

### Slide 9: What is LOPA? (2.2)
- LOPA is a semi-quantitative (Order-of-Magnitude) technique for risk identification
- For a given cause-consequence paring determined in a prior qualitative method, LOPA determines whether sufficient safeguards are in place to ensure an acceptable risk.
- LOPA does not determine what safeguards to use, but only whether proposed one is sufficient to close risk reduction gap

> Speaker notes: Reprioritize: bold highlighting

### Slide 10: What LOPA Does (2.3)
- For a given cause (initiating event), LOPA determines whether IPLs between that cause and its consequence are sufficient to reduce the probability of that consequence occurring.
  - An IPL is a safeguard that has been validated as a credible according to IEC standards which require independence, effectiveness, and auditability.
- LOPA often uses quantitative tools such as Fault Trees for visualization of Event-IPL-Consequence relationships 
- Ideally, only one IPL is used to close gap – this is unrealistic

> Speaker notes: IPL definition

### Slide 11: When to Use LOPA (2.4)
- For scenarios too complex for qualitative techniques where:
  - The initiating event, sequence of events, IPL credibility are not well understood.
- For scenarios too simple for quantitative techniques (QRA):
  - Scenarios that are simple but highly critical can be upgraded to QRA
  - Only about 1% of scenarios make it to this quantitative stage 
  - QRAs are also used in place of LOPAs for justification of significant reduction in protection layers/expenditures
- Scenario = cause-consequence pairing

### Slide 12: How LOPA Works (2.5)
- Identify consequence from qualitative analysis
- Select scenario for that consequence
- Determine the initiating event and its frequency (#/yr)
- Identify existing IPLs and their PFDs (and RRFs) 
- Determine scenario risk (a function of IPLs and their PFDs)
- Determine risk reduction gap (difference of actual & tolerable risk)
- Step 4: IPL determination
- Literature PFDs can be revised based on plant experience

> Speaker notes: Need to be more concise and organized

### Slide 13: Estimating Consequence Severity - Chapter 3
- Back to Table Contents

### Slide 14: Consequence Evaluation Approaches (3.1)
- Several methods can be employed at companies’ discretion:
  - Category Approach without Direct Reference to Human Harm
    - Uses matrices to determine category (1-5) based on material characteristic, damage to plant, and cost of event.
  - Qualitative Estimates with Human Harm
    - Consequence selected from reference table w/ inputs of impact to personnel, community, environment, and facility
  - Qualitative Estimates with Human Harm with Adjustments for Post release Probabilities
    - Estimates consequence from material characteristics, magnitude of release, and personnel presence
  - Quantitative Estimates with Human Harm
    - Uses advanced modeling to predict vulnerability zone

> Speaker notes: Emphasize 3 is modified 2

### Slide 15: Consequence Evaluation Method 1: Category Approach without Direct Reference to Human Harm
- Uses matrices to determine category (1-5) based on material characteristics, damage to plant, and cost of event.
- Advantages: simplistic, easy to use and can be cross-referenced to company risk tolerance criteria
- Disadvantages: This approach does not consider impact on personnel and requires baseline modeling for damage prediction.
- Ultimately, this method is best when human impact if infeasible to determine
- Often used for Alarm Rationalization (INSA 18.2 standard recommendation)
- Back to Consequence Evaluation Methods

> Speaker notes: Emphasize human impact is often infeasible to determine

### Slide 16: Consequence Evaluation Method 2: Qualitative Estimates with Human Harm
- Table 3.2 is referenced; most severe category determines consequence
- Advantages: harm is much easier to estimate than release size (which varies)
- Disadvantages: inaccurate; assumes probability of ignition, injury, personnel present
- Back to Consequence Evaluation Methods

> Speaker notes: Move fast

### Slide 17: Consequence Evaluation Method 3: Qualitative Estimates with Human Harm with Adjustments for Post release Probabilities
- Estimates Consequence from estimated magnitude of release, material properties & personnel present
- Advantages: harm is much easier to estimate than release size
- Disadvantages: estimation is analyst-dependent which makes it prone to inconsistency.
- Back to Consequence Evaluation Methods

### Slide 18: Consequence Evaluation Method 4: Quantitative Estimates with Human Harm
- Mathematical models determine effects of release and its impact.
- Advantages: a greater degree of certainty
- Disadvantages: modeling can only be applied for exact release conditions which makes this method impractical for generic estimates
  - Also limited by computing (for now)
- Back to Consequence Evaluation Methods

> Speaker notes: Move fast

### Slide 19: Developing Scenarios - Chapter 4
- Back to Table Contents

### Slide 20: LOPA Scenario Components (4.1-4.2)
- A scenario must have minimum of an initiating event (IE) and a subsequent consequence, but often involves other components:
  - Enabling Event: event that allows IE to result in consequence
  - Enabling Condition: condition that allows IE to result in consequence
  - IPLs are included on scenario pathway to illustrate qualified safeguards between IE and consequence (Figure 4.5)
- An IE can lead to multiple consequences and thus tied to multiple scenarios
- Most scenarios such as this one are only evaluated when enabling condition is present

### Slide 21: Identifying and Developing Candidate Scenarios (4.3)
- Candidate scenarios are derived from prior qualitative hazards analysis - although not exclusively
- Each scenario should each have deviation, causes, consequences, safeguards, recommendations tabulated in Summary Sheet:
  - LOPA is to assign numeric values of probability/frequency to each scenario component in pathway 
  - Multiple summary sheets for a scenario can be drafted:
    - Consequence severity method (chapter 3) and risk tolerance criteria method (chapter 8) are often included in the title
- HAZOP (next slide) often neglects enabling events and safeguards

### Slide 22: HAZOP Example
- Table 4.3A HAZOP example shows how recommendations are produced for deviation, cause, consequence:

### Slide 23: Identifying Initiating Event (IE) Frequency – Chapter 5
- Back to Table Contents

### Slide 24: Initiating Events (5.2)
- LOPA team verifies which Initiating Events (IE) from PHA should be included in evaluated scenarios
  - Some potential IEs are misidentified; they are root causes of IEs - examples: operator training, inadequate testing, etc.
    - Root Cause = an underlying system-related reason why an incident occurred
    - The root cause is not accounted for in the scenario pathway but does impact the frequency of that IE and its scenario
- IEs are classified as either an:
  - External Event
  - Equipment Failure (control and mechanical systems)
  - Human Failure
- IEs are often only valid for enabling event/condition present
  - Time at Risk (TAR ) values are assigned to reduce IE frequency time frame

### Slide 25: Frequency Estimation (5.3)
- The frequency of initial events is estimated using failure rates of system which are found from:
  - Plant historical data
  - Literature
  - Vendors
- Failure rates are order of magnitude estimates; exact precision is reserved for more quantitative analysis techniques
- Failure rates are modified for intermittent, batch operations to consider actual time at risk (TAR)
  - Frequency = failure rate x TAR
- Typical frequencies shown 

> Speaker notes: This is a bad graph, need to delineate between the two concepts: failure rate and frequency

### Slide 26: Identifying Independent Protection Layers (IPL) – Chapter 6
- IPL Definition and Purpose (6.2)
- IPL Rules (6.3)
- IPL Classification: Passive vs Active
- Glossary:
- Probability of Failure on Demand (PFD)
- Basic Process Control System (BPCS)
- Safey Instrumented System (SIS)
- Safety Instrumented Function (SIF)
- Safety Integrity Level (SIL)
- Back to Table Contents

### Slide 27: IPL Definition and Purpose (6.2)
- An Independent Protection Layer is a device, system, or action that is capable of preventing a scenario from proceeding to its undesired consequence.
- IPLs are classified as
  - Active/passive
  - Preventative/mitigative
- The effectiveness of IPL is quantified by PFD
  - PFD of 1 = 100% failure probability
- IPL Evaluation of Safeguards
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 28: IPL Rules (6.3)
- To qualify as an IPL, a safeguard must be:
  - Independent: not impacted by initiating event (IE) occurrence/consequence or other IPLs
    - Common cause failures (CCFs) often disqualify safeguards from IPL accreditation; loss of electrical power will cause IE and make subsequent IPL inoperable 
    - Independence is assessed using two approaches:
      - Approach A: conservative, only one IPL permitted per BPCS.
      - Approach B: aggressive, permits up to two IPLs in BPCS so long as logic solvers are not re-used between IPLs (assumed that only sensor and control elements are liable to fail)
        - Not recommended for isolated equipment (tank farms)
  - Effective: must be able to detect the condition, process the information, make the decision and take the required action.
    - Effectiveness is how safeguard performs when it does not fail – independent of PFD
    - Safeguard is considered ineffective if not rated properly (PSV capacity, blast wall strength, operator physical capability)
  - Auditable: effectiveness can be validated with testing and documentation on a periodic basis
    - This ensures reliability of safeguard
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 29: IPL Classification: Passive vs Active
- PASSIVE IPLs are safeguards that require no action to prevent an IE from resulting in a consequence.
  - These still have PFD values – albeit lower – due to the possibility of fabrication defects*
    - *Note that this delineation differs by company, some analysts consider improper fabrication or accrued corrosion to be independent scenarios with their own required IPLs
  - ISD is not considered an IPL itself, but does remove the need for an IPL as there is no scenario altogether
  - Examples of passive IPLs include dikes, drainage systems, open vents, blast walls
- ACTIVE IPLs require action of an automatic system or personnel in response to IE detection
  - Automatic IPLs usually consist of sensor, logic solver, and final control element:
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 30: IPL Classification: Mitigative vs Preventative (6.6)
- Mitigative IPLs reduce the frequency of a high-severity consequence but often initiate additional lower-severity consequence
  - Example: PRV that prevents runaway reaction but discharges flammable contents to atmosphere
  - LOPA analyst must use discretion: Is consequence trade-off is beneficial?
    - Most new consequences require their own scenario LOPA
- Preventative IPLs reduce the frequency of a high-severity consequence without the creation of another consequence
  - Example: inhibitor addition, steam valve closure, emergency cooling water flow
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 31: IPL - Instrumented Systems
- Instrumented systems are either Basic Process Control Systems (BPCS) or Safety Instrumented Systems (SIS)
  - BPCS IPLs have higher PFDs (rule of thumb is 1 x 10-1) than SIFs because of lacking element redundancy, security, and testing capability
    - SIF PFD goes down with increasing redundancy and testing frequency although these have tradeoffs of cost, convenience
- All instrumented systems have two types of controls:
  - Continuous Controller: normal control of process variable
  - State Controller: conditional control of process variables - alarms, interlocks, etc.
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 32: IPLs – More Examples
- Vendor Installed Safeguards are often included with fired equipment and rotating equipment
  - Ex.: Burner management systems (BMS) include fire eyes and purging cycles, must be maintained like any IPL
- Firefighting mitigation systems such as deluges, foam systems, sprays are safeguards that are not classified as IPLs due to reliability concerns
- Pressure relief systems are common IPLs for vessel protection but can create an additional IE/scenario for emitted material
  - Two-phase flow PRVs have higher PFD due to uncertainty of relieving conditions
- Human IPLs require operator action and have PFDs that correspond to expected operator response times (shorter time = higher PFD)
  - IPLs can lose credibility if operators’ workload is abnormally high
- Identifying Independent Protection Layers (IPL) – Chapter 6

### Slide 33: Determining the Frequency of Scenarios – Chapter 7
- Back to Table Contents

### Slide 34: Calculation of Risk
- Risk is found using Risk Index method:
  - Scenario Frequency, fc , is found using two methods:
    - Numerical Method
    - Logarithm Method
  - Consequence Severity, Ck  , from Chapter 3 methods

### Slide 35: Quantitative Calculation of Frequency and Risk – Numerical Methods (7.2)
- Calculate the fc , Mitigated Consequence Frequency (MCF),  for a given consequence:
    - fi     frequency of IE  found from Chapter 5
    - PFDj  for each IPL within scenario
    - Conditional modifiers, CM , for toxic/flammable release: probability of ignition, person present, and injury
      - Best to use decision tree for CM
  - For a consequence w/ multiple IEs:
    - Where fiC  is the consequence frequency for an IE, i
  - MCF should also be modified for IE has high frequency (Demand Freq. = 2 x Test Freq.)

### Slide 36: Calculation of Frequency with Integer Logarithm Methods (7.4)
- Consequence frequency:
  - FiI   log of the single IE frequency (absolute value)
  - Pij’  log of an IPL PFD (absolute value)
- This effectively correlates resulting FiC  integers to given consequence frequencies:
  - 1 = 1 x 10-1 /yr,
  - 4 = 1 x 10-4 /yr,
  - etc.
- This method is more simple than numerical methods but has less accuracy

### Slide 37: Summary of Consequence Frequency Calculation Methods
- Main methods:
  - Numerical Methods (7.2): calculates product of IE frequencies, IPL PFDs and CMs
    - Modified for consequence w/ multiple IEs
  - Integer Logarithm Methods (7.4): gets integer from logarithm of IE frequencies, IPL PFDs
  - Number of IPL Credits Method (Chapter 8, not covered yet): same as Numerical Methods, but utilizes adjusted IE frequency based on IPL PFDs to disregard direct IPL PFDs incorporation

### Slide 38: Using LOPA to Make Risk Decisions – Chapter 8
- Back to Table Contents

### Slide 39: Introduction to Risk Decisions (8.2)
- After scenario risk has been determined (Chapter 7), path forward is one of the following:
  - Manage residual risk by continuing with current operation
  - Modify operation to make risk tolerable
  - Abandon risk by terminating operation
- Whether the risk is tolerable is a decision made requiring judgement. Different types of risk judgement:
  - Comparing Calculated Risk with Predetermined Tolerable Risk – predominant method that has been demonstrated in these slides
  - Analyst Expert Opinion – not recommended
  - A third is a combination of these ^ two
- The reason that both forms of judgement are important: politics. A consequence can be deemed more/less consequential than Chapter 3 estimates due to the external perception of that consequence event
  - This component should be used as a tiebreaker for risk rather than the core determination of it. Additionally, analyst expert teams should not be single person.

### Slide 40: Comparing Calculated Risk to Scenario Risk Tolerance Criteria (8.3)
  - This is the most common type of risk judgement. Risk decision methods for this judgement are:
    - Matrix Methods (Qualitative): categorization using Consequence Severity Category (chapter 3, method 1) and Consequence Frequency (chapter 7)
    - Numerical Criteria Method (Semi-Quantitative) : For given consequence severity category, prohibits the exceedance of a given metric:
      - Usually either the maximum consequence frequency or number fatalities
    - Number of IPL Credits Method (Quantitative): For given consequence severity category and IE frequency, a certain number of IPL Credits (reduction in frequency) is required:

### Slide 41: Implementing LOPA – Chapter 9
- Back to Table Contents

### Slide 42: Is Company Ready for LOPA? (9.2)
- There are multiple criteria a company must satisfy to implement & sustain the practices intended with LOPAs
- Company’s LOPA personnel can’t be one-off subgroup (like a contractor, so to speak) within the organization
- The goals of LOPA should function interdependently with other KPIs in the organization
  - LOPA is not a ranked priority; it is the priority
- OSHA PSM program participation is necessary
  - LOPA scenarios must be drafted in prior PHA

### Slide 43: What Data are Required? (9.4)
- Consequences: no data available for this; chapter 3 methods must be used
- Component Failure Data: for every device (PSV, control loops, and procedures):
  - Best Source: Guidelines for Process Equipment Reliability Data CCPS 1989
  - Note that these generic data should be altered based on plant-specifcs (materials handled, climate, etc.)
- Human Error Rates: used for Human IPL PFDs
  - Best Source: Guidelines for Preventing Human Error in Process Safety CCPS 1994
  - Note that internal data on this is anecdotal, at best; use literature
- Incident Data: used for initiating event frequencies
  - Best Sources:
    - Research Paper
    - MARS (Major Accident Reporting System – European)
    - CSB Accidental Release Database –started in 2020

### Slide 44: How Are the Risk Tolerance Criteria Established? (9.6)
- Over-safeguarding a unit is as problematic as under-safeguarding it
  - Auditability of IPLs drops w/ overcomplexity
- Appropriate risk tolerance criteria is necessary to ensure the integrity of LOPA process:
  - Personnel will not feel obligated to hit PSV PMs if there are too many PSVs
- Common Risk Tolerance Criteria Methods:
  - Explicit: target risk value defined by organization
  - Implicit: risk judgment tool such as a risk matrix
- Both^ should be used to establish criteria before the LOPA begins
- See Risk Decisions/Judgement (8.2) Slide

### Slide 45: When to Use LOPA? (9.7)
- Use this flowchart, Evaluate Study for:
- Consequence Severity (Categorical)
- Consequence Frequency
- SIL Presence (guaranteed for any existing SIS)

### Slide 46: Typical Implementation Steps (9.8)
- Documenting Risk Tolerance Criteria
  - Acceptable level according to the organization
- The LOPA Guidance Document
  - Defined within organization for procedural execution of LOPA
- Developing a Step-by-Step Procedure
  - More specific procedural steps (IPL PFDs, IE frequencies, etc.)
- Conducting Pilot Tests
  - This is to evaluate material-specific hazards (runaway reactions)
- Developing Training Courses and Training the Analysts
  - 2-day training course required for attendees involving direct coaching
- Developing Training for Personnel Who Support LOPA
- Developing User Friendly Tools

### Slide 47: Using LOPA for Other Applications – Chapter 10
- Back to Table Contents

### Slide 48: Purpose (10.1)
- Due to semi-quantitative nature of LOPA, it naturally has many other applications:
- Capital improvement planning
- Management of change
- Mechanical integrity programs/risk-based inspections (next slide)
- Risk-based operator training
- Emergency response training
- Determining a credible design basis for overpressure protection (next slide)
- Evaluating a facility siting risks
- Evaluating the need for emergency isolation valves
- Evaluating the removal of a safety system from service
- Incident investigations
- Determining an SIL for SIF

### Slide 49: Using LOPA in Mechanical Integrity Programs or Risk-Based Inspection/Risk-Based Maintenance Programs (10.4)
- LOPA results such as the IPL PFDs allow maintenance teams to prioritize the maintenance/inspection of safety critical equipment (SCE)
  - IPLs that do not contribute to the risk reduction gap can be given lower (or no) priority

### Slide 50: Using LOPA to Determine a Credible Design Basis for Overpressure Protection (10.7)

### Slide 51: Advanced LOPA Topics – Chapter 11
- Back to Table Contents

### Slide 52: Counting Multiple Functions in One BPCS as IPLs in the Same Scenario (11.2)
- This section revisits section 6.3: IPL Rules (Independence assessment)
- Approaches A or B can be used for BPCS IPL accreditation:
  - Approach A assumes any failure of the BPCS, regardless of component, compromises the entire system
    - Conservative: 1 IPL per BPCS
  - Approach B assumes BPCS components are independent and that Logic Solvers are significantly less prone to failure
    - Aggressive: 2 IPLs per BPCS
- Approach B allows for Logic Solver to be shared between IPLs, but this requires independent Sensor, Input/Output Cards, and Final Control Elements:
  - Assumption that Logic Solver has significantly lower PFD than other components must be verified

### Slide 53: Additional Literature
- Guidelines for Hazard Evaluations Procedures (CCPS)
- Process Quantitative Risk Analysis (CCPS)
- Guidelines for Safe Automation of Chemical Processes (CCPS)
