# RecordMesh

**Record systems don’t connect—until RecordMesh.**

RecordMesh is an open source modular AI platform for jurisdiction-aware property document generation, life estate structuring, deed drafting, legal risk analysis, county recording packet generation, and real estate filing workflow automation.

The platform is designed to bridge fragmented state and county recording systems by transforming structured legal intent into filing-ready real property instruments and recording packets.

RecordMesh is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.

---

# Overview

RecordMesh provides a modular framework for generating and validating real property instruments based on the laws of the state where the property is located while preparing county-specific recording packets for filing workflows.

The platform separates:

- Legal intent
- Jurisdictional law logic
- Instrument generation
- Risk validation
- County recording requirements
- Filing packet assembly

This modular architecture allows RecordMesh to scale across jurisdictions without tightly coupling legal logic to formatting systems.

---

# Core Features

## Jurisdiction-Aware Life Estate Generation

Generate life estate structures based on state-specific real property rules and enforceability considerations.

Supported concepts include:

- Traditional life estates
- Reserved life estates
- Remainder interests
- Reversionary interests
- Conditional termination clauses
- Occupancy conditions
- Abandonment-trigger modeling
- Property return conditions
- Beneficiary structures
- Multi-party ownership configurations

---

## State Law Engine

A modular plugin-based legal rules engine for state-specific property law interpretation and drafting guidance.

Features include:

- State-specific deed requirements
- Real property law modeling
- Jurisdictional validation logic
- Enforceability analysis
- Legal conflict detection
- Homestead consideration analysis
- Transfer restriction detection
- Recording compliance checks
- Risk scoring
- Rule versioning
- Legal source references
- Expandable state plugin architecture

---

## Legal Risk & Validation Engine

Analyze generated instruments against jurisdictional constraints and enforceability concerns.

Validation features include:

- Clause conflict analysis
- State law compatibility checks
- Recording rejection risk analysis
- Judicial enforcement warnings
- Abandonment clause risk modeling
- Automatic forfeiture clause analysis
- Signature requirement validation
- Missing legal element detection
- Structural integrity checks
- Filing readiness validation

---

## County Recording Packet Generation

Generate county-specific filing packets designed around local recording office requirements.

Packet generation features include:

- County cover sheet generation
- Recording margin formatting
- Parcel identifier integration
- Grantor/grantee indexing preparation
- Return address formatting
- Filing instruction generation
- Recording fee estimation support
- Metadata packaging
- Multi-document packet assembly
- County formatting profiles
- State-to-county formatting translation

---

## County Profile Engine

A modular county requirement system that stores formatting and filing requirements independently from legal logic.

Features include:

- County-specific formatting rules
- Margin requirement profiles
- Font requirement profiles
- Recording metadata requirements
- Parcel indexing requirements
- E-recording compatibility profiles
- Transfer form mapping
- Cover page requirements
- Filing instruction templates
- County plugin expansion support

---

## Instrument Builder

Structured document generation for real property instruments.

Supported document types include:

- Life estate deeds
- Warranty deeds
- Quitclaim deeds
- Transfer instruments
- Conditional conveyance structures
- Remainder transfer structures
- Reservation clauses
- Reversion clauses
- Supplemental affidavit generation
- Recording declarations

---

## Document Rendering System

Render generated instruments into multiple formats.

Supported outputs:

- PDF
- DOCX
- Markdown archival format
- JSON structured legal objects

Rendering features:

- Recording-compliant margins
- Signature block generation
- Notary acknowledgment generation
- Structured section formatting
- Metadata embedding
- Version tracking

---

## Submission Adapter Layer

Optional submission pipeline support for recording workflows.

Features include:

- Manual filing packet generation
- E-recording preparation
- Submission metadata packaging
- Filing manifest generation
- Exportable submission bundles
- Vendor adapter support
- Recording endpoint abstraction

---

## Modular Plugin Architecture

RecordMesh is designed as a composable legal infrastructure system.

Modular layers include:

- Intent parsing
- State law engines
- Validation systems
- County profile modules
- Rendering systems
- Filing adapters
- Document templates
- Risk analysis engines

This architecture allows developers to extend the platform without modifying the core system.

---

## Structured Legal Intent Parsing

Convert natural language requests into structured legal data models.

Examples include:

- Property transfer requests
- Life estate reservation requests
- Conditional ownership requests
- Beneficiary instructions
- Recording workflow requests
- Filing packet requests

---

## Audit & Traceability

Track how generated instruments were created.

Features include:

- Rule version tracking
- Source reference tracking
- Generation timestamps
- Validation history
- Jurisdiction tracking
- Rendering logs
- Packet assembly metadata

---

# Technology Stack

## Backend
- Python
- FastAPI
- PostgreSQL
- JSONB
- Optional Neo4j support

## AI & Legal Modeling
- Open source LLM integration
- Retrieval-Augmented Generation (RAG)
- Legal rule engines
- Structured validation pipelines

## Frontend
- React
- TypeScript

## Infrastructure
- Docker
- GitLab CI/CD

---

# Design Principles

## Separation of Law and Formatting

State law logic is isolated from county recording formatting logic.

- State modules determine legality.
- County modules determine formatting and filing requirements.

---

## Modular by Default

Every layer is replaceable and independently versioned.

---

## Jurisdiction Awareness

All document generation is jurisdiction-aware and tied to state-specific rule systems.

---

## Recording-Centric Architecture

The platform is designed around real-world public recording workflows rather than generic document generation.

---

## Open Infrastructure

RecordMesh is designed as open legal infrastructure under AGPL-3.0+.

---

# Planned Features

- Nationwide county profile expansion
- Trust structure generation
- Probate workflow integration
- Medicaid planning overlays
- Property transfer simulations
- API integrations for parcel data
- GIS integration
- Electronic recording vendor adapters
- Real-time filing validation
- Blockchain-backed document verification
- Multi-language support
- Enterprise orchestration APIs

---

# Important Legal Notice

RecordMesh generates informational legal drafting assistance and recording workflow preparation tools.

Generated instruments, filings, validations, and recommendations are not a substitute for licensed legal counsel, title review, or jurisdiction-specific attorney advice.

Users are responsible for ensuring compliance with applicable laws, filing requirements, and recording office procedures.

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
  - [https://roxanneardary.com/recordmesh/](https://roxanneardary.com/recordmesh/)  

---

## License & Notice Requirements

RecordMesh is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- RecordMesh specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

# Attribution

Created by **Roxanne Ardary**  
**[roxanneardary.com](https://www.roxanneardary.com/)**

--- 
