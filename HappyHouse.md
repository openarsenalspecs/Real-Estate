# HappyHouse
**Protect, maintain, and enjoy your home.**
- HTML Mirror:  [https://roxanneardary.com/happyhouse-specification/](https://roxanneardary.com/happyhouse-specification/)

---

HappyHouse is a comprehensive, AI-powered home maintenance and property intelligence platform designed to track, manage, and optimize every aspect of a home, from appliances and roofs to solar systems, septic systems, well water systems, and individual replacement parts.

It combines structured data, automated scheduling, and AI insights to give homeowners and professionals complete visibility and control over their property.

---

## Overview

HappyHouse centralizes all property-related data into a single intelligent system:

- Inventory tracking  
- Maintenance scheduling  
- Service history logging  
- Warranty monitoring  
- AI-powered insights  
- Property-wide reporting  
- Part-level tracking and diagnostics  
- Water system and infrastructure tracking  

---

## Core Features

- Centralized home inventory system  
- AI-powered maintenance recommendations  
- Automated service scheduling and reminders  
- Warranty tracking with color-coded alerts  
- Service records with full history and receipts  
- Property-wide reporting and analytics  
- Chronological event timeline  
- Zero-knowledge encryption for privacy  
- Offline-first architecture  

---

## Modules

### Inventory Management
- Track appliances and home systems  
- Store purchase date, price, warranty, and notes  
- Upload invoices for automatic data extraction  
- Color-coded warranty status  

---

### Service Records
- Log all maintenance and repairs  
- Track providers, costs, and parts replaced  
- Attach receipts and documentation  
- Auto-update maintenance schedules  

---

### Warranty Tracker
- Active / expiring / expired status  
- Dashboard alerts for expiring warranties  
- Integrated with all modules  

---

### Part Locator
- Identify compatible replacement parts for any appliance or system  
- Store OEM and aftermarket part numbers  
- AI-assisted part diagnosis based on symptoms  
- Track part replacement history and costs  
- Predict part lifecycle and failure intervals  
- Fully integrated with service records and inventory  

---

### Roof Module
- Full roofing system tracking  
- Material, installer, slope, and structural details  
- Invoice upload with AI auto-fill  
- Repair and inspection history  
- Warranty tracking (material + labor)  
- Auto-calculated inspection schedules  

---

### Solar Module
- Panel, inverter, and battery tracking  
- Installation and system specifications  
- Panel-level monitoring and replacement tracking  
- AI-generated maintenance schedules  
- Warranty tracking and alerts  
- Permit and insurance records  

---

### Septic Module
- Septic system configuration and tracking  
- Pumping and inspection history  
- Auto-calculated service intervals  
- AI maintenance recommendations  
- Cost and repair tracking  

---

### Well Water Module
- Track well systems, pumps, tanks, and filtration  
- Store pump specifications (type, brand, model, horsepower)  
- Pressure tank and system configuration tracking  
- Water quality test logging (pH, iron, sulfur, hardness, bacteria)  
- Pump and component lifecycle tracking  
- AI-powered diagnostics for pressure issues and failures  
- Automatic maintenance scheduling and alerts  
- Full integration with Part Locator and Service Records  

---

### Property Report
Generate a complete professional report including:

1. Property Overview  
2. Full Maintenance History  
3. Roof System Status  
4. Appliance & Systems Inventory  
5. Warranty Summary  
6. Investment Breakdown by Category  
7. Outstanding Issues  
8. Recommendations & Upcoming Actions  
9. Overall Property Condition Assessment  

- Export as a printable PDF  

---

### History Timeline
- Chronological record of all events across all modules  
- Includes purchases, repairs, inspections, services, and upgrades  
- Filterable by event type  
- Fully integrated system-wide  

---

### Pro Workspace
- Cosmetic personalization for licensed professionals  
- Add profile photo, business name, license, and contact details  
- No modification to application logic or UI structure  

---

### API Explorer
- Interactive interface for all endpoints  
- View live JSON responses  
- Test CRUD operations and AI features  

---

## AI Features

- `/ai/prioritize` — Rank maintenance tasks  
- `/ai/predict` — Predict upcoming maintenance needs  
- `/ai/estimate-cost` — Estimate repair and maintenance costs  
- `/ai/tips` — Provide maintenance guidance  
- `/ai/warranty` — Analyze warranty risks  
- `/ai/part-lookup` — Identify compatible parts  
- `/ai/diagnose-part` — Suggest failing components  
- `/ai/predict-septic` — Septic system insights  
- `/ai/well-diagnose` — Diagnose well system issues  
- `/ai/well-predict` — Predict pump and component failure  
- `/ai/well-water-analysis` — Analyze water quality data  
- `/ai/auto-fill` — Extract data from invoices and receipts  

---

## Database Overview

Core tables:

- Categories  
- Tasks  
- TaskSchedule  
- ServiceProviders  
- HomeInventory  
- NotesPhotos  

Extended tables:

- ProfessionalProfiles  
- Roofs  
- SolarSystems  
- SepticSystems  
- SepticServiceRecords  
- WellSystems  
- WellServiceRecords  
- WaterTests  
- Parts  
- PartUsageHistory  

Full schema available in `/database/schema.sql`.  

---

## Security & Privacy

- AES-256-GCM encryption for all stored data  
- PBKDF2-derived master key (password never stored)  
- Zero-knowledge architecture  
- Secure API key storage via OS keychain or encrypted storage  
- Client-side PII scrubbing before AI requests  

⚠️ If the master password is lost, data cannot be recovered.  

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
  - [https://roxanneardary.com/happyhouse/](https://roxanneardary.com/happyhouse/)

---

## License & Notice Requirements

**HappyHouse** is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, network deployments, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- **HappyHouse** specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution **must also update `notice.md`**.
- When submitting a pull request, ensure that any new files maintain the correct attribution headers where applicable.
- All contributions must follow the established repository structure, naming conventions, and documentation formatting used throughout the project.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
