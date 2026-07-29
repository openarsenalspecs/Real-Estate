# ParcelPlanner

**Built on Public Law, Open to the Public.**

ParcelPlanner is an AGPL 3.0+ open-source property intelligence platform that helps users determine what can legally be built, modified, or developed on a parcel of land—and where they should buy property based on their development goals.

It combines zoning intelligence, legal research, development feasibility analysis, rental income modeling, and AI-assisted strategy generation grounded exclusively in official government law and regulatory documents.

---

## Core Features

### Property Intelligence Engine
- Parcel-level analysis of land use potential
- Jurisdiction detection (city, county, state)
- Zoning classification identification
- Overlay and special district detection

### Zoning & Legal Analysis Module
- Reads municipal zoning ordinances
- Interprets county land development codes
- Identifies permitted, conditional, and prohibited uses
- ADU eligibility detection
- Tiny home legality analysis
- Multi-family conversion rules
- Rental restriction analysis (long-term & short-term)

### Buyer Opportunity Discovery Module
- Reverse-search jurisdictions based on user goals
- “Where can I build this?” analysis engine
- ADU-friendly municipality ranking
- Tiny home legality by region comparison
- Duplex and multi-family expansion screening
- Land acquisition recommendation engine

### Development Opportunity Engine
- Identifies viable construction options:
  - Accessory Dwelling Units (ADUs)
  - Garage conversions
  - Detached rental units
  - Tiny homes (where legal)
  - Duplex/triplex conversions
  - Room rental strategies
- Classifies opportunities as:
  - Allowed
  - Conditional
  - Prohibited

### Buildability Analysis
- Setback calculations
- Lot coverage analysis
- Floor area ratio evaluation
- Parking requirement assessment
- Utility access feasibility checks

### Financial & Rental Analysis
- Market rent estimation
- Cash flow modeling
- ROI calculations
- Cap rate estimation
- Payback period analysis
- Investment scenario comparison

### Strategy Engine
- Converts legal + financial data into actionable plans
- Multi-strategy comparisons (ADU vs conversion vs new build)
- Risk and constraint scoring
- Step-by-step development roadmaps

### AI Research Assistant
- Natural language property questions
- Legal explanation of zoning codes
- Regulation interpretation (based on official sources only)
- Strategy recommendations grounded in law

### Government Source Verification System
- Validates official zoning documents
- Tracks ordinance version history
- Ensures only government-issued sources are used
- Detects superseded or outdated regulations
- Maintains audit trail of legal references

---

## Data & Source Policy

ParcelPlanner is strictly grounded in **official public law only**.

### Allowed Sources
- State statutes and administrative codes
- Municipal ordinances and zoning codes
- County land development regulations
- Unified Development Codes (UDC)
- Official zoning maps and GIS systems
- Government planning and permitting documents
- Court rulings and administrative decisions

### Prohibited Sources
- Real estate blogs
- Law firm summaries
- Realtor websites
- News articles
- Forums and social media
- Investor websites
- Third-party zoning summaries

Only government-issued legal documents may be used as authoritative sources.

---

## System Architecture

### Core Modules

- Location Module
- Jurisdiction Discovery Module
- Government Source Verification Module
- Zoning Research Module
- Legal Research Module
- Development Opportunity Module
- Buildability Analysis Module
- Financial Analysis Module
- Strategy Engine Module
- Buyer Opportunity Discovery Module
- AI Research Assistant Module
- Report Generation Module

---

## Output Types

ParcelPlanner generates:

- Property feasibility reports
- Zoning compliance breakdowns
- Development opportunity matrices
- Financial investment models
- Jurisdiction comparison reports
- Buyer opportunity rankings

Export formats:
- Markdown
- JSON
- HTML
- PDF

---

## Example Use Cases

### Property Owner
> “Can I build an ADU on my property in Miami-Dade?”

ParcelPlanner responds with:
- Zoning classification
- ADU legality
- Size restrictions
- Permit requirements
- Official ordinance citations

---

### Property Buyer
> “Where can I buy land where I can build a detached rental unit?”

ParcelPlanner responds with:
- Ranked municipalities
- Legal allowances by jurisdiction
- Minimum lot requirements
- Zoning conditions
- Acquisition guidance

---

### Investor Strategy
> “I want $2,000/month rental income from my property.”

ParcelPlanner generates:
- Feasible development strategies
- Cost estimates
- Rental projections
- ROI analysis
- Legal feasibility confirmation

---

## Technology Stack (Suggested)

- Frontend: Next.js + TypeScript
- Backend: Python (FastAPI)
- Database: PostgreSQL + PostGIS
- GIS Integration: OpenStreetMap + government GIS layers
- AI Layer: LLM + RAG over legal documents
- Document Processing: zoning ordinance parsers

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
  - [https://roxanneardary.com/parcelplanner/](https://roxanneardary.com/parcelplanner/)

---

## License & Notice Requirements

ParcelPlanner is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ParcelPlanner specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
