# OpenProperty Specification

## Overview

OpenProperty is an open-source real estate transparency and property intelligence platform designed to create a more informed, verifiable, and ethical real estate ecosystem.

OpenProperty provides a modular foundation for applications that support buyers, renters, sellers, landlords, agents, inspectors, contractors, engineers, attorneys, municipalities, and other participants in property transactions.

The platform is designed around the principle that property information should be discoverable, understandable, traceable, and verifiable. It combines AI-assisted analysis, jurisdiction-aware regulatory guidance, public records, property documents, professional verification, and structured due diligence workflows.

OpenProperty includes specialized applications such as HouseLens for buyers and renters and TrustLens for sellers and property owners.

## Mission

OpenProperty shall help transform real estate from a fragmented information system into a transparent property intelligence ecosystem.

The platform shall:

- Make property information easier to discover
- Identify missing information
- Analyze property disclosures
- Verify permits and compliance where data is available
- Identify zoning and land-use considerations
- Generate questions for sellers, landlords, municipalities, and professionals
- Recommend appropriate inspections
- Preserve evidence and source information
- Support informed decision-making
- Encourage complete and ethical disclosure
- Reduce information asymmetry between transaction participants
- Provide open-source infrastructure for future real estate applications

## Design Principles

OpenProperty shall be designed around the following principles:

- Transparency first
- Verification over assumption
- Location-aware intelligence
- State law and local regulation priority
- Comprehensive due diligence
- Human-in-the-loop decision making
- Explainable AI
- Open-source development
- Modular architecture
- Vendor-neutral infrastructure
- Interoperability
- Data provenance
- Privacy by design
- Security by design
- User ownership of information
- No unnecessary vendor lock-in
- Clear distinction between facts, claims, assumptions, recommendations, and unknowns

# Core Modules

## Property Identity Module

The Property Identity Module shall establish a consistent digital identity for each property.

The module shall support:

- Property address
- Geographic coordinates
- Parcel identifiers
- Tax identifiers where legally available
- Property type
- Current and historical use
- Jurisdiction
- Municipality
- County
- State
- Relevant regulatory authorities
- Property characteristics
- Associated records

The property identity shall provide the foundation for all other OpenProperty analysis.

## Jurisdiction Intelligence Module

The Jurisdiction Intelligence Module shall determine which laws, regulations, ordinances, disclosure requirements, and permitting requirements apply to a property.

The module shall identify:

- State requirements
- County requirements
- Municipal requirements
- Township requirements
- Zoning jurisdiction
- Building authority
- Code enforcement authority
- Rental authority
- Environmental authorities
- Other relevant governmental entities

All recommendations that depend on location shall reference the property's jurisdiction.

## Regulatory Intelligence Module

The Regulatory Intelligence Module shall organize applicable legal and regulatory information.

The module shall support:

- State disclosure requirements
- Property disclosure laws
- Rental regulations
- Zoning requirements
- Building codes
- Permit requirements
- Occupancy requirements
- Inspection requirements
- Rental registration requirements
- Local property regulations
- HOA-related restrictions where applicable

The system shall maintain effective dates and source references where available.

OpenProperty shall not present generalized information as jurisdiction-specific legal advice.

## Property Disclosure Module

The Property Disclosure Module shall provide a common framework for analyzing and managing property disclosures.

The module shall:

- Accept disclosure documents
- Extract structured information
- Analyze disclosure completeness
- Identify unanswered questions
- Identify ambiguous responses
- Identify contradictions
- Compare disclosures with applicable requirements
- Generate follow-up questions
- Identify areas requiring professional review
- Preserve source documents and evidence

The system shall distinguish information disclosed by a property owner from information independently verified by OpenProperty.

## Missing Information Module

The Missing Information Module shall identify information that should be obtained before a user proceeds with a property transaction.

Potential missing information includes:

- Property disclosures
- Permit records
- Inspection records
- Certificates
- Renovation documentation
- Repair records
- Contractor documentation
- Zoning information
- HOA documents
- Rental documentation
- Environmental records
- Insurance-related information where legally available

The module shall generate actionable requests rather than simply reporting that information is missing.

## Question Intelligence Module

The Question Intelligence Module shall generate customized questions based on the property, transaction type, jurisdiction, documents, records, and identified risks.

Questions may be directed to:

- Sellers
- Landlords
- Listing agents
- Property managers
- Township officials
- Municipal officials
- County officials
- HOA representatives
- Inspectors
- Engineers
- Contractors
- Attorneys
- Other qualified professionals

Questions shall be prioritized according to:

