# InspectHome

**InspectHome — Find Homes With Confidence.**

InspectHome is an **open-source, transparency-first real estate platform** that replaces traditional listing systems with a **verification-based property network**. Every listing is required to include full disclosures, supporting documents, and source attribution before it can be published.

Unlike conventional real estate platforms that prioritize advertising and lead generation, InspectHome is built around **truth, documentation, encryption, and accountability**.

---

# Core Vision

InspectHome exists to transform real estate into a **verifiable data system** rather than a marketing-driven listing feed.

The platform ensures:

- Every property has a complete disclosure record  
- Every claim can be verified or flagged  
- Every document is securely stored and encrypted  
- Every listing includes its original source  
- Every user retains full control over their sensitive data  

---

# Full Feature Specification

## 1. Mandatory Property Disclosure System

Every listing must complete a legally structured disclosure form before publication.

### Required disclosure fields include:

- Structural condition  
- Roof age and condition  
- HVAC system status  
- Plumbing and electrical systems  
- Water damage history  
- Flooding history  
- Pest or termite history  
- Known defects or repairs  
- Insurance claims history  
- Renovation history  
- Environmental hazards  

### Enforcement:

- Listings cannot be published without full disclosure completion  
- Disclosure requirements adapt by **state and jurisdiction**  
- Missing or incomplete disclosures block publication  

---

## 2. Document Vault (Encrypted Upload System)

Sellers and landlords can upload verified property documents.

### Supported documents:

- Property deed  
- Title documents  
- Home inspection reports  
- Surveys  
- Renovation receipts  
- Permits and zoning approvals  
- Warranties (roof, HVAC, appliances)  
- Insurance documentation  
- HOA documents  
- Maintenance records  

### Security:

- All documents are **client-side encrypted before upload**  
- The server never has access to raw document data  
- Zero-knowledge architecture ensures host cannot decrypt data  

---

## 3. AI Listing Assistant & Compliance Engine

An AI system guides users through listing creation and ensures compliance.

### AI capabilities:

- State-by-state real estate advertising law compliance  
- Fair housing law detection and enforcement  
- Listing description improvement suggestions  
- Detection of misleading or illegal phrasing  
- Required disclosure prompting  
- Document recommendation system  

### Example enforcement:

- Flags discriminatory language  
- Requires correction before listing publication  
- Prevents unsupported property claims  

---

## 4. Government Data Integration

InspectHome integrates publicly available government and municipal property data to enhance listing accuracy and provide independent verification layers alongside seller-submitted information.

### Integrated Data Sources May Include:

- County property tax records  
- Parcel and cadastral data  
- Zoning and land-use classifications  
- Building permits and inspection filings  
- Code violations and enforcement records  
- Flood zone and environmental hazard maps  
- Property boundary and GIS data  
- Assessor and valuation records (where publicly available)  

### Purpose of Integration:

- Cross-check seller disclosures against official records  
- Improve listing accuracy and reduce misinformation  
- Provide buyers with independent, verifiable context  
- Surface potential risks or inconsistencies in property history  
- Enhance transparency without relying solely on user-submitted data  

### Data Handling Principles:

- Government data is treated as a **read-only verification layer**  
- No modification of official records is permitted within the system  
- Data is displayed alongside listings for contextual analysis only  
- All integrated datasets are attributed to their original public sources where required  

---

## 5. Listing Source Attribution System

Every listing must include its original source.

### Required fields:

- Brokerage name (if applicable)  
- Original listing URL  
- Listing agent (where required by law)  
- Listing origin type (owner, brokerage, builder)  

### Enforcement:

- Listings without valid source attribution cannot be published  
- Source links are permanently displayed on listing pages  

---

## 6. Neighborhood Intelligence System

Provides contextual data about the surrounding area.

### Includes:

- School district quality  
- Crime trends and statistics  
- Flood and environmental risk  
- Insurance cost estimates  
- Property tax trends  
- Zoning and development plans  
- Transportation access  
- Broadband availability  
- Investor ownership density  
- Short-term rental concentration  
- Market appreciation trends  

