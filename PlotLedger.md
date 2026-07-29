# PlotLedger
*The Future of Parcel Intelligence*

**PlotLedger** is an open-source AI-powered platform that aggregates, analyzes, and visualizes **large land parcels (9+ acres)** across the United States. It connects **ownership records, sale history, zoning classifications, permits, and special privileges**, providing a comprehensive view for developers, planners, researchers, and enthusiasts.

---

## Features

- **National Parcel Directory**
  Identify all parcels ≥9 acres in every U.S. state and merge contiguous parcels owned by the same entity.

- **Ownership & Sale History**
  Track current and historical owners, past sales, transaction dates, and prices.

- **Zoning & Special Privileges**
  Compare parcels against local zoning laws. Detect special allowances, variances, density bonuses, and conditional use approvals.

- **Permits & Applications**
  Connect each parcel to historical permits and active applications. Flag deviations from standard zoning rules.

- **AI Analysis**
  Automatically parse zoning codes and permit text. Score parcels for development potential and legal deviations. Predict opportunities for future permits and special privileges.

- **Interactive Map Visualization**
  Explore parcels with Mapbox or Leaflet. Color-code by zoning, privilege tier, or development score. Search and filter by state, county, owner, or parcel size.

- **State-by-State Modular Design**
  Each state is a module: easily add, update, or expand. Supports future global expansion.

---

## Installation

To set up PlotLedger locally:

1. Clone the repository:
   git clone https://codeberg.org/RoxanneA/PlotLedger.git
   cd PlotLedger

2. Install Python dependencies:
   pip install -r requirements.txt

3. Initialize the database (PostGIS recommended):
   python initialize_db.py

4. Start the backend server:
   python app.py

5. Open the frontend in your browser (default: http://localhost:3000).

---

## Usage

1. Load parcel data for your state using the GIS ingestion scripts.
2. Merge contiguous parcels and verify ownership data.
3. Run AI analysis to detect zoning deviations, special privileges, and permits.
4. Visualize parcels in the interactive map.
5. Export parcel reports or share datasets with collaborators.

---

## Data Sources

- County GIS portals for parcel boundaries  
- County property appraisers for ownership and sale history  
- Municipal permit and zoning portals  
- Public legal records for special district and variance documentation  

> **Note:** Ensure compliance with local open-data licenses. Personal contact information is not included to protect privacy.

---

## Contributing

PlotLedger is fully open-source under the **GNU Affero General Public License v3.0+ (AGPL-3.0+)**. Contributions are welcome:

- Add new county or state datasets  
- Improve AI algorithms for zoning analysis  
- Enhance frontend map features  
- Add predictive scoring models  

All contributions must include attribution to **Roxanne Ardary** and [roxanneardary.com](https://www.roxanneardary.com/).

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
  - [https://roxanneardary.com/plotledger/](https://roxanneardary.com/plotledger/)

---

## License & Notice Requirements

PlotLedger is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PlotLedger specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