- Legal relevance
- Safety implications
- Financial significance
- Transaction importance
- Uncertainty
- Potential property impact
- Time sensitivity

## Permit Intelligence Module

The Permit Intelligence Module shall analyze property improvements and determine which permits, inspections, or approvals may need to be investigated.

Supported improvements may include:

- Additions
- Sunrooms
- Decks
- Porches
- Garages
- Finished basements
- Finished attics
- Structural modifications
- Electrical work
- Plumbing work
- HVAC installations
- Roofing
- Windows
- Doors
- Pools
- Spas
- Solar systems
- Generators
- Accessory dwelling units
- Outbuildings
- Other material improvements

The module shall identify records that should exist based on available information and applicable requirements.

An absent public record shall not automatically be interpreted as proof that work was unpermitted.

## Zoning and Land Use Module

The Zoning and Land Use Module shall analyze property use and applicable land-use restrictions.

The module shall support:

- Zoning classification
- Permitted uses
- Conditional uses
- Setbacks
- Lot requirements
- Accessory structures
- Home occupations
- Rental restrictions
- Short-term rental restrictions
- Development restrictions
- Easements where available
- Variances
- Special exceptions
- Other land-use considerations

The module shall generate questions and verification requests when zoning information may affect the intended use of a property.

## Public Records Module

The Public Records Module shall organize and analyze legally accessible public property information.

Supported records may include:

- Property records
- Tax records
- Assessment records
- Permit records
- Zoning records
- Code enforcement records
- Occupancy records
- Planning records
- Public notices
- Environmental records
- Flood records
- Municipal records
- Other official records

Official records shall be distinguished from third-party sources.

## Document Intelligence Module

The Document Intelligence Module shall process property-related documents.

Supported documents may include:

- Disclosure forms
- Inspection reports
- Permit documents
- Certificates
- Contractor invoices
- Repair records
- Warranties
- HOA documents
- Lease agreements
- Rental disclosures
- Survey documents
- Environmental reports
- Zoning documents
- Municipal correspondence

The module shall support:

- OCR
- Document classification
- Information extraction
- Entity extraction
- Date extraction
- Issue identification
- Cross-document comparison
- Missing information detection
- Source preservation

## Property Systems Module

The Property Systems Module shall organize information about major property systems.

Supported systems may include:

- Foundation
- Structure
- Roof
- Electrical
- Plumbing
- HVAC
- Water heating
- Sewer
- Septic
- Well
- Drainage
- Windows
- Doors
- Insulation
- Fire safety
- Chimneys
- Appliances
- Pools
- Solar systems
- Generators
- Other material systems

The module shall track available documentation, reported conditions, inspection status, age where available, and unresolved questions.

## Inspection Intelligence Module

The Inspection Intelligence Module shall determine which property systems may require evaluation by qualified professionals.

Recommendations may include:

- General home inspection
- Structural engineer
- Licensed electrician
- Licensed plumber
- HVAC professional
- Roofing professional
- Chimney professional
- Pest professional
- Environmental professional
- Mold professional
- Septic professional
- Well professional
- Pool professional
- Other appropriately qualified specialists

Each recommendation shall explain:

- Why the inspection may be appropriate
- What should be examined
- What evidence triggered the recommendation
- What professional qualification may be appropriate

AI recommendations shall not substitute for professional inspection or engineering judgment.

## Risk Intelligence Module

The Risk Intelligence Module shall identify potential areas of concern.

Risk categories may include:

- Structural risk
- Water intrusion
- Electrical risk
- Plumbing risk
- HVAC risk
- Environmental risk
- Permit risk
- Zoning risk
- Disclosure risk
- Rental compliance risk
- Documentation risk
- Financial risk
- Insurance-related risk
- Data inconsistency
- Unknown property condition

Each finding shall include available evidence, uncertainty, recommended actions, and source information.

## Evidence and Provenance Module

The Evidence and Provenance Module shall preserve the origin and status of information.

The module shall track:

- Source
- Source type
- Source URL where applicable
- Document
- Date obtained
- Jurisdiction
- Relevant record
- Extracted information
- Verification status
- Confidence
- User-provided claims
- Professional verification

The system shall distinguish:

- Verified facts
- Official records
- User-provided information
- Seller-provided information
- Landlord-provided information
- AI-generated inference
- Unverified claims
- Unknown information

## AI Intelligence Module

The AI Intelligence Module shall provide the reasoning and analysis layer across OpenProperty.

AI capabilities shall include:

- Document analysis
- Disclosure analysis
- Regulatory analysis
- Question generation
- Risk detection
- Permit reasoning
- Zoning analysis
- Inspection recommendations
- Information comparison
- Missing information detection
- Due diligence prioritization
- Natural language explanations
- Report generation

AI-generated results shall include appropriate uncertainty indicators and supporting evidence where possible.

## Due Diligence Module

The Due Diligence Module shall convert property intelligence into an actionable workflow.

The module shall:

- Create due diligence checklists
- Track questions
- Track document requests
- Track government requests
- Track inspections
- Track professional reviews
- Track responses
- Track unresolved issues
- Track deadlines
- Prioritize outstanding actions
- Record user decisions

## Transaction Intelligence Module

The Transaction Intelligence Module shall organize information throughout the transaction lifecycle.

Supported stages may include:

- Property discovery
- Initial evaluation
- Disclosure review
- Offer preparation
- Contract period
- Inspection period
- Due diligence
- Financing
- Appraisal
- Closing preparation
- Post-closing property record

The module shall identify outstanding information and recommended actions at each stage.

## Transparency Assessment Module

The Transparency Assessment Module shall evaluate how thoroughly a property has been documented and investigated.

Assessment factors may include:

- Disclosure completeness
- Permit verification
- Renovation documentation
- Inspection documentation
- Public record verification
- Zoning verification
- Regulatory compliance
- Unresolved questions
- Missing documents
- Professional verification

Transparency assessments shall never be represented as guarantees of property quality, legality, safety, or value.

## Property Transparency Passport Module

The Property Transparency Passport Module shall provide a structured, shareable summary of verified property information.

The passport may include:

- Property identity
- Disclosure history
- Permit history
- Renovations
- Inspections
- Repairs
- Certificates
- Zoning information
- Compliance information
- Verification records
- Supporting evidence
- Outstanding questions

Information shall only be included according to appropriate authorization, provenance, privacy, and legal requirements.

## Property History Module

The Property History Module shall organize available historical information about a property.

Potential information includes:

- Previous disclosures
- Permits
- Renovations
- Repairs
- Inspections
- Ownership changes where legally available
- Property use changes
- Code enforcement
- Zoning changes
- Other verifiable historical events

The module shall preserve source provenance and distinguish historical records from current conditions.

## User and Access Control Module

The User and Access Control Module shall manage user identities and permissions.

Supported roles may include:

- Buyer
- Renter
- Seller
- Landlord
- Agent
- Inspector
- Engineer
- Contractor
- Attorney
- Administrator
- Data provider
- Developer

Permissions shall be based on the user's authorized access to property information.

## Privacy and Security Module

The Privacy and Security Module shall protect property and user information.

The module shall support:

- Secure authentication
- Authorization
- Encryption in transit
- Encryption at rest where applicable
- Secure document storage
- Access controls
- Audit logging
- Data minimization
- Configurable retention
- Secure deletion
- Privacy-conscious AI processing

## Reporting Module

The Reporting Module shall generate structured property intelligence reports.

Reports may include:

- Property overview
- Disclosure analysis
- Regulatory requirements
- Missing information
- Permit findings
- Zoning findings
- Inspection recommendations
- Risk findings
- Questions
- Document requests
- Due diligence status
- Evidence
- Source references
- Outstanding issues

Reports shall clearly distinguish verified information from unresolved information.

## Notification and Workflow Module

The Notification and Workflow Module shall help users manage time-sensitive property tasks.

It may support:

- Due diligence deadlines
- Inspection scheduling
- Document requests
- Government requests
- Follow-up reminders
- Missing information alerts
- Status changes
- Transaction milestones

## Interoperability Module

OpenProperty shall provide standardized interfaces for exchanging property intelligence.

The module shall support, where practical:

- REST APIs
- Structured property data
- Structured document metadata
- Geographic data
- Evidence records
- Property identifiers
- Portable reports
- Plugin interfaces
- AI provider interfaces
- Data source interfaces

## Developer and Extension Module

The Developer and Extension Module shall provide documented interfaces for extending OpenProperty.

Developers shall be able to create:

- Regulatory modules
- AI modules
- Public data connectors
- Municipal integrations
- Inspection systems
- Document processors
- Mapping integrations
- Reporting systems
- User interfaces
- Professional services integrations

Extensions shall not require unnecessary modification of the OpenProperty core.

# Specialized Applications

