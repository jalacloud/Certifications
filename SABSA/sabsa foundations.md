# SABSA Chartered Security Architect
### January 2021

---

SABSA Certification Study // Exam Preparation

# F1 Content
## Section 1 - SABSA Principals & Objectives
- #### Enterprise Security Architecture Framework
  - A consistent set of principals, policies, capabilities and standards that sets the direction and vision for the development and operation of the organisation's business information systems so as to ensure alignment with and support for the business needs.
  - __Concept of Enterprise__:
  	- The treatment of an organisation as a single entity
	- Aims to optimise all parts of the organisation in a coherent way
  - __Concept of Security__:
  	- To provide confidence & assurance
	- To protect business assets
	- To support business objectives
  - The REAL role of Architected Security:
  	- Enable business
	- Enable technology
	- Enable change - securely
	- Protecting relationship & leveraging trust
- #### SABSA Guiding Principals
  - Architecture must not presuppose any particular:
  	- Cultures or operating systems
	- Management style
	- Set of management processes
	- Management standards
	- Technology standards
	- Technology platforms
  - Because ALL of these things change over time
  - Architecture must meet your unique set of business requirements
  - Architecture must provide sufficient flexibility to incorporate choice and change of policy, standards, practices, or legislation
 
- #### Holistic Approach
  - Provide ALL the links in the chain
  - Ensure that security services are properly managed
  - To ensure that security meets the needs of the business

- #### Features, Benefits, and Advantages


## Section 2 - SABSA Framework Overview
- #### The SABSA Matrix
- #### The Traceability Concept
  - Traceability for __Completeness__: Every business requirement for security is met and the residual risk is acceptable to the business appetite.
  - Tracebility for __Justification__: Every operational or technological security element can be justified by reference to a risk-prioritised business requirement.
  - Applications of Traceability:
    * Bi-directional - Completeness. Justification.
    * Actuarial Preservation - Controls. Enablers.
    * Manage Change - Confirm links not removed.
    * Knowledge Management - Re-use components. Predictability.
      
## Section 3 - Business Context & Requirements
- #### The Traceability Concept
  - Approach to traceability:
    * Good traceability requires small, credible steps, not big jumps
    * __Buzzwords__: Credible abstraction, business-drivers, two-way, business drivers for security. 
- #### Credible abstraction of business requirements
	- Meaningful traceabiity is enabled by credible abstraction from business context (assets, goals and objective) to a business security context
	- Traceability therefore starts by delivering two slightly different sets of requirements:
		1. Business Requirements - Business-level assets, goals and objectives.
		2. Business Drivers for Security - The business requirement abstracted into one or more statements of security-relevance to the business requirement
- #### SABSA Attributes
  - __Attributes Customisation__
    - The Attributes Profile represents the business requirements for security for a specific organisation and should be customised to fully reflect local needs & culture
    - Customised attribute names
    - Customised attribute definitions
    - Customised attribute measures, metrics & performance targets
    	- Advanced useage involves multiple domain levels with linkage and aggregated performance
  - Attributes can be tangible or intangible
  - Provides the "missing link" between business requirements and technology / process design
  - Powerful requirements engineering technique
  - Attributes must be measurable
  - Attributes represent what is most important to any stakeholder

## Section 4 - Risk & Opportunity Framework
- #### Role of Risk Management is Business & Architecture
  - Achieve an appropriate balance between realising opportunities for gains while minimising losses/threats.
  - Defined through 'Opportunities & Threats Inventory' (Contextual/Motivation - SABSA Matrix Cell)
  - Achieved through analysis of Internal & External Risk Factors
  - Establish an appropriate infrastructure and culture and apply a logical and systematic method
  - Embed into the organisation's philosophy, practices and business processes
  - Accountability assurance & governance
- #### Risk Assessment
  - __Advantages of the Impact-based Approach__
    - Much broader view of the business goals - not just the tangible assets
    - Provides a good view of business criticality
    - Allows priorities to be established
    - Uses language understood by business managers
    - Involves the business managers in the process
    - Speed, cost, usability
  - PESTELIM Analysis
    * Political Factors
    * Economic Factors
    * Social Factors
    * Technological Factors
    * Environmental Factors
    * Legal Factors
    * Industry Factors
    * Military Factors
  - SWOT Analysis (Strengths, Weaknesses, Opportunities, Threats)
