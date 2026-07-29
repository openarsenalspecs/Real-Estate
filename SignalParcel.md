# SignalParcel

**Mapping ownership through verified public records.**

---

## Subtitle

A public records graph for land ownership and operations.

---

## Mission

SignalParcel connects fragmented public records into structured ownership networks for transparency and analysis.

It is designed to unify land ownership, business operations, and licensing data into a single, navigable graph built entirely from verified public sources.

---

## North Star Statement

SignalParcel exists to make land ownership systems readable, verifiable, and structurally transparent using only public records.

---

## What SignalParcel Does Differently

- Connects scattered public records into structured ownership relationships
- Maps land parcels to operating entities and corporate structures
- Links licensing data to real-world property usage
- Builds a navigable graph of ownership, control, and operations
- Enables cross-referencing between land, business entities, and regulatory records

---

## Core Principles

- Only uses publicly available records
- No private or non-public personal data collection
- Full source attribution for every record
- Reproducible data pipelines
- Transparent entity resolution and matching logic
- Open-source and auditable by design

---

## What It Is

- A public records aggregation and normalization system
- A structured ownership graph of land and operators
- A transparency-focused data infrastructure project
- An analytical tool for understanding property and business relationships

---

## What It Is Not

- A surveillance system
- A tool for tracking private individuals
- A behavioral profiling or social monitoring platform
- A system that uses non-public or restricted personal data

---

## Core Concept

- From parcel to structure.
- See the structure behind the land.
- Connecting ownership through public records.
- Structured transparency for land systems.

---

## Data Model Modules

### 1. Parcel Module
Core land unit representation:
- Parcel ID (county/state identifiers)
- Geographic boundaries (GIS support)
- Physical address normalization
- Land classification (recreational, commercial, mixed-use)

---

### 2. Lot / Block / Acreage Module
Handles traditional land subdivision structures and physical scale mapping:

- Lot number identification (subdivision-level tracking)
- Block grouping within plats or developments
- Acreage calculation and normalization
- Cross-referencing between deed descriptions and GIS parcels
- Historical subdivision mapping (changes over time)
- Multi-parcel aggregation (single ownership across multiple lots/blocks)

---

### 3. Ownership Module
- LLC and corporate entity mapping
- Parent → subsidiary relationships
- Ownership structure representation
- Registered agent tracking (official filings only)
- Entity lifecycle history

---

### 4. Operator Module
- Identifies operating business entity
- Detects operator vs land owner mismatch
- Tracks management companies and concessionaires
- Links licensing responsibility to operators

---

### 5. Licensing Module
- Business license verification
- Permit tracking (state and county level)
- Compliance status records
- Expiration and renewal history

---

### 6. Entity Resolution Engine
- Normalizes business names across jurisdictions
- Resolves duplicates and variations
- Matches addresses to parcels and filings
- Confidence scoring for entity linking

---

### 7. Ownership Graph Engine
- Builds relationships between:
  - Parcels
  - Operators
  - LLCs and corporations
  - Parent companies
- Stores data in graph structure for traversal and querying
- Enables visualization of ownership chains

---

### 8. AI Analysis Layer
- Extracts structured data from public documents
- Parses filings and PDFs into entity records
- Identifies inconsistencies in public records
- Summarizes ownership structures for readability

---

## Data Provenance & Audit Trail

Every record includes:

- Source URL or official record ID
- Timestamp of ingestion
- Jurisdiction (county/state/federal)
- Original document reference
- Parsing method (API, scrape, AI extraction)
- Confidence score
- Change history log

All data is traceable to its original public source.

---

## Confidence Scoring System

SignalParcel assigns confidence levels to relationships:

- **High confidence**: Exact identifier match (parcel ID, EIN, registry ID)
- **Medium confidence**: Strong name + address alignment
- **Low confidence**: Fuzzy or incomplete matches

Applied to:
- Ownership links
- Operator mappings
- Parcel associations
- Corporate relationships

---

## Temporal Tracking

SignalParcel maintains historical change data:

- Ownership transfers
- Operator changes
- License issuance and expiration
- Parcel subdivision or consolidation events

This enables:
- Timeline-based analysis
- Historical ownership graphs
- Change detection over time

---

## Geographic Integration (GIS Layer)

- Parcel geometry support
- County plat map integration
- Coordinate normalization (lat/long)
- Boundary overlays
- Multi-parcel ownership clustering

---

## System Architecture

- **Ingestion Layer** – APIs, scrapers, public records feeds  
- **Normalization Layer** – cleaning and standardization  
- **Entity Resolution Engine** – matching and scoring  
- **Graph Database Layer** – relationships and ownership networks  
- **AI Extraction Layer** – document parsing and structuring  
- **API Layer** – public data access  
- **Frontend Layer** – visualization and map interface  

---

## Public API (Conceptual)

- `/parcel/{id}`
- `/entity/{id}`
- `/ownership/{parcel_id}`
- `/graph/{entity_id}`
- `/search?query=`

---

## Data Limitations

- Coverage varies by jurisdiction
- Some counties lack digitized records
- Entity matching is probabilistic, not absolute
- Non-public agreements are not represented

---

## Legal Boundary

- Only publicly available records are used
- No private or restricted datasets are accessed
- No inference of non-public personal data is performed

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
  - [https://roxanneardary.com/signalparcel/](https://roxanneardary.com/signalparcel/)  

---

## License & Notice Requirements

SignalParcel is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- SignalParcel specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
