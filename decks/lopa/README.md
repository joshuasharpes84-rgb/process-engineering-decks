# Layer of Protection Analysis

LOPA methodology: initiating event frequency, independent protection layers, enabling conditions/conditional modifiers, and target mitigated risk.

- **View in browser:** https://jsharpes-portfolio.netlify.app/slides/lopa/
- **Download the .pptx (279 MB):** https://github.com/joshuasharpes84-rgb/process-engineering-decks/releases/download/decks-v1/Layer-of-Protection-Analysis.pptx
- **Author:** Joshua Sharpes, EIT (https://jsharpes-portfolio.netlify.app)
- **Slides:** 51

## How to use this file
This is the slide-by-slide text of the deck, extracted so you (or your AI assistant) can search it, quote it, or ask questions about it without opening a large PowerPoint file. Figures, charts and equations drawn as images are not captured here; open the viewer or the .pptx for those. Narrated decks play their audio in PowerPoint Slide Show mode.

## Slide outline

### Slide 1: Layer of Protection Analysis
- Joshua Sharpes

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
- Estimating Consequences and Severity
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
  - Consequence: measure of the expected effects of an event in terms of personnel impact, environmental damage, and loss of business.
    - This is triple bottom line – people, planet, profit.
- Probability of Failure on Demand (PFD): likelihood of device/method failing when dependent upon.
- Frequency: initiating event occurrences per year
- Risk Reduction Gap: the difference between tolerable risk and actual risk of scenario
  - Risk Reduction Factor (RRF): IPL factor that serves as credit to close this gap

> Speaker notes: Ipl definition needed in addition to other terms more frequently mentioned

### Slide 5: History of LOPA (1.2)
- American Chemistry Council published Responsible Care Process Safety Code of Management Practices the late 80s in effort to formalize practice for evaluating safeguards
- CCPS Standards were developed in the late 90s which began to
  - Develop semi-quantitative tool for industry use
  - Establish Safety Instrumented Function (SIF) classification for Safety Integrity Level (SIL) determination
  - Reduce scenarios that would need QRA
- ISA (US) and IEC (International) standards were being developed simultaneously for exact SIL calculation based on SIF classification
  - These standards are what is used today
- Up until these developments, plants would implement informal or formal, but inconsistent, methods for closing their risk reduction gaps which resulted in over-reliance on the process design phase outcomes

### Slide 6: Use of LOPA in the Process Life Cycle (1.3)
- Design phase during drafting PFDs/P&IDs
  - Can be used to modify inherently safer design (ISD)
- Modifications to an Existing Process throughout lifecycle
- Identification of safety critical equipment that require periodic testing and maintenance
- Determination of acceptable risk
- Operator actions and responses

> Speaker notes: Timescale vs tangible actions

### Slide 7: Overview of LOPA – Chapter 2

### Slide 8: What is LOPA? (2.2)
- LOPA is semi-quantitative technique risk identification method used as an intermediate between the qualitative and quantitative methods
  - Spectrum of qualitative and quantitative methods
- For a given cause-consequence paring determined in a prior qualitative method, LOPA determines whether sufficient safeguards are in place to ensure an acceptable risk.
- LOPA does not determine what safeguards to use, but only whether proposed one is sufficient to close risk reduction gap

> Speaker notes: Reprioritize: bold highlighting

### Slide 9: What LOPA Does (2.3)
- For a given cause (initiating event), LOPA determines whether IPLs between that cause and its consequence are sufficient to reduce the probability of that consequence occurring.
  - An IPL is a safeguard that has been validated as a credible according to IEC standards which require independence, effectiveness, and auditability.
- LOPA often uses quantitative tools such as Fault Trees for visualization of Event-IPL-Consequence relationships 
- Ideally, only one IPL is used to close gap – this is unrealistic

> Speaker notes: IPL definition

### Slide 10: When to Use LOPA (2.4)
- For scenarios too complex for qualitative techniques where:
  - The initiating event, sequence of events, IPL credibility are not well understood.
- For scenarios too simple for quantitative techniques (QRA):
  - Scenarios that are simple but highly critical can be upgraded to QRA
  - Only about 1% of scenarios make it to this quantitative stage 
  - QRAs are also used in place of LOPAs for justification of significant reduction in protection layers/expenditures
- Scenario = cause-consequence pairing

### Slide 11: How LOPA Works (2.5)
- Identify consequence from qualitative analysis
- Identify scenario for consequence
- Determine the initiating event frequency (#/yr)
- Identify existing IPLs and their PFD (and RRFs) 
- For scenario, determine risk (a function of IPLs and their PFDs)
- Determine risk reduction gap (this is actual minus tolerable risk)
- Step 4: IPL determination
- Literature PFDs can be revised based on plant observations

> Speaker notes: Need to be more concise and organized

### Slide 12: Estimating Consequences and Severity - Chapter 3

### Slide 13: Consequence Evaluation Approaches (3.1)
- Several methods can be employed at companies’ discretion:
  - Category Approach without Direct Reference to Human Harm
    - Uses matrices to determine category (1-5) based on material characteristic, damage to plant, and cost of event.
  - Qualitative Estimates with Human Harm
    - References table for selection of low, medium high , and very high consequence based on inputs of impact to personnel, community environment, and facility
  - Qualitative Estimates with Human Harm with Adjustments for Post release Probabilities
    - Uses estimate of release magnitude with frequency of event (chapter 7) that personnel will be present.
  - Quantitative Estimates with Human Harm
    - Uses modeling to predict vulnerability zone

> Speaker notes: Emphasize 3 is modified 2

### Slide 14: Consequence Evaluation Method 1: Category Approach without Direct Reference to Human Harm
- Advantages: simplistic, easy to use and can be cross-referenced to company risk tolerance criteria
- Disadvantages: This approach does not consider impact on personnel and requires baseline modeling for damage prediction.
- Ultimately, this method is best when human impact if infeasible to determine
- Often used for Alarm Rationalization (INSA 18.2 standard recommendation)

> Speaker notes: Emphasize human impact is often infeasible to determine

### Slide 15: Consequence Evaluation Method 2: Qualitative Estimates with Human Harm
- Table 3.2 is referenced by LOPA analyst
- Advantages: harm is much easier to estimate than release size
- Disadvantages: assumes probability of ignition, injury, personnel present

> Speaker notes: Move fast

### Slide 16: Consequence Evaluation Method 3: Qualitative Estimates with Human Harm with Adjustments for Post release Probabilities
- Instead of using lookup table (as in Method 2), uses estimated magnitude of release in conjunction with Chapter 7 Frequency evaluation which considers material properties/personnel present.
- Advantages: harm is much easier to estimate than release size
- Disadvantages: estimation is analyst-dependent which makes it prone to inconsistency.

### Slide 17: Consequence Evaluation Method 4: Quantitative Estimates with Human Harm
- Mathematical models determine effects of release and its impact.
- Advantages: a greater degree of certainty
- Disadvantages: modeling can only be applied for exact release conditions which makes this method impractical for generic estimates

> Speaker notes: Move fast

### Slide 18: Developing Scenarios - Chapter 4

### Slide 19: LOPA Scenario Components (4.1-4.2)
- A scenario must have minimum of an initiating event (IE) and a subsequent consequence, but often involves other components:
  - Enabling Event: event that allows IE to result in consequence
  - Enabling Condition: condition that allows IE to result in consequence
  - IPLs are included on scenario pathway to illustrate qualified safeguards between IE and consequence (Figure 4.5)
- An IE can lead to multiple consequences and thus tied to multiple scenarios
- Most scenarios such as this one are only evaluated when enabling condition is present

### Slide 20: Identifying and Developing Candidate Scenarios (4.3)
- Candidate scenarios are derived from prior qualitative hazards analysis
- Each scenario should each have deviation, causes, consequences, safeguards, recommendations tabulated in Summary Sheet:
  - LOPA is to assign numeric values of probability/frequency to each scenario component in pathway 
  - Multiple summary sheets for a scenario can be drafted:
    - Consequence severity method (chapter 3) and risk tolerance criteria method (chapter 8) are often included in the title
- HAZOP - next slide - often neglects enabling events and safeguards

### Slide 21: HAZAOP Example
- Figure 4.2 HAZOP example shows how recommendations are produced for deviation, cause, consequence:

### Slide 22: Identifying Initiating Event (IE) Frequency – Chapter 5

### Slide 23: Initiating Events (5.2)
- LOPA team verifies which Initiating Events (IE) from PHA should be apart of scenarios
  - Some potential IEs are misidentified; they are root causes of IEs (examples: operator training, inadequate testing, etc.)
  - LOPA team needs to understand difference between IE and root cause of that IE
    - Root Cause = an underlying system-related reason why an incident occurred
    - The root cause is not accounted for in the scenario pathway but does impact the frequency of that IE and its scenario
- IEs are classified as either an:
  - External Event
  - Equipment Failure (control and mechanical systems)
  - Human Failure
- IEs are often only valid for enabling event/condition present
  - Time at Risk (TAR ) values are assigned to reduce IE frequency time frame

### Slide 24: Frequency Estimation (5.3)
- The frequency of initial events is estimated using failure rates of system which are found from:
  - Plant historical data
  - Literature
  - Vendors
- Failure rates are order of magnitude estimates; exact precision is reserved for more quantitative analysis techniques
- Failure rates are modified for intermittent, batch operations to consider actual time at risk (TAR)
  - Frequency = failure rate x TAR
- Typical frequencies shown 

> Speaker notes: This is a bad graph, need to delineate between the two concepts: failure rate and frequency

### Slide 25: Identifying Independent Protection Layers (IPL) – Chapter 6
- IPL Definition and Purpose (6.2)
- IPL Rules (6.3)
- Glossary:
- Probability of Failure on Demand (PFD)
- Basic Process Control System (BPCS)
- Safey Instrumented System (SIS)
- Safety Instrumented Function (SIF)
- Safety Integrity Level (SIL)

### Slide 26: IPL Definition and Purpose (6.2)
- An Independent Protection Layer is a device, system, or action that is capable of preventing a scenario from proceeding to its undesired consequence.
- IPLs are classified as
  - Active/passive
  - Preventative/mitigating
- The effectiveness of IPL is quantified by PFD
  - PFD of 1 = 100% failure probability
- IPL Evaluation of Safeguards

### Slide 27: IPL Rules (6.3)
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
  - Auditable: effectiveness can be validating with testing and documentation on a periodic basis
    - This ensures reliability of safeguard

### Slide 28: IPL Classification: Passive vs Active
- Passive IPLs are safeguards that require no action to prevent an IE from resulting in a consequence.
  - These still have PFD values – albeit lower – due to the possibility of fabrication defects*
    - *Note that this delineation differs by company, some analysts consider improper fabrication or accrued corrosion to be independent scenarios with their own required IPLs
  - ISD is not considered an IPL itself, but does remove the need for an IPL as there is no scenario altogether
  - Examples of passive IPLs include dikes, drainage systems, open vents, blast walls
- Active IPLs require action of an automatic system or personnel in response to IE detection
  - Automatic IPLs usually consist of sensor, logic solver, and final control element:

### Slide 29: IPL - Instrumented Systems
- Instrumented systems are either Basic Process Control Systems (BPCS) or Safety Instrumented Systems (SIS)
  - BPCS IPLs have higher PFDs (rule of thumb is 1 x 10-1) than SIFs because of lacking element redundancy, security, and testing capability
    - SIF PFD goes down with increasing redundancy and testing frequency although these have tradeoffs of cost and convenance
- All instrumented systems have two types of controls:
  - Continuous Controller: normal control of process variable
  - State Controller: conditional control of process variables - alarms, interlocks, etc.

### Slide 30: IPLs – More Examples
- Vendor Installed Safeguards are often included with fired equipment and rotating equipment
  - Burner management systems (BMS) include fire eyes and purging cycles, must be maintained like any IPL
- Firefighting mitigation systems such as deluges, foam systems, sprays are safeguards that are not classified as IPLs due to reliability concerns
- Pressure relief systems are common IPLs for vessel protection but can create an additional IE/scenario for emitted material
  - Two-phase flow PRVs have higher PFD due to uncertainty of relieving conditions
- Human IPLs require operator action and have PFDs that correspond to expected operator response times (shorter time = higher PFD)
  - IPLs can lose credibility if operators’ workload is abnormally high

### Slide 31: IPL Classification: Mitigative vs Preventative (6.6)
- Mitigative IPLs reduce the frequency of a high-severity consequence but often initiate another lower-severity consequence
  - Example: PRV that prevents runaway reaction but discharges flammable contents to atmosphere
  - LOPA analyst must use discretion is consequence trade-off is beneficial
    - Most new consequences require their own scenario LOPA
- Preventative IPLs reduce the frequency of a high-severity consequence without the creation of another consequence
  - Example: inhibitor addition, steam valve closure, emergency cooling water flow

### Slide 32: Determining the Frequency of Scenarios – Chapter 7

### Slide 33: Quantitative Calculation of Risk and Frequency – Numerical Methods (7.2)
- Calculate the Mitigated Consequence Frequency (MCF),  for a given consequence:
    - fi  = frequency of initiating event  found from Chapter 5
    - Use conditional modifiers, CM , for component of toxic/flammable release: probability of ignition, probability of person present, and probability of injury
      - Flammable substances can be ignited several ways (immediate, delayed, etc.), each with different probabilities; it is best to use decision tree for CM
  - Since consequence can be caused by multiple IEs, MCF can be modified to account for each IE:
  - MCF should also be modified for IE has high frequency (Demand Freq. = 2 x Test Freq.)
- Calculate the Risk of undesired outcome, k, using Risk Index method:
  - Ck  is the measurement of the consequence, determined using Chapter 3 methods

### Slide 34: Calculation of Risk or Frequency with Integer Logarithm Methods (7.4)
- An alternative to the numerical methods of the last slide, this method can be employed by taking the logarithm of IE frequencies and the IPL PFDs:
- This effectively correlates resulting FiC  integers to given consequence frequencies:
  - 1 = 1 x 10-1 /yr,
  - 4 = 1 x 10-4 /yr,
  - etc.
- This method is more simple than numerical methods but has less accuracy

### Slide 35: Summary of Consequence Frequency Calculation Methods
- Main methods:
  - Numerical Methods (7.2): calculates product of IE frequencies, IPL PFDs and conditional modifiers
  - Integer Logarithm Methods (7.4): takes logarithm of IE frequencies and IPL PFDs to get integer result
  - Number of IPL Credits Method (Chapter 8, not covered yet): same as Numerical Methods, but utilizes adjusted IE frequency based on IPL PFDs to disregard the IPL PFDs in this calculation

### Slide 36: Using LOPA to Make Risk Decisions – Chapter 8

### Slide 37: Introduction (8.2)
- After scenario risk has been determined (Chapter 7), path forward is one of the following:
  - Manage residual risk by continuing with current operation
  - Modify operation to make risk tolerable
  - Abandon risk by terminating operation
- Whether the risk is tolerable is a decision made requiring judgement. Different types of risk judgement:
  - Comparing calculated risk with predetermined tolerable risk – predominant method that has been demonstrated in these slides
  - Analyst Expert Opinion – not recommended
  - A third is a combination of these ^ two
- The reason judgement is important: politics. A consequence can be deemed more/less consequential than Chapter 3 estimates due to the perception of that consequence event
  - This component should be used as a tiebreaker for risk rather than the core determination of it. Additionally, analyst expert teams should not be single person.

### Slide 38: Comparing Calculated Risk to Scenario Risk Tolerance Criteria (8.3)
  - This is the most common type of risk judgement. Risk decision methods for this judgement are:
    - Matrix Methods: qualitative categorization using Consequence Severity Category (chapter 3, method 1) and Consequence Frequency (chapter 7)
    - Numerical Criteria Method: For given consequence severity category, prohibits the exceedance of a given metric:
      - Usually either be maximum consequence frequency or number fatalities
    - Number of IPL Credits Method: For given consequence severity category and initiating event frequency, requires a certain number of credits that correlate to the IPL PFDs:

### Slide 39: Implementing LOPA – Chapter 9

### Slide 40: Is Company Ready for LOPA? (9.2)
- There are multiple criteria a company must satisfy to not only implement but also sustain the practices intended with LOPAs
- Generally speaking, a company’s LOPA personnel can not be positioned as a one-off subgroup (like a contractor, so to speak) within the organization
- The goals of LOPA need to work interdependently with other production KPIs in the organization
  - LOPA is not a ranked priority; it is the priority
- OSHA PSM program participation is necessary
  - LOPA scenarios are drafted in prior PHAs

### Slide 41: What Data are Required? (9.4)
- Consequences: no data available for this; chapter 3 methods must  used
- Component Failure Data: for every device (PSV, control loops, and procedures)
  - Best Source: Guidelines for Process Equipment Reliability Data CCPS 1989
  - Note that these generic data should be altered based on plant particulars (materials handled, climate, etc.)
- Human Error Rates: used for Human IPL PFDs
  - Best Source: Guidelines for Preventing Human Error in Process Safety CCPS 1994
  - Note that internal data on this is anecdotal, at best
- Incident Data: used for initiating event frequencies
  - Best Sources:
    - https://www.icheme.org/media/9781/xx-paper-87.pdf (Summary Research Paper)
    - MARS (Major Accident Reporting System – European)
    - CSB Accidental Release Database –started in 2020

### Slide 42: How Are the Risk Tolerance Criteria Established? (9.6)
- Over-safeguarding a unit is as problematic as under-safeguarding it:
  - Auditability of IPLs drops
- Therefore, appropriate risk tolerance criteria is necessary to ensure the integrity of the LOPA process:
  - Personnel will not feel obligated to hit PSV PMs if there are too many PSVs
- Common Risk Tolerance Criteria Methods:
  - Explicit: Target risk value defined by organization
  - Implicit: risk judgment tool such as a risk matrix
  - Both of these methods should be used to establish criteria before the LOPA begins

### Slide 43: When to Use LOPA? (9.7)
- Two different approaches are used:
- Use the Estimated Risk from PHA
- Use the Consequence Category 
  - This flowchart shows potential progression to quantitative risk assessment (QRA)

### Slide 44: Typical Implementation Steps (9.8)
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

### Slide 45: Using LOPA for Other Applications – Chapter 10

### Slide 46: Purpose (10.1)
- Due to semi-quantitative nature of LOPA, it has many applications:
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

### Slide 47: Using LOPA in Mechanical Integrity Programs or Risk-Based Inspection/Risk-Based Maintenance Programs (10.4)
- LOPA results such as the IPL PFDs allow maintenance teams to prioritize the maintenance/inspection of safety critical equipment (SCE)
  - IPLs that do not contribute to the risk reduction gap can be given lower (or no) priority
- Maintenance teams can also use the IE frequency to gauged how frequently the IPL should be inspected and maintained

### Slide 48: Using LOPA to Determine a Credible Design Basis for Overpressure Protection (10.7)

### Slide 49: Advanced LOPA Topics – Chapter 11

### Slide 50: Counting Multiple Functions in One BPCS as IPLs in the Same Scenario (11.2)
- Approaches A or B can be used for BPCS IPL accreditation:
  - Approach A assumes any failure of the BPCS, regardless of component, compromises the entire system
    - Conservative: 1 IPL per BPCS
  - Approach B assumes BPCS components are independent and that Logic Solvers are significantly less prone to failure
    - Aggressive: 2 IPLs per BPCS
- Approach B allows for Logic Solver to be shared between IPLs, but this requires independent Sensor, Input/Output Cards, and Final Control Elements:
  - Assumption that Logic Solver has significantly lower PFD than other components must be verified

### Slide 51: Additional Literature
- Guidelines for Hazard Evaluations Procedures (CCPS)
- Process Quantitative Risk Analysis (CCPS)
- Guidelines for Safe Automation of Chemical Processes (CCPS)