## HouseLens
[https://roxanneardary.com/houselens/](https://roxanneardary.com/houselens/)  

HouseLens shall provide the buyer and renter experience within the OpenProperty ecosystem.

HouseLens shall focus on:

- Property due diligence
- Disclosure analysis
- Missing disclosure questions
- Permit investigation
- Zoning research
- Inspection recommendations
- Public record analysis
- Seller and landlord questions
- Township and municipal questions
- Risk analysis
- Transaction preparation

## TrustLens
[https://roxanneardary.com/trustlens/](https://roxanneardary.com/trustlens/)  

TrustLens shall provide the seller and property owner experience within the OpenProperty ecosystem.

TrustLens shall help users:

- Prepare disclosures
- Identify required documentation
- Anticipate buyer questions
- Verify renovations
- Identify permits that should be investigated
- Prepare inspection documentation
- Gather municipal records
- Identify potential compliance issues
- Improve listing transparency
- Prepare a property for due diligence

# Optional Plugin Modules

## Municipal Records Plugin

Provides connections to participating municipal and county record systems.

Capabilities may include:

- Permit history
- Certificates
- Code enforcement records
- Occupancy records
- Zoning information
- Property records

## Permit Database Plugin

Connects OpenProperty to compatible permit databases.

Capabilities may include:

- Permit searches
- Permit status
- Permit dates
- Permit types
- Inspection records
- Final approvals

## Zoning Data Plugin

Provides zoning information and geographic land-use data.

Capabilities may include:

- Zoning classifications
- Zoning maps
- Ordinances
- Setbacks
- Permitted uses
- Variances
- Special exceptions

## Property Tax Plugin

Provides compatible tax and assessment information.

Capabilities may include:

- Assessments
- Tax history
- Property classifications
- Tax status
- Public assessment records

## Environmental Data Plugin

Provides environmental and hazard information.

Potential data sources include:

- Flood information
- Environmental contamination records
- Wetlands
- Hazard areas
- Radon information
- Other legally accessible environmental datasets

## HOA Intelligence Plugin

Analyzes HOA and condominium association information.

Capabilities may include:

- Covenants
- Restrictions
- Fees
- Assessments
- Rules
- Rental restrictions
- Architectural restrictions
- Meeting documents
- Financial documents

## Rental Compliance Plugin

Provides jurisdiction-specific rental analysis.

Capabilities may include:

- Rental registration
- Occupancy requirements
- Rental inspections
- Landlord requirements
- Tenant protections
- Security deposit requirements
- Local rental restrictions

## Insurance Intelligence Plugin

Provides property insurance research and risk analysis where legally and technically available.

Capabilities may include:

- Insurance questions
- Claims-related information where authorized
- Property risk factors
- Insurance documentation
- Coverage considerations

## Contractor Verification Plugin

Provides contractor and professional credential verification.

Capabilities may include:

- License verification
- License status
- Credential information
- Expiration dates
- Disciplinary records where publicly available

## Professional Services Plugin

Provides optional connections to qualified professionals.

Supported categories may include:

- Inspectors
- Engineers
- Electricians
- Plumbers
- HVAC professionals
- Roofers
- Environmental professionals
- Attorneys
- Other qualified specialists

## OCR Plugin

Provides OCR capabilities for scanned property documents.

## Mapping Plugin

Provides geographic visualization of property information.

Capabilities may include:

- Parcel boundaries
- Zoning
- Flood zones
- Environmental conditions
- Nearby infrastructure
- Property context

## Local AI Plugin

Allows OpenProperty installations to use locally hosted AI models.

The plugin shall support privacy-conscious deployments where property documents and personal information should remain within the user's infrastructure.

## External AI Provider Plugin

Allows users to configure compatible external AI services.

The plugin architecture shall make provider selection configurable and shall avoid requiring a single AI vendor.

## Notification Plugin

Provides optional notification services for:

- Email
- Messaging
- Calendar
- Due diligence deadlines
- Document requests
- Transaction milestones

## Export Plugin

Provides export functionality for:

- Property reports
- Transparency Passports
- Due diligence records
- Evidence packages
- Question lists
- Document inventories

# Data Architecture

OpenProperty shall treat property information as structured, traceable data rather than isolated documents.

Core data entities may include:

- Property
- Parcel
- Jurisdiction
- Disclosure
- Document
- Permit
- Inspection
- Renovation
- Repair
- Regulation
- Zoning Record
- Public Record
- Risk
- Question
- Request
- Professional
- Verification
- Evidence
- Transaction
- User
- Organization

Each entity should support provenance and verification status where applicable.

# Verification Framework

OpenProperty shall use a verification framework that categorizes information according to its evidentiary status.

Possible statuses include:

- Verified
- Official Record
- Professionally Verified
- User Provided
- Seller Provided
- Landlord Provided
- Reported
- AI Inferred
- Unverified
- Conflicting
- Unknown

The system shall not silently convert uncertain information into verified facts.

# AI Governance

OpenProperty AI systems shall follow transparent and accountable design principles.

AI systems shall:

- Identify the basis for important recommendations
- Provide source references where available
- Express uncertainty
- Avoid fabricating records
- Avoid inventing laws or regulations
- Identify missing information
- Recommend human verification when appropriate
- Preserve user control
- Avoid discriminatory decision-making
- Avoid making unsupported legal conclusions

# Ethical Real Estate Requirements

OpenProperty shall be designed to promote ethical real estate transactions.

The platform shall:

- Encourage truthful disclosure
- Identify potentially incomplete information
- Help users discover material questions
- Promote professional verification
- Avoid assisting users in concealing property conditions
- Avoid discriminatory property recommendations
- Protect sensitive information
- Maintain clear AI limitations
- Support informed consent
- Preserve evidence and provenance

# Open Data and Public Information

OpenProperty shall prioritize lawful access to public information.

Integrations shall respect:

- Government data policies
- Terms of use
- Licensing requirements
- Privacy requirements
- Copyright
- Database rights where applicable
- Rate limits
- Access restrictions

OpenProperty shall not require unauthorized scraping or circumvention of access controls.

# Security Requirements

OpenProperty shall implement security controls appropriate to the sensitivity of property and personal information.

Security requirements shall include:

- Secure authentication
- Least-privilege access
- Secure session management
- Encryption
- Audit logging
- Secure file handling
- Input validation
- API authentication
- Dependency management
- Security testing
- Vulnerability reporting procedures

# Privacy Requirements

OpenProperty shall minimize collection and retention of personal information.

Users shall have appropriate controls over:

- Uploaded documents
- Personal information
- Property information
- Sharing permissions
- Retention
- Deletion
- External AI processing

Sensitive information shall not be shared with third-party services without appropriate authorization.

# Interoperability and Vendor Independence

OpenProperty shall remain usable without dependence on a single commercial provider.

The system shall support interchangeable:

- AI providers
- Database systems
- Public data sources
- Mapping providers
- Notification services
- Document processors
- Authentication systems

Where practical, interfaces shall use documented and portable formats.

# Local-First Support

OpenProperty should support local-first deployments.

Local deployments should be capable of:

- Storing property documents locally
- Running compatible AI models locally
- Processing documents locally
- Maintaining local property records
- Operating with limited external dependencies

External integrations may be enabled when users choose them.

# Open Source Development

OpenProperty shall remain modular and accessible to developers.

Contributors may improve:

- Core modules
- AI systems
- Regulatory knowledge
- Data integrations
- Document analysis
- Inspection intelligence
- Security
- Privacy
- User interfaces
- Reporting
- Accessibility
- Internationalization

The project shall encourage collaboration among developers, real estate professionals, inspectors, engineers, attorneys, researchers, municipalities, and public-data contributors.

# Future Property Intelligence Network

OpenProperty should evolve toward a property intelligence network in which authorized information can move with the property throughout its lifecycle.

Potential capabilities include:

- Persistent property identity
- Long-term property history
- Verified renovation records
- Permit history
- Inspection history
- Disclosure history
- Compliance history
- Evidence provenance
- Property Transparency Passport
- Authorized data sharing
- Transaction intelligence
- Post-closing property records

The system shall preserve privacy, authorization, provenance, and legal compliance as these capabilities develop.

# Success Criteria

OpenProperty shall be considered successful when it enables users to:

- Understand the legal context of a property
- Identify applicable disclosure requirements
- Analyze property disclosures
- Detect missing information
- Verify available public records
- Investigate permits
- Evaluate zoning considerations
- Generate questions
- Request appropriate documentation
- Identify appropriate professional inspections
- Track due diligence
- Understand property risks
- Trace findings to evidence
- Distinguish verified information from unknown information
- Make better-informed real estate decisions

# Limitations and Professional Review

OpenProperty is an information and decision-support platform.

It does not replace:

- Attorneys
- Licensed inspectors
- Engineers
- Contractors
- Appraisers
- Insurance professionals
- Government officials
- Financial professionals
- Other qualified professionals

Users should seek professional advice when required or appropriate.

AI-generated recommendations shall not be treated as professional determinations.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/openproperty/](https://roxanneardary.com/openproperty/)

---

## License & Notice Requirements

OpenProperty is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- OpenProperty specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
