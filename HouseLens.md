# HouseLens

### From Unknowns to Insights

**HouseLens** is an open-source property intelligence platform designed to protect **home buyers and renters** by bringing transparency, verification, and AI-assisted analysis to real estate transactions.

HouseLens helps users uncover risks, verify disclosures, confirm permits, and identify critical questions before committing to a property purchase or rental agreement.

It is part of the **OpenProperty** ecosystem. https://codeberg.org/RoxanneA/OpenProperty

---

# Mission

Buying or renting a home is often the largest financial commitment a person makes, yet property information can be incomplete, unclear, or difficult to verify.

HouseLens exists to:

* help buyers and renters uncover hidden property risks
* analyze property disclosure documents
* verify permits, zoning, and legal compliance
* recommend inspections by licensed professionals
* guide users through the due diligence process
* ensure transparency in every property decision

HouseLens transforms property evaluation from guesswork into **data-driven insight**.

---

# Key Features

## AI Disclosure Analysis

Users can upload property disclosures and related documents.

HouseLens analyzes:

* seller disclosures
* rental disclosures
* inspection reports
* permit documentation
* renovation records

The AI highlights:

* missing information
* inconsistencies
* potential risks
* questions that should be asked

---

## Missing Disclosure Detection

If a property disclosure was **not provided**, HouseLens automatically generates a comprehensive list of questions based on:

* state property disclosure laws
* common defect categories
* typical buyer protections

This ensures that buyers and renters **never miss critical questions**.

---

## State-Law-Aware Property Evaluation

HouseLens determines where the property is located and prioritizes:

* state disclosure laws
* county regulations
* township permit requirements
* zoning restrictions
* rental compliance rules

All recommendations are generated based on the **legal framework of the property location**.

---

## Permit and Renovation Verification

HouseLens evaluates property upgrades such as:

* sunrooms
* finished basements
* electrical upgrades
* plumbing renovations
* structural modifications
* additions or expansions

The system identifies:

* permits that should exist
* inspections that should have occurred
* potential compliance issues

---

## Inspection Recommendations

HouseLens recommends inspections by licensed professionals when appropriate, including:

* structural engineers
* electricians
* plumbers
* HVAC specialists
* roof inspectors
* pest inspectors
* environmental specialists

These recommendations help verify disclosure accuracy.

---

## Property Transparency Report

HouseLens generates a comprehensive **Property Transparency Report** including:

* disclosure completeness
* permit verification
* inspection recommendations
* zoning and compliance risks
* AI-identified concerns

This report helps buyers and renters make informed decisions.

---

# Buyer Due Diligence Assistant

HouseLens guides users step-by-step through the property evaluation process.

The system generates questions for:

* sellers
* landlords
* real estate agents
* township offices
* county building departments
* homeowners associations

This ensures that **no stone is left unturned** during property research.

---

# Document Analysis

Users can upload documents such as:

* seller disclosure forms
* inspection reports
* permits
* HOA documents
* lease agreements

HouseLens uses AI and OCR to extract and evaluate relevant information.

---

# Technology Stack

## Backend

* Python
* FastAPI

## Frontend

* React
* Next.js
* TailwindCSS

## Database

* PostgreSQL

## AI Layer

Supports:

* local large language models
* optional external AI APIs

Used for:

* document analysis
* disclosure evaluation
* risk detection
* question generation
* compliance guidance

---

## Document Processing

* OCR document scanning
* structured data extraction
* automated document classification

---

## Security

HouseLens prioritizes data security with:

* encrypted document storage
* secure authentication
* encrypted communication
* user-controlled document access

---

# Open Source Collaboration

HouseLens benefits from contributions from:

* developers
* legal researchers
* real estate professionals
* inspectors
* open data advocates

Areas for contribution include:

* state disclosure law modules
* inspection recommendation rules
* permit database integrations
* fraud detection improvements
* UI improvements
* documentation

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
- HouseLens specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

# Part of the OpenProperty Ecosystem

HouseLens is one component of the broader **OpenProperty** transparency network.

OpenProperty applications include:

* **HouseLens** — buyer and renter protection
* **TrustLens** — seller transparency and preparation.  [https://codeberg.org/RoxanneA/TrustLens](https://codeberg.org/RoxanneA/TrustLens)

Together they create a complete real estate transparency platform.

---

# Vision

HouseLens aims to become the most trusted open-source property intelligence tool available.

By combining AI analysis, legal awareness, and public records verification, HouseLens empowers buyers and renters to move **from unknowns to insights** before committing to a home.
