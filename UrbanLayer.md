# UrbanLayer
**City regulations, instantly understood.**
- HTML Mirror:  [https://roxanneardary.com/urbanlayer-specification/](https://roxanneardary.com/urbanlayer-specification/)

---

## Specification

UrbanLayer is an open-source municipal infrastructure specification for converting zoning laws, permitting requirements, planning regulations, and municipal spatial data into structured, machine-readable systems.

UrbanLayer is designed as a municipality-centric platform. Each municipality can maintain its own regulatory rules, permit types, workflows, geographic data, and administrative requirements while using a shared core architecture.

The specification is modular and extensible. Core modules define the foundational capabilities required by the platform. Optional plugin modules provide additional capabilities that municipalities may enable according to their needs.

## Design Principles

UrbanLayer shall follow these principles:

- Municipality-centric architecture
- Open-source infrastructure
- Modular design
- Local regulatory control
- Human oversight
- Explainable automation
- Regulatory source traceability
- Geographic accuracy
- Version-controlled rules
- Interoperable data
- Vendor neutrality
- Local-first deployment capability
- Transparent compliance analysis
- Configurable municipal workflows

---

## Core Modules

### Municipality Module

The Municipality Module defines the primary jurisdictional configuration for each deployment.

Capabilities include:

- Municipality identification
- State and county relationships
- Municipal boundaries
- Department configuration
- Administrative contacts
- Municipal policies
- Local regulatory authorities
- Municipal-specific configuration
- Local rule overrides
- Municipal data ownership
- Municipal configuration versioning

The municipality shall remain the primary configuration boundary for local zoning and permitting rules.

### Regulatory Rules Module

The Regulatory Rules Module manages municipal regulations as structured digital rules.

Capabilities include:

- Zoning regulations
- Land-use regulations
- Building requirements
- Setback requirements
- Height restrictions
- Lot coverage requirements
- Density requirements
- Parking requirements
- Permitted uses
- Conditional uses
- Accessory structure requirements
- Variance requirements
- Environmental restrictions
- Historic preservation requirements
- Effective dates
- Regulatory versions
- Rule dependencies
- Rule provenance
- Source references

### Universal Zoning Rule Language Module

The Universal Zoning Rule Language, or UZRL, provides a standardized machine-readable representation for zoning regulations.

UZRL shall support:

- Zoning districts
- Dimensional requirements
- Conditional requirements
- Permitted uses
- Prohibited uses
- Exceptions
- Conditional uses
- Variances
- Special conditions
- Geographic conditions
- Rule dependencies
- Effective dates
- Rule versioning
- Regulatory references

UZRL shall support both machine processing and human-readable representations.

### Regulatory Source Module

The Regulatory Source Module maintains the relationship between structured rules and their authoritative source material.

Capabilities include:

- Source document registration
- Ordinance identification
- Section references
- Page references
- Regulatory citations
- Source URLs
- Publication dates
- Effective dates
- Amendment references
- Source version tracking
- Rule-to-source relationships

Every machine-readable regulatory rule should be traceable to its originating source whenever authoritative source information is available.

### Permit Module

The Permit Module provides configurable municipal permitting capabilities.

Capabilities include:

- Permit types
- Permit applications
- Application requirements
- Required documents
- Application status
- Permit fees
- Review requirements
- Approval requirements
- Correction requests
- Resubmissions
- Permit history
- Permit records
- Municipal-specific permit definitions

Municipalities shall be able to create, modify, and deactivate permit types according to local requirements.

### Permit Compliance Module

The Permit Compliance Module evaluates applications against applicable municipal rules.

Capabilities include:

- Zoning compliance checks
- Dimensional checks
- Setback verification
- Building height verification
- Lot coverage verification
- Density verification
- Parking verification
- Use verification
- Geographic restrictions
- Environmental restrictions
- Historic restrictions
- Conditional requirements
- Violation detection
- Compliance reports
- Conditional approval results
- Human review escalation

Compliance results shall provide understandable explanations of the rules applied.

### GIS Module

The GIS Module provides geographic and spatial analysis capabilities.

Capabilities include:

- Parcel boundaries
- Zoning districts
- Municipal boundaries
- Flood zones
- Wetlands
- Environmental protection areas
- Conservation areas
- Infrastructure networks
- Utility systems
- Roads
- Historic districts
- Preservation areas
- Elevation
- Terrain
- Slope
- Spatial intersections
- Buffer analysis
- Geographic proximity analysis

The GIS Module shall support common interoperable geographic data formats and services.

### Municipal Data Layer Module

The Municipal Data Layer Module manages spatial datasets used by municipal compliance processes.

Core supported layers include:

- Parcel boundaries
- Zoning districts
- Flood hazard zones
- Wetlands and environmental protections
- Infrastructure networks
- Historic preservation districts
- Elevation and terrain

Municipalities may add additional layers according to local regulatory requirements.

### Rule Engine Module

The Rule Engine Module executes machine-readable regulatory rules.

Capabilities include:

- Rule evaluation
- Conditional logic
- Rule dependencies
- Geographic conditions
- Dimensional calculations
- Threshold calculations
- Exceptions
- Overrides
- Effective-date evaluation
- Rule version selection
- Compliance determination
- Explanation generation

The Rule Engine shall remain deterministic where official regulatory rules can be represented deterministically.

### Workflow Module

The Workflow Module manages municipal review processes.

Capabilities include:

- Application routing
- Automated checks
- Department review
- Planner review
- Zoning review
- Building review
- Environmental review
- Board review
- Variance review
- Conditional approval
- Escalation
- Reassignment
- Notifications
- Approval
- Denial
- Correction requests
- Workflow history

Municipalities shall be able to configure workflows without modifying the core platform.

### Document Module

The Document Module manages regulatory and permit documents.

Capabilities include:

- Document uploads
- Document classification
- Document indexing
- Document versioning
- Document metadata
- Source tracking
- Permit attachments
- Regulatory documents
- Application records
- Document search

### AI Regulation Parser Module

The AI Regulation Parser Module assists municipalities in converting existing regulatory documents into structured rules.

Capabilities include:

- PDF analysis
- Regulatory text extraction
- Section identification
- Rule identification
- Cross-reference identification
- UZRL generation
- Source citation mapping
- Ambiguity detection
- Conflicting rule detection
- Rule confidence assessment

AI-generated rules shall require appropriate human validation before becoming authoritative municipal rules.

### AI Document Analysis Module

The AI Document Analysis Module assists with the interpretation of submitted permit materials.

Capabilities include:

- Site plan analysis
- Architectural document analysis
- Document classification
- Measurement extraction
- Structure identification
- Property feature identification
- Rule matching
- Potential violation detection
- Review recommendations

AI analysis shall remain advisory unless a municipality explicitly authorizes an automated determination for a particular process.

### Property Simulation Module

The Property Simulation Module allows users to evaluate proposed development scenarios before submitting formal applications.

Capabilities include:

- Parcel selection
- Interactive mapping
- Proposed structure placement
- Structure dimensions
- Setback simulation
- Height simulation
- Lot coverage simulation
- Zoning use simulation
- Permit requirement estimation
- Compliance testing
- Violation explanations
- Scenario comparison

Simulation results shall clearly distinguish preliminary guidance from official municipal determinations.

### Public Portal Module

The Public Portal Module provides public-facing access to municipal information and services.

Capabilities include:

- Property lookup
- Zoning lookup
- Permit requirement lookup
- Permit applications
- Permit status
- Document submission
- Compliance guidance
- Property simulation
- Regulatory search
- Public regulatory information

Municipalities shall control which information and services are publicly accessible.

### Municipal Administration Module

The Municipal Administration Module provides administrative controls.

Capabilities include:

- User management
- Department management
- Role management
- Permissions
- Review assignments
- Application queues
- Municipal settings
- Rule management
- Workflow management
- Data management
- Audit access

### Audit and Provenance Module

The Audit and Provenance Module records important system and regulatory events.

Capabilities include:

- Rule changes
- Rule approvals
- Application changes
- Workflow events
- Administrative actions
- AI-generated content
- Human approvals
- Data imports
- Data updates
- Source changes
- Configuration changes

Audit records shall support accountability and regulatory traceability.

### Regulatory Versioning Module

The Regulatory Versioning Module manages changes to municipal regulations over time.

Capabilities include:

- Rule versions
- Effective dates
- Historical rules
- Future rules
- Amendments
- Repealed rules
- Rule comparisons
- Change histories
- Version selection
- Historical compliance evaluation

The system shall be capable of determining which rule version applies to a transaction based on applicable dates.

### Data Validation Module

The Data Validation Module evaluates the quality and integrity of municipal datasets.

Capabilities include:

- Missing data detection
- Duplicate detection
- Invalid geometry detection
- Projection validation
- Layer completeness checks
- Conflicting zoning detection
- Outdated dataset detection
- Data source validation
- Data quality reporting

### Deployment Module

The Deployment Module provides guided municipal installation and configuration.

Capabilities include:

- Municipality setup
- Jurisdiction configuration
- GIS data import
- Regulatory document import
- AI-assisted rule generation
- Permit configuration
- Workflow configuration
- User configuration
- Public portal configuration
- Deployment validation
- System health checks

The deployment process shall be designed to minimize technical requirements for municipalities.

### Integration Module

The Integration Module provides interoperability with external systems.

Capabilities include:

- REST APIs
- Geographic data services
- Municipal databases
- Document systems
- Property systems
- Permit systems
- Identity systems
- Mapping systems
- External regulatory data
- Data import and export

The integration architecture shall avoid unnecessary vendor lock-in.

### Security Module

The Security Module provides platform security controls.

Capabilities include:

- Authentication
- Authorization
- Role-based access
- Permission management
- Secure document access
- Audit logging
- Administrative controls
- Data access controls
- Configuration protection

Municipal deployments shall be capable of applying security requirements appropriate to their jurisdiction and use case.

## Optional Plugin Modules

Optional plugins extend UrbanLayer without modifying the core architecture.

### Environmental Review Plugin

Provides additional environmental analysis.

Capabilities may include:

- Wetland analysis
- Habitat analysis
- Conservation analysis
- Environmental buffers
- Protected-area analysis
- Environmental permit guidance

### Flood Analysis Plugin

Provides advanced flood-related analysis.

Capabilities may include:

- Flood zone analysis
- Elevation analysis
- Floodplain checks
- Required documentation identification
- Flood-related compliance guidance

### Historic Preservation Plugin

Provides historic preservation analysis.

Capabilities may include:

- Historic district identification
- Landmark identification
- Preservation requirements
- Design review requirements
- Historic permit workflows

### Infrastructure Planning Plugin

Provides infrastructure-related planning analysis.

Capabilities may include:

- Utility proximity
- Road access
- Sewer availability
- Water availability
- Stormwater infrastructure
- Infrastructure capacity analysis

### Advanced Planning Plugin

Provides advanced planning and development analysis.

Capabilities may include:

- Development scenarios
- Density analysis
- Land-use analysis
- Development constraints
- Planning simulations
- Infrastructure impact analysis

### Regulatory Comparison Plugin

Provides cross-jurisdiction regulatory analysis.

Capabilities may include:

- Municipality comparisons
- Zoning comparison
- Permit comparison
- Regulatory differences
- Rule similarity analysis
- Regulatory benchmarking

### Regulatory Conflict Plugin

Detects potential conflicts within municipal regulations.

Capabilities may include:

- Contradictory rules
- Duplicate requirements
- Cross-reference conflicts
- Conflicting definitions
- Outdated references
- Regulatory dependency problems

### Regulatory Change Monitoring Plugin

Monitors regulatory sources for changes.

Capabilities may include:

- Source monitoring
- Ordinance change detection
- Amendment detection
- Rule change alerts
- Source version comparison
- Municipal review queues

### Advanced AI Planning Plugin

Provides optional AI-assisted planning capabilities.

Capabilities may include:

- Development scenario generation
- Planning analysis
- Land-use recommendations
- Infrastructure scenario modeling
- Planning document analysis
- Policy impact analysis

AI recommendations shall remain subject to municipal review and applicable law.

### Building Plan Analysis Plugin

Provides advanced analysis of architectural and engineering plans.

Capabilities may include:

- Plan interpretation
- Dimension extraction
- Building footprint analysis
- Floor-area analysis
- Setback measurement
- Structure identification
- Compliance pre-checking

### Three-Dimensional Property Plugin

Provides optional three-dimensional visualization.

Capabilities may include:

- 3D property models
- Proposed structure visualization
- Height visualization
- Terrain visualization
- Development scenarios
- Spatial conflict visualization

### Open Municipal Rule Library Plugin

Provides collaborative sharing of municipal rules.

Capabilities may include:

- Rule publishing
- Rule discovery
- Rule templates
- Municipal contributions
- Rule validation
- Rule versioning
- Source attribution
- Community review

## Human Oversight

UrbanLayer shall distinguish between:

- Official municipal determinations
- Automated compliance checks
- AI-generated interpretations
- Preliminary citizen guidance
- Simulation results

AI-generated regulatory interpretations shall not automatically become authoritative without an appropriate municipal approval process.

Municipal staff shall retain control over official regulatory decisions.

## Regulatory Transparency

UrbanLayer shall provide mechanisms for users to understand how a compliance result was generated.

Where applicable, results should identify:

- Applicable municipality
- Applicable zoning district
- Rules evaluated
- Regulatory source
- Rule version
- Effective date
- Relevant geographic layers
- Compliance result
- Violations
- Conditions
- Human review requirements

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
  - [https://roxanneardary.com/urbanlayer/](https://roxanneardary.com/urbanlayer/)

---

# License & Notice Requirements

UrbanLayer is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- UrbanLayer specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