- #### Risk Management Process
  - The SABSA Lifecycle with the addition of Assurance and Govern & Communicate.
  	- Strategy & Planning
	- Design
	- Implement
	- Manage & Measure
	- Assurance and Governance overlay
- #### Risk Management Systems
  - SABSA Risk & Opportunity Model
    - Risk Context: Negative Outcomes vs Positive Outcomes.
    - Threats vs Opportunities
    - Loss Event vs Beneficial Event
    - Impact is expressed as positive or negative consequences of potential events upon Attributes
    - Negative impact expressed as:
    	- Reduction in Attribute performance
	- Failure to meet Attribute performance target
    - Positive impact expressed as:
    	- Increase in Attribute performance
	- Increase in Attribute performance threshold to higher target
    - Controls (Protect from Negative Consequences) --> __Attribute__ <-- Enablers (Enhance for Positive Consequences)

## Section 5 - Policy Architecture
- #### Policy Framework
  - The security policy is determined by the business requirements for information management and information systems, following an assessment of the possible operational risks & opportunities
  - Security policy is a statement of business requirements for security, translated into a logical structure that can be consistently applied, monitored and measured (using Attributes)
  - The security policy states what logical services are required by as far as possible avoids any reference to particular physical mechanisms/controls/services
  - __ENTERPRISE POLICY:__
  	- Contextual Policy (Business View): Over-arching Business Risk Management Policy (Enterprise Wide)
  	- Conceptual Policy (Architect View): Policies for each Enterprise Risk Stategy (Enterprise Wide) - Sub-domains within Enterprise superdomain
  - __DOMAIN POLICY:__
  	- Logical Policy (Designer View): __Policies__ for each Risk Strategy (Domain Level)
  	- Physical Policy (Builder View): __Procedures & Practices__ for each Risk Strategy (Domain Level)
  	- Component Policy (Tradesman View): Detailed __Standards and Rules__ for each Risk Strategy (Domain Level)
  	- Operational Policy (Service Manager View): Detailed Security __Implementation & Operation Guides__ (Domain Level)
  - Each Policy Authority in the SABSA Policy Framework is accountable for the risks and opportunities to their own domain-level assets (attributes), goals & objectives
- #### Policy Domain Concept
  - A security domain is a set of elements subject to a common security policy defined and owned by a single security policy authority.
  	- Every domain has a Policy Authority - the owner of risk TO that domain
- #### Policy Domain Model
  - Enterprise-wide Business Risk Management Policy (CONTEXTUAL) - Superdomain
  - Enterprise Risk Strategy Policy (CONCEPTUAL) - Delegated responsiblity from owner of enterprise/organisation (CEO)
  	- Example: CIO = Information Risk Policy, CFO = Financial Risk Policy, COO = Operations Risk Policy...etc
  - Domain-specific Interpretation (LOGICAL)
  	- Sub-Domain(s): LOGICAL Policy
  - __Logical__ Domain Layer = __Security Policies__
  - __Physical__ Domain Layer = __Security Procedures__
  - __Component__ Domain Layer = __Security Standards__

## Section 6 - Architectural Strategies
- #### Systems Engineering
  - Objectives of System Engineering in SABSA are:
  	* Managing complexity (through layering techniques and modularisation)
	* Top-down decomposition
	* Structured thinking
	* Peer review
	* Communication & documented preservation of ideas
  - Total System Objectives: System objectives expressed as "Business Requirements" that the system should satisfy
  	- The ability to __measure performance__ is of prime importance in order to properly satisfy the buiness requirements

- #### Integrated Compliance Framework
  - Contextual layer assesses and communicates the business requirement in the context of the overall business
  - Conceptual layer sets out the strategy for treating risk and meeting the control and enablement objectives
  - SABSA lower layers (logical, physical, component) engineer the deployment of controls (both technical and operational) in the best place, at the best time, with the best use of investment
  - The aim is to provide the framework for compliance with multiple standards simulateously
  - Allows for many standards, control frameworks, and libraries to be used within the over-arching SABSA methodology
  - Applicable frameworks and control libraries able to be leveraged within the SABSA Matrix
- #### Control Strategies
  - __The Control System Concept__
  	- The __Control sub-system__ - exerts control
	- The __monitoring and measurement sub-system__ - affected by actions of contol sub-system
	- The __Decision sub-system__ - makes decisions based upon the measurement provided by the measurement sub-system
  - Strength-in-Depth Controls Model
  	- SABSA has no controls library (standard or set of controls or control objectives) of its own
	- Controls are architected within the framework
	- Can utilise other control standards and frameworks in desired