---

## 7. Property Timeline System

Each property includes a permanent chronological record.

### Timeline events:

- Construction date  
- Ownership transfers  
- Renovations and upgrades  
- Building permits  
- Inspections  
- Repairs and maintenance  
- Insurance claims (when available)  
- Price history  
- Listing history  

The timeline evolves over time, creating a **living property record**.

---

## 8. AI Fraud Detection System

InspectHome uses AI to detect fraudulent or suspicious listings.

### Detection includes:

- Duplicate listings across platforms  
- Stolen or reused images  
- AI-generated or manipulated images  
- Metadata inconsistencies  
- Fake landlord or brokerage identities  
- Suspicious pricing patterns  
- Address mismatches  
- Forged or altered documents  
- Permit inconsistencies  
- Scam pattern recognition  

### Enforcement:

- Flagged listings enter review queue  
- High-risk listings are blocked from publishing  

---

## 9. Ownership Transparency System

Where legally available, InspectHome surfaces ownership structures.

### Includes:

- LLC ownership detection  
- Corporate ownership identification  
- Investment entity tracking  
- Ownership portfolio size (number of properties held)  

This helps reveal institutional ownership patterns in housing markets.

---

## 10. Property Risk Dashboard

Each property includes a risk summary.

### Risk categories:

- Flood risk  
- Insurance risk  
- Structural risk (based on disclosures)  
- Market volatility risk  
- Investor concentration risk  
- Permit compliance risk  

---

## 11. Federated Network Architecture

InspectHome is designed as a **federated system**, not a centralized platform.

### Supported operators:

- Independent brokerages  
- Municipal governments  
- Housing cooperatives  
- Universities  
- Nonprofit organizations  
- Private self-hosted instances  

### Federation features:

- Optional listing sharing between trusted instances  
- Local control over moderation and policies  
- Geographic segmentation per instance  
- Decentralized hosting capability  

---

## 12. End-to-End Encryption System

InspectHome uses zero-knowledge encryption for sensitive data.

### Encrypted data includes:

- User identities  
- Private messages  
- Uploaded documents  
- Disclosure forms  
- Buyer-seller communications  

### Security model:

- Encryption occurs client-side  
- Server stores only ciphertext  
- Host cannot decrypt private data  

---

## 13. Buyer Tools

InspectHome provides buyer-side utilities.

### Features:

- Save and compare listings  
- Document access requests  
- AI-generated property summaries  
- Risk evaluation reports  
- Neighborhood comparison tools  
- Offer tracking workspace  

---

## 14. Seller Tools

Sellers receive structured listing assistance.

### Features:

- Guided listing wizard  
- Disclosure automation  
- Document upload system  
- Compliance validation  
- AI writing assistance  
- Legal prompt warnings  

---

## 15. Open API & Data Access

InspectHome supports open data access for research and transparency.

### Includes:

- Market trends  
- Disclosure statistics  
- Permit activity data  
- Price history datasets  
- Neighborhood analytics  

---

# Technical Stack (Reference Implementation)

Backend:
- Python
- FastAPI
- PostgreSQL + PostGIS
- Redis

Search:
- Elasticsearch or Typesense

Scraping:
- Scrapy
- Playwright

Frontend:
- React / Next.js
- MapLibre
- TailwindCSS

Infrastructure:
- Docker
- Self-hosted deployment support

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
  - [https://roxanneardary.com/inspecthome/](https://roxanneardary.com/inspecthome/)

----

## License & Notice Requirements

InspectHome is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- InspectHome specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Getting Started

Because this platform handles encrypted user data, setup requires:
1. Environment variable configuration  
2. Encryption key generation  
3. Database initialization  
4. Running backend and frontend containers  

Detailed setup instructions can be found in the project’s `docs/Workflow.md`.

---

## Contributing

Contributions are welcome!  
Please read the **CONTRIBUTING.md** file before submitting pull requests.  
All contributions must follow the licensing and attribution requirements.

---
