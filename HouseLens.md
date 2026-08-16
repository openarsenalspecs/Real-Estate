# HouseLens Specification
**From Unknowns to Insights.**
- HTML Mirror:  [https://roxanneardary.com/houselens-specification/](https://roxanneardary.com/houselens-specification/)

---

## Overview

HouseLens is an open-source AI-powered property intelligence platform designed to give home buyers and renters comprehensive transparency throughout the property evaluation and transaction process.

HouseLens analyzes property disclosures, documents, public records, legal requirements, permits, zoning information, inspection requirements, and other available property information. The platform uses the property's location as a primary context so that recommendations and evaluations prioritize the laws, regulations, disclosure requirements, and permitting practices applicable to that property.

HouseLens is designed to help users identify unknowns before they become costly surprises. The system does not replace attorneys, licensed inspectors, engineers, contractors, government officials, landlords, sellers, or other qualified professionals. Instead, it identifies questions that should be asked, records that should be obtained, and professional evaluations that may be appropriate.

---

## Design Principles

HouseLens shall be designed around the following principles:

- Transparency first
- Buyer and renter protection
- Location-aware analysis
- State law and local regulation awareness
- Comprehensive due diligence
- Human review and professional verification
- Explainable AI recommendations
- Open-source development
- Local-first operation where practical
- Vendor-neutral architecture
- Data privacy and security
- No unnecessary vendor lock-in
- Clear distinction between verified facts, reported information, assumptions, and recommendations

## Core Modules

### Property Context Module

The Property Context Module establishes the legal and geographic context for every property evaluated by HouseLens.

The module shall:

- Identify the property location
- Determine the applicable state
- Determine applicable county or equivalent jurisdiction
- Determine applicable municipality, township, city, or local authority
- Identify known zoning jurisdiction
- Identify applicable property type
- Identify whether the property is intended for purchase or rental
- Record relevant property characteristics
- Establish the regulatory context used by the analysis engine
- Maintain source references for location-based determinations

All subsequent recommendations shall use the established property context whenever applicable.

### Disclosure Analysis Module

The Disclosure Analysis Module shall analyze property disclosures provided by sellers, landlords, owners, agents, or other authorized sources.

The module shall:

- Accept uploaded disclosure documents
- Extract structured information from documents
- Identify disclosed defects and conditions
- Identify incomplete responses
- Detect unanswered questions
- Identify ambiguous statements
- Identify potentially contradictory information
- Compare disclosures against applicable state requirements
- Compare disclosed information against other available property records
- Generate follow-up questions
- Identify documentation that should be requested
- Identify issues that may require professional evaluation

The module shall distinguish between information explicitly disclosed, information inferred by the system, and information that remains unknown.

### Missing Disclosure Module

If a property disclosure is not provided, the Missing Disclosure Module shall generate a comprehensive property question set.

The question set shall be based on:

- Property location
- State disclosure requirements
- Property type
- Age of the property
- Known renovations
- Available public records
- Available permit information
- Environmental conditions
- Known property systems
- Rental requirements where applicable

Questions shall cover, where relevant:

- Structural conditions
- Roof
- Foundation
- Basement
- Crawl spaces
- Water intrusion
- Mold
- Plumbing
- Electrical systems
- HVAC
- Water heating
- Sewer or septic systems
- Well systems
- Windows and doors
- Insulation
- Fire safety
- Pest activity
- Flooding
- Drainage
- Environmental hazards
- Previous repairs
- Insurance claims
- Property damage
- Renovations
- Additions
- Code compliance
- Zoning
- Easements
- Shared structures
- HOA requirements
- Rental history
- Tenant history
- Known disputes
- Pending assessments
- Other material property conditions

### State Disclosure Compliance Module

The State Disclosure Compliance Module shall use property location to identify applicable state-regulated disclosure requirements.

The module shall:

- Maintain jurisdiction-specific disclosure rules
- Identify required disclosure categories
- Compare provided disclosures against applicable requirements
- Identify potentially missing information
- Generate jurisdiction-specific questions
- Identify areas requiring legal or professional review
- Maintain citations or source references for regulatory information
- Track effective dates of applicable requirements

The module shall avoid presenting general guidance as jurisdiction-specific legal advice.

### Local Regulation Module

The Local Regulation Module shall evaluate municipal and local requirements affecting the property.

The module shall support analysis of:

- Township requirements
- Municipal codes
- Zoning requirements
- Building requirements
- Occupancy requirements
- Certificate requirements
- Permit procedures
- Inspection requirements
- Local property restrictions
- Rental requirements
- Short-term rental requirements where applicable
- Local environmental requirements
- Local land-use restrictions

The module shall generate recommended questions and records to request from the appropriate local authority.

### Permit and Renovation Module

The Permit and Renovation Module shall identify improvements and alterations that may require permits or inspections.

The module shall analyze information concerning:

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
- Outbuildings
- Accessory dwelling units
- Solar installations
- Generators
- Other material improvements

For each applicable improvement, the system shall determine whether documentation should be requested and whether municipal verification may be appropriate.

The system shall identify permits that appear to be expected based on available information but shall not represent an absent record as definitive proof that work was unpermitted.

### Public Records Module

The Public Records Module shall organize and analyze publicly available property information.

Supported information may include:

- Property records
- Tax records
- Permit records
- Zoning records
- Assessment records
- Code enforcement records
- Public notices
- Planning records
- Flood information
- Environmental records
- Municipal records
- Other legally accessible public information

The module shall maintain source information and distinguish official records from third-party data.

### Question Generation Module

The Question Generation Module shall transform findings into actionable questions.

Questions shall be categorized by recipient, including:

- Seller
- Landlord
- Listing agent
- Property manager
- Township
- Municipality
- County
- HOA
- Inspector
- Contractor
- Engineer
- Attorney
- Utility provider
- Other relevant authority

The system shall prioritize questions according to potential importance, uncertainty, legal relevance, financial impact, safety implications, and transaction timing.

### Inspection Recommendation Module

The Inspection Recommendation Module shall identify property systems that may warrant examination by qualified professionals.

Recommendations may include:

- General home inspection
- Structural engineer
- Electrical contractor
- Licensed electrician
- Licensed plumber
- HVAC professional
- Roofing professional
- Chimney professional
- Pest professional
- Mold professional
- Environmental professional
- Septic professional
- Well professional
- Pool professional
- Other appropriately qualified specialists

Recommendations shall explain why an inspection may be appropriate and identify the information or condition the professional should evaluate.

HouseLens shall not represent AI analysis as a substitute for professional inspection or engineering judgment.

### Document Request Module

The Document Request Module shall generate customized document request lists.

Potential requests include:

- Property disclosures
- Permits
- Final inspection records
- Certificates of occupancy
- Certificates of compliance
- Renovation records
- Contractor invoices
- Warranties
- Inspection reports
- Repair records
- Insurance claims information where legally obtainable
- HOA documents
- Tax records
- Utility records where appropriate
- Survey documents
- Environmental reports
- Zoning documentation
- Rental records where appropriate

### Risk Analysis Module

The Risk Analysis Module shall identify potential areas requiring additional investigation.

Risk categories shall include:

- Structural risk
- Water intrusion risk
- Electrical risk
- Plumbing risk
- HVAC risk
- Environmental risk
- Permit risk
- Zoning risk
- Disclosure risk
- Rental compliance risk
- Financial risk
- Documentation risk
- Data inconsistency
- Unknown property condition

Risk results shall include supporting evidence, uncertainty indicators, recommended actions, and relevant sources where available.

### Transparency Assessment Module

The Transparency Assessment Module shall evaluate how completely a property has been documented.

The assessment may consider:

- Disclosure completeness
- Permit documentation
- Inspection documentation
- Renovation records
- Public record verification
- Zoning information
- Compliance information
- Known risks
- Unresolved questions
- Missing documents
- Professional inspection recommendations

The system may produce a transparency assessment, but it shall not imply that a numerical score guarantees property quality, safety, legality, or value.

### Due Diligence Workflow Module

The Due Diligence Workflow Module shall organize the user's investigation into actionable steps.

The workflow shall:

- Identify outstanding questions
- Identify missing documents
- Identify records requiring verification
- Identify recommended inspections
- Track completed requests
- Track responses
- Track unresolved issues
- Record user notes
- Establish transaction deadlines where supplied by the user
- Prioritize actions according to urgency and importance

### Evidence and Source Module

The Evidence and Source Module shall provide traceability for AI-generated findings.

Each material finding should identify, where available:

- Source document
- Public record source
- Government source
- Date obtained
- Relevant jurisdiction
- Extracted evidence
- Confidence level
- Verification status

The system shall clearly distinguish verified information from unverified statements.

### AI Analysis Module

The AI Analysis Module shall provide the intelligence layer across HouseLens.

AI capabilities shall include:

- Document analysis
- Disclosure analysis
- Question generation
- Risk identification
- Permit reasoning
- Regulatory guidance
- Inspection recommendations
- Information comparison
- Missing information detection
- Due diligence prioritization
- Natural language explanations

AI-generated conclusions shall be presented as recommendations or analysis rather than automatically treated as legal, engineering, inspection, or financial determinations.

### User Review Module

The User Review Module shall keep humans in control of important decisions.

Users shall be able to:

- Review AI findings
- Correct extracted information
- Reject recommendations
- Mark information as verified
- Add notes
- Upload supporting documents
- Request additional analysis
- Track professional responses
- Export findings

### Privacy and Security Module

The Privacy and Security Module shall protect sensitive property and user information.

The module shall support:

- Secure authentication
- Authorization controls
- Encryption in transit
- Encryption at rest where applicable
- Secure document handling
- Access logging
- Data minimization
- Configurable retention
- Secure deletion
- Privacy-conscious AI processing

### Reporting Module

The Reporting Module shall generate organized reports for users.

Reports may include:

- Property overview
- Disclosure analysis
- Missing information
- Questions for sellers or landlords
- Questions for municipalities
- Permit findings
- Zoning findings
- Inspection recommendations
- Risk findings
- Document checklist
- Outstanding due diligence
- Source references

Reports shall clearly identify information that remains unresolved.

## Optional Plugin Modules

HouseLens shall support optional plugins so functionality can be expanded without requiring every installation to include every integration.

### Municipal Records Plugin

Provides integrations with participating municipal and county record systems.

### Permit Database Plugin

Connects to permit databases and supports automated permit history retrieval.

### Zoning Data Plugin

Provides zoning maps, classifications, ordinances, and related municipal information.

### Property Tax Plugin

Provides property assessment and tax information from supported public sources.

### Flood and Environmental Data Plugin

Integrates legally accessible environmental and hazard datasets.

### HOA Document Plugin

Analyzes association documents, restrictions, fees, assessments, rules, and disclosures.

### Rental Compliance Plugin

Provides jurisdiction-specific rental registration, inspection, occupancy, and landlord compliance analysis.

### Insurance Risk Plugin

Analyzes available property insurance information and identifies questions regarding prior claims, coverage requirements, and insurability.

### Contractor Verification Plugin

Provides verification support for contractor licensing and relevant professional credentials.

### Professional Referral Plugin

Allows users to locate qualified inspectors, engineers, contractors, attorneys, and other professionals.

### Public Data Connector Plugin

Provides connectors for compatible government and public-data systems.

### Local AI Plugin

Allows installations to use locally hosted AI models for privacy-sensitive analysis.

### External AI Provider Plugin

Allows users or administrators to configure compatible external AI providers when desired.

### OCR Plugin

Provides optical character recognition for scanned disclosures, permits, reports, and other documents.

### Mapping Plugin

Provides geographic visualization of property boundaries, zoning, environmental conditions, nearby infrastructure, and other relevant information.

### Notification Plugin

Provides optional email, messaging, calendar, or deadline notifications.

### Export Plugin

Supports exporting reports and due diligence records to compatible document formats.

### Integration Plugin Framework

The plugin architecture shall support third-party modules without requiring modifications to the HouseLens core.

Plugins should define:

- Capabilities
- Permissions
- Data requirements
- Data sources
- Configuration options
- Privacy requirements
- Failure behavior
- Version compatibility

## Rental Support

HouseLens shall support both buyers and renters.

Rental analysis may include:

- Lease document analysis
- Rental disclosure analysis
- Landlord question generation
- Property condition questions
- Required rental inspections
- Occupancy requirements
- Rental registration
- Security deposit requirements
- Habitability considerations
- Utility responsibilities
- HOA rental restrictions
- Local rental regulations
- Property management documentation

Rental recommendations shall prioritize the laws applicable to the property's location.

## Buyer Support

Buyer workflows shall include:

- Property research
- Disclosure analysis
- Missing disclosure questions
- Permit verification
- Zoning research
- Inspection recommendations
- Document requests
- Seller questions
- Township questions
- Risk identification
- Due diligence tracking
- Pre-closing review

## AI-Assisted Township and Government Requests

HouseLens shall generate customized requests that users can submit to relevant government offices.

Requests may concern:

- Permit history
- Final inspections
- Certificates
- Zoning
- Occupancy
- Code violations
- Property use
- Local restrictions
- Required approvals

The system shall identify the appropriate authority when that information is available.

## Transaction Readiness

HouseLens shall provide a transaction readiness view showing:

- Completed due diligence
- Outstanding questions
- Missing documentation
- Unverified claims
- Recommended inspections
- Potential risks
- Regulatory questions
- User decisions

The system shall help users understand what remains unknown before proceeding.

## Explainability Requirements

HouseLens AI recommendations shall provide understandable explanations.

Where practical, each recommendation shall identify:

- What was detected
- Why it matters
- What evidence supports the finding
- What remains unknown
- What the user should do next
- Who should be contacted
- Whether professional verification is recommended

## Ethical Requirements

HouseLens shall be designed to support ethical real estate transactions.

The system shall:

- Promote complete and truthful disclosure
- Avoid facilitating concealment of material property conditions
- Identify potentially misleading information
- Encourage professional verification
- Avoid discriminatory recommendations
- Avoid making decisions based on protected characteristics
- Protect sensitive user information
- Clearly disclose limitations of AI-generated analysis

Core functionality shall not depend on a single commercial provider.

## Future Property Transparency Record

HouseLens should support integration with a persistent property transparency record.

The record may eventually contain:

- Property history
- Disclosures
- Permits
- Inspections
- Renovations
- Repairs
- Compliance records
- Supporting evidence
- Verification events

Information shall only be added according to appropriate authorization, provenance, privacy, and legal requirements.

## Success Criteria

HouseLens shall be considered successful when it can help a user:

- Understand the legal context of a property
- Analyze available disclosures
- Identify missing disclosures
- Generate comprehensive questions
- Identify permits that should be investigated
- Identify zoning and compliance questions
- Determine which systems may require professional inspection
- Request appropriate documents
- Track unresolved due diligence
- Understand the evidence supporting recommendations
- Distinguish verified information from unknown information
- Make more informed property decisions

---

# Part of the OpenProperty Ecosystem
[https://roxanneardary.com/openproperty/](https://roxanneardary.com/openproperty/)  

HouseLens is one component of the broader **OpenProperty** transparency network.  

OpenProperty applications include:

* **HouseLens** — buyer and renter protection  
[**TrustLens**](https://codeberg.org/RoxanneA/TrustLens) — seller transparency and preparation.  
[https://roxanneardary.com/trustlens/](https://roxanneardary.com/trustlens/)

Together they create a complete real estate transparency platform.

---

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
  - [https://roxanneardary.com/houselens/](https://roxanneardary.com/houselens/)

---

## License & Notice Requirements

HouseLens is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- HouseLens specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