- #### SABSA Multi-tiered Control Strategy Model
  - Proportional response to risk management and assessment through mutliple tiers; __DETER, PREVENT, CONTAIN, DETECT, RECOVER, ASSURE__
  - Prioritised, Proportional & Balanced Investment
  - SABSA multi-tiered control strategy provides assurance of security capabilities (in design or in review/audit):
  	- Risk-proportional capability to DETER
	- Risk-proportional capability to PREVENT
	- Risk-proportional capability to CONTAIN
	- Risk-proportional capability to DETECT (and also TRACK)
	- Risk-proportional capability to RECOVER
	- Risk-proportional capability to ASSURE
  - The multi-tiered controls strategy is modeled against the risk assessment __to determine proportional and appropriate response__.
  - Enables further removal of subjectivity in selection of Risk Treatments
  - Right control, right place, at the right time
  
## Section 7 - Role & Responsibility Concepts

- #### The SABSA Governance Model
  - __Phases & Activities__
  	- __STRATEGY and PLANNING:
	  - Develops Strategy and Plans
	  - Sets Goals, Objectives, & Expectations
	  - Sets Performance Targets
	  - Sets Risk Appetite
	  - Sets Policy to meet objectives and targets
	- __DESIGN__:
	  - Design Processes
	  - Design Systems
	  - Design Staffing Model
	  - Design Controls and Enablers
	- __IMPLEMENT__:
	  - Establish Processes
	  - Implement Systems
	  - Appoint and train people
	  - Establish controls and enablers
	- __MANAGE and MEASURE__:
	  - Manage processes and operations
	  - Manage systems
	  - Manage people
	  - Performance and Risk Monitoring against KPI's and KRI's
  - __Roles and Responsibilities__:
  	- OWNER: The owner is a Domain Policy Authority who sets goals, risk appetite, and performance targets for ASSETS (attributes) in a specific domain
		- __Role__: Accountable for performance of the assets (attributes) within a specific domain
		- __Governance Model__: Strategy and Planning phase
		- __Policy Role__: Sets policy for the domain
		- __Communications and Risk Management Role__:
			- Consults: Super domain authority on risk appetite
			- Consults: Lateral or externally impacted domain authorities
			- Informs: Risk performance to super domain authority (or externally if enterprise domain authority)
			- Informs: Policy & performance targets to subdomains & service providers
	- TRUSTEE: The Delegated Authority (called a steward or trustee) is appointed by a domain owner as a subject matter expert to be responsible for the assets (attributes) in a specific domain. Policy Authority to delegated to the steward or trustee.
		- __Role__: Responsible for the performance of the assets (attributes) in a specific domain
		- __Governance Model__: Strategy and Planning phase (acts as domain authority)
		- __Policy Role__: Sets policy for the domain on behalf of the domain authority
		- __Communications and Risk Management Role__:
			- Consults: Super domain authority and domain owner on risk appetite
			- Consults: Lateral or externally impacted domain authorities
			- Informs: Risk performance to super domain authority (or externally if enterprise domain authority) and domain owner
			- Informs: Policy & performance targets to subdomains & service providers
	- CUSTODIAN: The custodian is appointed by a domain owner as a subject matter expert or service provider to be RESPONSIBLE for the assets (attributes) in a specific domain. Unlike Trustees, policy authority is NOT delegated to the custodian. 
		- __Role__: Responsible for the performance of the assets (attributes) in a specific domain
		- __Governance Model__: Design, Implement, Manage & Measure phases
		- __Policy Role__: Complies with policy and SLA for the domain assets on behalf of domain authority
		- __Communications and Risk Management Role__:
			- Informed by: Domain authority on risk appetite, policy and performance target
			- Informs: Risk performance to domain authority (reports upwards)
	- COMPLIANCE: The compliance role is appointed by domain owner as subject matter expert to provide a compliance checking service and to report on the degree to which the risk appetite and policy of the owner is being met by the responsible and custodial parties
		- __Role__: Responsible for checking the performance of assets (attributes) in a specfic domain on behalf of the owner (domain owner)
		- __Governance Model__: Design, Implement, Manage & Measure phases
		- __Policy Role__: Reports on policy compliance
		- __Risk Management Communications Role__:
			- Informed by: Domain authority on risk appetite, policy, and performance target
			- Informs: Domain authority on policy compliance
	- AUDITOR: The auditor role is appointed by a super domain authority as subject matter expert to provide an independent audit service and reporting on the degree to which the risk appetite and policy of the super domain authority is being met by sub-domain authorities
		- __Role__: Responsible for auditing the performance of assets (attributes) in a specfic sub-domain on behalf of the owner of a super domain 
		- __Governance Model__: Design, Implement, Manage & Measure phases
		- __Policy Role__: Reports on policy compliance and procedure weaknesses
		- __Risk Management Communications Role__:
			- Informed by: Super domain authority on risk appetite, policy, and performance target
			- Informs: Super domain authority on policy compliance
  	- __Main takeaways__:
		- Auditor is external to the enterprise and provides INDEPENDENT audit and reporting services to the super domain authority.
		- Auditor role exists at the Design, Implement, Manage & Measure phases.
		- Compliance role is __internal__ and reports on policy compliance to the specific domain owner to which it is assigned.
		- Trustee role is a delegation of the domain owner role. Trustee is responsible for assets (attributes), and reports to super domain authority AND domain owner. 		 - Trustee exists at Strategy & Planning phase of the SABSA Governance model.
		- Custodian is appointed to be RESPONSIBLE for assets (attributes. Policy Authority is NOT delegated (unlike with trustees).
		- Custodian role exists at the Design, Implement, Manage & Measure phases.
		- Owner is accountable for performance of assets (attributes). Is the domain policy authority who sets goals, and risk appetite.
		- Owner exists at the Strategy and Planning phase.
- #### Risk Aggregation
	- Risk appetite and policy is communicated and distributed TOP-DOWN by the super domain authority in a SABSA domain model.
	- Risk performance and policy compliance is communicated and aggregated BOTTOM-UP to the super domain authority by the sub-domain authority in a SABSA domain model.

## Section 8 - Domain Concepts
- #### SABSA Domain Model Concept & Framework
  - __Benefits and Applications of Domain Models__:
    - Reduces complexity & delivers clarity
    - Controls resource segregation & enables information-sharing
    - Strategic concept that associates people with technology with policy
  - __Domain Registration Authority__:
    - Setting policy for domain
    - Verifying credentials of applicant
    - Establishing authentic indentity of applicant
    - Establishing right to be registered
    - Set operating practices and procedures
    - Revoke registrations
  - __Domain Certification Authority__:
    - Setting credentials issuing (certification)
    - Checking registration and authorisations
    - Publishing credentials and CRLs
    - Providing a chain of trust through hierachies
- #### Domain Definitions 
  - __Security Domain Definition__:
    - A security domain is a set of elements subject to a common security policy defined and owned by a single policy authority
  - __Super Domain Definition__:
    - A super domain is a set of elements subject to a common security policy defined and owned by a single security policy authority that contains one or more compliant subdomains, each with their own specific interpretation of the super domain policy
  - __Subdomain Definition__:
    - A subdomain is a set of elements subject to a security policy defined and owned by a single policy authority, that is derived from, and complies with, the policy of a higher authority
  - __Peer Domain Definition__:
    - Peer domains are subdomains sharing a common super domain policy with which they must comply
    - Super domain = common policy for ALL peer subdomains
    - Each peer domain has a specific compliant policy
   
## Section 9 - Time & Performance Management Concepts
- #### The SABSA Lifecycle
  - Properties of a Strategic Lifecycle
    - Strategy:
      - Setting out __long-term goals__ and plans for reaching those goals
      - Might have a beginning but never ends
      - Strategic organisations are in a state of constant change
    - Tactics:
      - Setting __medium-term goals__ and plans to achieve those goals
      - Have both a defined beginning and an end (they 'go-live')
      - Projects are tactical initiatives towards strategic goals
      - Alternatively, they address an immediate problem
    - Operations:
      - Deals with the __day-to-day__ job of keeping the business running
      - Based upon repetitive procedures that make up business processes
      - Developed through tactical projects, which in turn were driven by strategies
  - __SABSA Lifecycle Principals__:
    - Strongly business-driven
      - Regards it as mandatory that security demonstrably supports the business mission
    - Splits "Plan" into two (strategy & planning, and Design) to gain more granular traceability from business need to technical implementation and security management
    - "If you cannot measure you cannot manage"
    - SABSA view is mutually compatible with Deming's "Plan, Do, Check, Act"
  - __The SABSA Lifecycle Overlay__:
    - Strategy = Contextual & Conceptual Layers
    - Tactical = Logical, Physical, & Component Layers
    - Operations = Security Service Management Matrix

- #### Through-life Risk Managment Framework
  - Characteristics of Through-life Risk Management:
    - Establishes an appropriate infrastructure and culture and applies logical and systematic methods of establishing context, identifying, analysing, evaluating, treating, monitoring and communicating risks in a way that enables organisations to minimise losses and maximise gains
    - Provides governance by managing, communicating, and assuring risk treatment policies, targets, and practices through every phase of the lifecycle
    - Risk management activities performed through each phase of the SABSA lifecycle:
   - __Strategy & Planning__ - Business-driven Risk Management / Threats and Opportunities Inventory / Sets Risk appetite, and risk thresholds
     - Establish context: stakeholders, business drivers, attributes
     - Establish strategy: control objectives, enablement objectives, conceptual design
   - __Design__ - Risk activities designed based on the risk appetite and activities layed out in strategy and planning phase
     - Gap analysis of controls/enablers
     - Logical design; policies, services
     - Physical design; procedures, mechanisms
     - Components; tools and standards
     - Operations
   - __Implement__ - Implementation of risk mitigation policies, processes, & systems
     - Plan; proof of concept, roll out
     - Manage; implementation, training
     - Test; audit & review, system tests, process tests, penetration tests, UAT, OAT
   - __Manage & Measure__ - Risk management and measurement at lower layers and reported upwards to meet traceability requirements
     - Ops management; events, incidents
     - Assurance; audit & review, live pen tests
     - Monitoring; KPIs & KRIs, risk scorecard, risk dashboard
     - Improvements; capability maturity model (CMM) - Unreliable, Informal, Defined, Monitored, Optimised - SMP
  - Entrprise Lifecycle Risk Perspectives:
    - All risk management activities (strategic - long-term, tactical - medium-term, and operations - short-term) should support the over-arching business strategy for achieving long-term goals and objectives

- #### Process Improvement Framework
  - SABSA Maturity Model - SMP
    - Qualitative measurement technique for maturity of processes
    - Consistent, objective 5-point maturity scale
      1. Unreliable 
      2. Informal
      3. Defined
      4. Monitored
      5. Optimised
    - Provides gap analysis to drive a SABSA improvement programme
    - Each of the six SMP process areas (below) map onto the six cells of each row/layer of the SABSA Matrix corresponding to the particular SMP domain
    - Coordinates SABSA process information from all parts of the business
      - Demonstrates due diligence to senior management, auditors, and regulators
    - SABSA Maturity Profile Domains / SMP Process Areas:
      - The six SMP domains are:
        - Contextual architecture
	- Conceptual architecture
	- Logical architecture
	- Physical architecture
	- Component architecture
	- Service Management architecture
- #### Performance Management Framework
  - Slide 313
  - __Architecture Measurement Categories__
  	- __Completeness__
  	- __Assurance__
  	- __Compliance__
  	- __Performance__
  	- __Justification & significance__
  - Measurement Approaches
  	- High level statements of the approach to obtaining a measurement
	- Appropriate to the business need
	- In the language of the intended audience
	- Culturally specific
  - Measurement Guidelines
  	- Measurement should be a repeatable process (for comparison & prediction)
	- Measurement should have a clear communications role
	  - Tracking performance
	  - Assigning resources
	- Measurement should yield quantifible metrics (percentage, average, numbers, values, etc)
  - __Metrics Guidelines__
  	- Data used to calculate metrics should be readily obtainable
	- Metrics may (should) be calculated independently of parties with vested interest
	- The type of metric used may change in line with the maturity of the security process
	  - E.g. When you are highly compliant, consider changing from conformance measure to significance measure
	  - The more mature your organisation is in its security programme, the more defined and optimised the metrics should be
	- Performance metric / trend should be tested prior to going 'live'
	- Expectations management is key
  - __Types of Metrics__
  	- __Soft Metric__
	  - Qualitative
	  - Subjective
	  - Open to interpretation
	- __Hard Metric__
	  - Quantitative
	  - Objective
	  - Fixed, not open to interpretation
	- __Descriptive__
	  - Describes current-state of the object/attribute being measured
	- __Comparitive__
	  - Compares current-state of object/attribute with a similar object/attribute relating to a different place and/or time
	- __Predictive__
	  - Trend analysis in order to project and predict a future state
  - Conceptual Measures & Metrics Framework
  	- Business Requirement / Contextual level
	- Business Driver for Security / Derived from business requirements - conceptual abstraction
	- Attribute / Business Attributes Profile
	- Measurement Category (Completeness, Assurance, Compliance, Performance, Justification & Significance) - C.A.C.P.JS
	- Measurement Approach
	- Metric
- #### Through-life Architecture Vitality Framework
  - Slide 323
  - Through-life Vitality Framework
  	- A consistent set of principals, policies, capabilities, and standards that sets the direction and vision for the development and operation of the organisation's business information systems so as to ensure alignment with and support for the business needs
	- SABSA Guiding Principals to be an enabler of change
		- Provides the roadmap for joining together all of your requirements, whatever they might be, or become
  - __Architecture Vitality is the Architecture's capaciy to live, breathe and adapt its principals, policies, capabilities and standards such that it is viable in supporting dynamic business needs__
  - Each of the major SABSA Frameworks incorporates traceability from contextual requirements through solution design, implementation & management
  - The Manage & Measure Phase incorporates Feedback Loops for each in order to detect requirements to change the solutions
  - Vitality is achieved by adding to these feedback loops:
  	- Detection mechanism for brand new requirements
	- Architectural change management

# F2 Content

## Section 10 - Asset Architecture & Asset Management
- #### The SABSA Matrix - Deliverables of the SABSA Design Phase Layers
  - Design phase layers = Logical layer, Physical layer, Component layer
  - __Logical Architecture Layer__
  	- Concerned with *INFORMATION* security and system functionality
  	- __Information Assets__ (What / Assets)
	- __Risk Management Polcies__ (Why / Motivation)
	- __Process Maps & Services__ (How / Process)
	- __Entity & Trust Framework__ (Who / People)
	- __Domain Maps__ (Where / Location)
	- __Calendar & Timetable__ (When / Time)
 	- Elements exist in logical domains not tied to specific physical locations
  - __Physical Architecture Layer__
  	- Concerned with *DATA* security and infrastructure security
	- Elements exist in a specific physical domain and location
	- __Data Assets__ (What / Assets)
	- __Risk Management Practices__ (Why / Motivation)
	- __Process Mechanisms__ (How / Process)
	- __Human Interface__ (Who / People)
	- __ICT Infrastructure__ (Where / Location)
	- __Processing Schedule__ (When / Time)
  - __Component Architecture Layer__
  	- Specialised tools, brands, specific granular technical specifications & standards, protocols
	- __ICT Components__ (What / Assets)
	- __Risk Management Tools & Standards__ (Why / Motivation)
	- __Process Tools & Standards__ (How / Process)
	- __Personnel Management Tools & Standards__ (Who / People)
	- __Locator Tools & Standards__ (Where / Location)
	- __Step timing & sequencing__ (When / Time)
- #### Service Management
  - The objective of Release & Deployment Management is to build, test and deliver the capabilities and resources to provide the required services
  - A project (or any change) exists to:
  	- Improve current capabilities or performance
	- Introduce new capabilties
  - Knowledge is aggregated and contextualised through the SABSA Architecture layers
  - Knowledge management ensures that reliable information is available during the service lifecycle
  - The Service Management Layer maps to the SABSA Security Architecture layers:
  	- Contextual Layer (Business Wisdom)
	- Conceptual Layer (Business Knowledge)
	- Logical Layer (Business Information)
	- Physical & Component Layer (Business Data)
	- Service Management Layer (Knowledge Management) -> Maps to all of the above ^^

- #### SABSA Start-up Approaches
  - Executive interview approach
  	- Requires access to stakeholders, c-suite, senior executives
  - Analysis followed by validation
  	- No access to stakeholders
	- Team research & assumptions
	- Review, concensus, & sign-off of strategy
  - SABSA Fast-Track
  	- Full scope experience & proof-of-concept
	- Limited financial liability & commitment
	- Requires access to full team and stakeholders
  - Blended Approach
  	- Complex or distributed organisations often require a combination of the other three approaches
  - __Fast-Track Start-up Concept__
  	- Based on intensive facilitated workshops
	- Heavily customised to specific needs of organisation
	- Key programmes and risk priorities
        - Key players experience every aspect of the programme in a short time
	- Workshops run in parallel syndicates to ensure full scope is covered
	- Unlike other approaches, fast-track covers full scope of SABSA

## Section 11 - Risk & Policy Management Architecture
- #### Risk & Policy Management Architecture
  - Business risk and opportunities exist traceable through every layer of the architecture
  - Reponsibility for managing enterprise risks & opportunities is delegated to __Domains__
  - Each Domain Policy Authority:
  	- Operates within the risk appetite parameters of the super domain
	- Is compliant with the super domain policy
	- Has vested interest in risk performance within their own risk domain
	- Deploys specific controls and enablers to manage risk according to the architecture layer at which their domain exists
		- Right control, right place, at the right time
		- E.g. Network risk is managed by network controls and enablers deployed in the network domain according to network security policy
  - __Risk Level__
  	- LOGICAL LAYER: Business Risks & Opportunities to Logical Domains
	- PHYSICAL LAYER: Risk & Opportunities to Physical Environment & Infrastructure Domains
	- COMPONENT LAYER: Risks & Opportunities to System Components & Configuration
  - __Policy Level__
  	- LOGICAL LAYER: Appetite & Strategy articulated in Logical Policy
	- PHYSICAL LAYER: Managed by Physical Procudures derived from Policy
	- COMPONENT LAYER: Managed by Standards for Tools & Products
  - __Control Level__
  	- LOGICAL LAYER: Security Services
	- PHYSICAL LAYER: Security Mechanisms
	- COMPONENT LAYER: Security Components
  - __Service Management Activity Controls__
  	- LOGICAL: Management of Security Services (Logical)
	- PHYSICAL: Management of Infrastructure & Environment
	- COMPONENT: Management of Tools, Products, & Standards
  - SABSA Multi-Tiered Control Strategy
  	- Control Services - Logical
	- Control Mechanisms - Physical
	- Control Components - Component
	- __Deter__
  	- __Prevent__
  	- __Contain__
  	- __Detect__
  	  - Evidence & Track
  	- __Recover & Restore__
  	- __Assure__

  - Pure risk = 100% vulnerability, 100% weakness
  - Risk High = Risk is not proportional
  - Actuarial Data removes some subjectivity in initial rating by creating defined impact parameters & thresholds for risk appetite
  - Dynamic risk causes change in warning thresholds:
  	- High alert risk appetite spectrum means smaller percentage of acceptable risk level/threshold	

- #### SABSA Assurance Framework
  - Maps to the SABSA matrix (Assets, Motivation, Process, People, Location, Timeliness)
  - Maps to SABSA Lifecycle
  - __SABSA Assurance Defined__
  	- __Assurance__
	  - Providing confirmation and confidence that the enterprise risks are being adequately managed and that residual information risk is within the risk appetite or risk tolerence of the organisation
	- __Assurance Management__
	  - The process of managing assurance, including governing, planning and executing an enterprise assurance programme
	  - The process of providing assurance that the enterprise security architecture is:
	  	- BUSINESS-DRIVEN
		- COMPLETE
		- CONSISTENT
		- ROBUST
		- FIT-FOR-PURPOSE IN EVERY WAY
	- __Assurance Management Activities__
	  - The set of activities that comprise 'assurance management' 
	    - Audits
	    - Tests
	    - Reviews
	    - Checks & balances

  - SABSA Assurance Levels (4 levels)
  	- Level 1
	- Level 2
	- Level 3
	- Level 4
  	- Assurance levels are the ONLY part of the framework that can be customised/modified
	- __Assurance levels correlate to the risk levels__
		- Higher the risk level, higher the assurance level required
		- Lower the risk level, lower the assurance level required

## Section 12 - Transformation & Service Architecture
- #### Process Analysis
  - Vertical Consistency
  	- A requirement for a business process is expressed as an attribute with a performance target
	- A process is 'executed' by a series of progressively more granular steps down through each of the architecture layers
	- Vertical consistency means that the conceptual attribute required at the top of the process model must be accurately represented at each layer (or the requirement is not met)
	- Security services are the means of specifying and providing the required functionality at each layer
	
- #### Security Services
  - Business-driven requirements organised into a consistent, logical / functional specification
  - Derived exclusively from the contextual and conceptual layers above, especially:
  	- Attribute profile (with performance targets)
	- Control & enablement objectives (to defined risk appetite)
	- Domain model (organisation & infrastructure policy architecture)
	- Trust model (inter-domain service requirements)
  - __Primary Security Services__
  	- Primary security services are wholly embedded within a domain element
	- Self-contained within the element to provide security functionality that secures the element
  - __Secondary Security Services__
  	- Secondary security services operate between elements in a domain
	- They secure the communications between the elements
  - __Implicit Security Services__
  	- Implicit security services are implicit in a domain - they secure the domain from within
	  - E.g. Both primary and secondary services are providing "application security" from within the applications domain.
  - __Explicit Security Services__ 
	- Explicit security services are explicitly requested from one domain to another
	- Domain 1 and Domain 2 both have separate implicit security services that belong to each of their respective domains
	- An element in Domain 1 explicitly requests the security services of a service within domain 2

- #### Service Value & SLAs
  - SABSA Concept of Security Service Management
  	- Security service management is a set of specialised organisational capabilties for providing value to customers in the form of security services
	- Involves matching business requirements for control and enablers to available service provider resources and capabilities
	- Aims to make security capabilities and resources available to the customer in the highly usable form of security services that meet control and enablement objectives
	- Value is created by services that meet the customer's enablement AND control objective

## Section 13 - Entity & Trust Framework
- #### SABSA Trust Model
  - The Trust Concept
  	- Trust is a relational business attribute not a technical one
	- Trust is an important concept relevant to business relationships
	- Technical services are often used to support trusted interoperation between trusted entities
		- Certification Authority
		- Registration Authority: Establishes trust and authorises participation in a domain
  - Trust Models
  	- For two or more entities to interact and exchange information they must first trust each other
	- Trust is established through __registration__ by a mutually trusted third-party within a given domain (logical or physical)
	- All registered entities within a given domain trust one another within the domain policy
	- The technical mechanism needed to support trusted interaction is 'mutual authentication'
  - Relationships & Trust
  	- One-way Trust (simple)
	- Two-way Trust (complex)
	- Transitive or pass-through Trust
  - __Key points of trust and trust modelling__:
  	- Trust modelling in SABSA is about a clear specification of the business requirements for Trust, Security, and Control
  	- Logical trust model decomposition maps attributes to information flows
		- Progressing down to attributes mapping to services
  	- The direction of the trust arrows determines who is dependent upon security / control
  	- Trust strength is determined by strength of registration process
  - __Trust Roles & Participants__
  	- Trust Broker / Trusted Third-Party
		- Sells trust
		- Acts as the trusted third-party who is trusted by two or more individual domains
	- Claimant
		- Claims identity
		- Claims authority
		- Has been certified by the trust broker as being TRUSTED
	- Relying Party
		- Relying party is the TRUSTING party and is dependent on the claimant to claim identity
	- Registration Authority
		- Establishes trust and authorises participation in a domain
  - Business Entity Relationships
  	- Various levels of trust and information flows
	- Unilateral relationships
		- One party broadcasts or publishes information, others may receive it at their choice
	- Bilateral relationships
		- Two parties make a specific contract
	- Multilateral relationships
		- Group membership controlled by agreed rules

## Section 14 - Inter-Domain Security Associations
- #### Domain Associations
  - The SABSA method for achieving business engineering objectives is called "Securiy Associations Modelling"
  - Engineering Objectives
  	- The attributes profile created in the Conceptual Architecture represents the business requirements for security end-to-end of business processes
  - __Security Associations__
  	- Security associations exist at many levels
  	- Standards define Security Associations as the set of shared information that describes the security relationship between two entities, such as;
		- Cryptographic keys
		- Sequence numbers
		- Trusted time
		- Etc..
	- In SABSA, the security association is a LOGICAL representation of the business requirements for trust and security:
		- Intra-domain (between entities in a single domain)
		- Inter-domain (between entities in different domains)
	- A fully engineered set of security associations combine to deliver the required attribute end-to-end of the business process, irrespective of which domain boundaries are crossed, or how many
  - __End-to-End Security Objective__
  	- Domains exist at both LOGICAL and PHYSICAL levels
	- Logical domain associations - associations in and between
		- Business units, & lines of business
		- User communities & groups
	- Physical domain associations - associations in and between
		- Territories & jurisdictions
		- Buildings and sites
		- Infrastructure layer domains (networks, platforms, middleware...etc.)
  - __Extended Domain Concept__
  	- The extended domain concept is used when one domain policy authority must exert control over another in order to successfully manage their own risk
	- Effectively the dominant policy authority extends their domain into another - the stronger domain implants its policy into the 'territory' or another as a special sub-domain
	- Concept of ISP-owned CPE devices being used on customer premises.
	- Internet Service Provider owns the CPE and thus EXTENDS its security domain to the customer premises so as to exert policy over the CPE device.
	- Authentication server providing a 'security agent' to client PC's is the same concept of an extended domain




## Section 15 - Service Sequencing & Performance





