# SABSA Chartered Security Architect
### January 2021

---

SABSA Certification Study // Exam Preparation

# F1 Content
## Section 1 - SABSA Principals & Objectives
- #### Enterprise Security Architecture Framework
  - A consistent set of principals, policies, capabilities and standards that sets the direction and vision for the development and operation of the organisation's business information systems so as to ensure alignment with and support for the business needs.
- #### SABSA Guiding Principals
- #### Holistic Approach
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
   
   
   
  
# F2 Content
