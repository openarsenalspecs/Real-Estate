# HabitaSense  
Built on Data. Grounded in Reality.

HabitaSense is an open-source, AGPL-3.0+ licensed housing market intelligence platform designed to bring transparency, fairness, and accountability to rental and home ownership pricing. Using AI-driven analysis, HabitaSense evaluates listings, detects inflated pricing, identifies appraisal irregularities, and provides true market-value insights based on real data.

## Features

### AI Listing Intelligence
- Automated parsing of rental and sale listings  
- Extraction of structured features (beds, baths, square footage, amenities)  
- Natural language processing for listing descriptions  
- Detection of missing or inconsistent listing details  

### Price Fairness Analysis
- Real-time price comparison against local market comps  
- Historical sales and rental benchmarking  
- Regional normalization by neighborhood, ZIP code, and city  
- Amenity-weighted valuation adjustments  
- Cost-per-square-foot and adjusted-value scoring  

### Fraud and Inflation Detection
- Inflated pricing detection based on statistical deviation  
- Suspicious pattern recognition (rapid relisting, artificial price swings)  
- Appraisal history anomaly detection  
- Identification of listing-to-record inconsistencies  
- Fraud likelihood scoring  

### Market Movement Tracking
- Significant price drop alerts  
- Full listing history tracking across time  
- Market volatility indicators  
- Trend-shift alerts based on local patterns  

### Rental vs Ownership Modeling
- Long-term rent vs buy cost analysis  
- Mortgage break-even projections  
- Interest rate sensitivity modeling  
- Total cost of occupancy estimation  

### Geospatial Intelligence
- Neighborhood price heatmaps  
- Spatial analysis powered by PostGIS  
- Proximity-based value adjustments (schools, transit, amenities)  
- Regional affordability scoring  

### Trust and Transparency Layer
- Listing trust score (0–100)  
- Explainable AI outputs for all flags  
- Feature-level value justification  
- Open scoring methodology for public review  

### Data Integration Layer
- Ingestion of MLS, county, tax assessor, and zoning data  
- Multi-source data normalization  
- Public record mapping  
- Robust import and reconciliation pipeline  

### Alerts and Monitoring
- Overpriced listing alerts  
- Underpriced opportunity detection  
- Rapid market change notifications  
- Irregular valuation warnings  

### Financial Oversight Integrations
- Loan risk prediction  
- Fair appraisal value estimation  
- Detection of appraisal irregularities and suspicious valuation spikes  
- Predatory lending pattern recognition  
- HOA financial health scoring  
- Property tax anomaly detection  
- Mortgage stress testing under rate fluctuations  
- Equity-growth projections  
- Corporate ownership detection  
- Foreclosure risk indicators  
- Over-leveraged property identification  

### AI and Model Layer
- Regression-based price prediction models  
- Anomaly detection for outlier identification  
- LLM-assisted feature extraction  
- Explainability tools for transparency  
- Continuous model retraining  
- Bias-correction mechanisms  

### Platform Features
- RESTful API architecture  
- Real-time processing pipeline  
- PostgreSQL + PostGIS database  
- React / Next.js frontend  
- Map-based visualization system  
- Data export tools  

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
  - [https://roxanneardary.com/habitasense/](https://roxanneardary.com/habitasense/)

---

## License & Notice Requirements

HabitaSense is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- HabitaSense specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---
