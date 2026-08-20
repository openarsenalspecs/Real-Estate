# ValueGrid
**The Open Ledger of Property Intelligence**
- HTML Mirror:  [https://roxanneardary.com/valuegrid-specification/](https://roxanneardary.com/valuegrid-specification/)

---

ValueGrid is an open-source property intelligence platform designed to create a transparent, verifiable, and publicly accessible foundation for understanding real estate value.

By combining advanced valuation models, environmental risk analysis, survey intelligence, regulatory datasets, and a National Property Ledger, ValueGrid provides a trusted infrastructure for appraisers, lenders, researchers, developers, and the public.  The goal is to build a system that meets or exceeds the capabilities of proprietary platforms.

ValueGrid is created to support professional appraisal workflows, regulatory compliance, and public transparency across the entire property ecosystem.

---

# Core Principles

### Transparency
All valuation logic, models, and datasets are openly documented.

### Verifiability
Property records include version history and cryptographic verification to detect tampering.

### Professional Utility
The platform is designed to support real-world appraisal workflows and lending processes.

### Public Accessibility
Non-sensitive data can be explored by anyone through a public interface.

### Open Collaboration
Researchers, developers, appraisers, and surveyors can contribute improvements.

---

# Key Features

## Advanced Property Valuation Engine

ValueGrid provides transparent property valuation models that can be inspected, audited, and improved by the community.

Features include:

• comparable sales analysis  
• price trend modeling  
• neighborhood market analysis  
• liquidity scoring  
• valuation confidence scoring  
• valuation explanation reports

---

## National Property Ledger

The National Property Ledger serves as the authoritative historical record for property intelligence.

Each property record contains versioned data including:

• property attributes  
• valuation history  
• survey data  
• environmental risk layers  
• zoning information  
• permit and improvement history

All updates are timestamped and traceable.

---

## Environmental Risk Intelligence

ValueGrid integrates authoritative environmental and geospatial datasets that directly influence property value, insurability, safety, development potential, and long-term risk. Rather than relying solely on traditional valuation inputs, the platform incorporates environmental intelligence into every property record and valuation analysis.

Environmental datasets may include:

- Flood maps and flood zone classifications
- Base Flood Elevation (BFE)
- Historical flood events
- Storm surge risk
- Sea level rise projections
- Wildfire risk
- Radon risk zones
- Wetlands and protected lands
- Coastal erosion zones
- Landslide susceptibility
- Earthquake hazard zones
- Sinkhole susceptibility
- Soil stability and erosion potential
- Drought risk
- Extreme heat exposure
- Air quality trends
- Water quality advisories
- Hazardous waste and contaminated site proximity
- Superfund site proximity
- Brownfield locations
- Dam inundation zones
- Levee protection areas
- Hurricane exposure
- Tornado risk
- Severe weather history
- Lightning frequency
- Snow and ice risk (where applicable)

### Airport Safety & Aviation Intelligence

ValueGrid incorporates aviation-related datasets to help identify risks and development limitations associated with nearby airports.

Layers include:

- Airport locations
- Airport safety zones
- Runway Protection Zones (RPZ)
- Airport Overlay Districts
- Noise contour maps
- Height restriction areas
- Flight approach and departure corridors
- Avigation easements
- Military airspace restrictions (where publicly available)

### Environmental Risk Scoring

Environmental data is combined into a comprehensive property risk profile that can be used alongside valuation models.

Example factors include:

- Flood exposure
- Radon probability
- Wildfire exposure
- Airport noise impact
- Coastal risk
- Storm surge exposure
- Environmental contamination proximity
- Climate resilience

The resulting Environmental Risk Score provides a transparent summary of the property's overall environmental profile while allowing users to review each contributing factor individually.

### National Property Ledger Integration

Environmental intelligence becomes part of each property's permanent record within the National Property Ledger.

Each property record may include:

- Environmental Risk Score
- Flood Zone Classification
- Base Flood Elevation
- Flood Insurance Requirement
- Flood History
- Storm Surge Risk
- Wildfire Risk
- Radon Zone
- Radon Test History (when available)
- Wetlands Indicator
- Protected Land Indicator
- Coastal Erosion Risk
- Sinkhole Risk
- Earthquake Hazard Zone
- Soil Stability Rating
- Airport Safety Zone Status
- Runway Protection Zone Indicator
- Airport Noise Zone
- Height Restriction Zone
- Environmental Dataset Version
- Last Environmental Update Date

### Benefits

Integrating environmental intelligence provides:

- More accurate property valuations
- Better lending and underwriting decisions
- Improved insurance risk analysis
- Greater transparency for buyers and sellers
- Enhanced appraisal support
- Development feasibility insights
- Long-term climate and resilience awareness
- Publicly verifiable environmental property intelligence

---

## Survey Intelligence Engine

ValueGrid can ingest and analyze professional land surveys including:

• boundary surveys  
• ALTA/NSPS land title surveys  
• topographic surveys  
• subdivision plats  
• elevation certificates

The system extracts:

• property boundary geometry  
• easements  
• encroachments  
• building placement  
• elevation information

This allows precise spatial analysis and improved valuation accuracy.

---

## GIS Mapping System

A fully interactive geospatial map allows users to visualize property intelligence layers.

Map layers include:

Property layers  
• parcel boundaries  
• building footprints  
• survey geometry  

Environmental layers  
• flood maps  
• radon zones  
• wildfire risk  

Infrastructure layers  
• transportation corridors  
• utility proximity  
• broadband availability

---

## Regulatory & Zoning Intelligence

ValueGrid integrates zoning and land-use rules to help analyze development potential.

Capabilities include:

• setback compliance analysis  
• buildable area calculation  
• zoning classification mapping  
• land use restrictions

---

## Market Analytics

ValueGrid analyzes housing markets at multiple geographic levels.

Features include:

• price trends  
• supply and demand metrics  
• market liquidity indicators  
• housing affordability indexes

---

## Public Verification Database

A publicly accessible property intelligence database allows users to explore verified information.

Publicly viewable data may include:

• parcel boundaries  
• environmental risks  
• valuation ranges  
• survey status  
• zoning classification  
• market trends

Sensitive information such as personal financial data is excluded.

---

## Cryptographic Record Integrity

Each property record update generates a cryptographic hash fingerprint.

This allows anyone to verify that records have not been altered after publication.

Example record metadata:


Record Version: 12
Last Updated: 2026-03-12
Change: Flood zone update
Source: FEMA
Hash: a84e6d7b91f2b42...


---

# Example Property Record


Property ID: US-FL-025-00012345

Lot Size: 9,850 sq ft
Structure Size: 2,100 sq ft
Year Built: 1994

Estimated Value: $415,000
Confidence Score: 83%

Flood Zone: AE
Radon Risk: Moderate
Airport Noise Zone: Low

Last Survey: 2021
Buildable Area: 7,200 sq ft


---

# Public API

Developers can access property intelligence through open APIs.

Example endpoints:


/property/{id}
/valuation/{id}
/environment/{id}
/survey/{id}
/market/{region}


Example response:


GET /valuation/US-FL-025-00012345

{
estimated_value: 415000,
confidence: 0.83,
valuation_range_low: 398000,
valuation_range_high: 432000
}


---

# Use Cases

ValueGrid supports a wide range of applications.

### Appraisers
Transparent valuation models and professional analysis tools.

### Lenders
Improved risk analysis for mortgage underwriting.

### Researchers
Large-scale property datasets for housing research.

### Developers
Land intelligence for project feasibility analysis.

### Public Users
Clear, accessible information about property conditions and risks.

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
  - [https://roxanneardary.com/valuegrid/](https://roxanneardary.com/valuegrid/)

---

# License & Notice Requirements

ValueGrid is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- ValueGrid specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
