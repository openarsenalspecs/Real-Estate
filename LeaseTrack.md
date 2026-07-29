# LeaseTrack 
**Rental Trends. Ownership Patterns. Compliance Checks.**

An open source AI platform that analyzes U.S. rental markets to identify affordability gaps, ownership patterns, landlord compliance issues, and market anomalies through AI driven analytics and public data integration.

### Mission

LeaseTrack brings transparency to the U.S. rental housing market by combining rental listings, public records, ownership information, licensing databases, and artificial intelligence into a single open platform. The system helps researchers, policymakers, tenant advocates, investors, journalists, and consumers better understand rental markets through objective data analysis rather than isolated listings.

---

# Core Objectives

* Analyze rental affordability by ZIP Code.
* Compare rents against qualifying income standards.
* Detect unusual rental market activity.
* Monitor ownership concentration.
* Verify landlord licensing compliance.
* Provide explainable AI generated findings.
* Produce interactive visualizations.
* Support community driven improvements.

---

# Feature Modules

## Rental Market Module

### Rental Collection

Collect rental listings from:

* MLS rental listings
* Zillow Rentals
* Apartments.com
* Rent.com
* Realtor rental listings
* Facebook Marketplace
* Craigslist
* Nextdoor
* Additional public rental websites

### Unit Classification

Support:

* Studio
* Efficiency
* One Bedroom
* Two Bedroom
* Three Bedroom
* Four Bedroom
* Five Plus Bedrooms
* Single Family Rentals
* Condominiums
* Townhomes
* Duplexes
* Multifamily Units
* Accessory Dwelling Units

---

## Affordability Module

Compare:

* Average rent
* Median rent
* Median household income
* Standard qualifying income
* Required annual income
* Required monthly income

Calculate:

* Rent to income ratio
* Required qualifying salary
* Local affordability score
* Market affordability index

Identify:

* Underpriced markets
* Overpriced markets
* Affordable housing shortages
* High burden rental markets

---

## AI Analysis Module

Automatically analyze flagged markets.

Evaluate:

* Rapid rent increases
* Historical rent trends
* Rental inventory changes
* Vacancy trends
* Pricing anomalies
* Seasonal patterns
* Neighborhood trends
* Housing shortages

Generate:

* AI summaries
* Market explanations
* Risk assessments
* Affordability reports
* Trend reports

---

## Ownership Intelligence Module

Determine ownership type.

Identify:

* Individual owners
* Corporate owners
* LLC ownership
* Trust ownership
* Institutional investors
* Government ownership
* Nonprofit ownership

Analyze:

* Ownership concentration
* Absentee ownership
* Corporate acquisition patterns
* Portfolio size
* Geographic ownership clusters

---

## Licensing Compliance Module

Review licensing requirements where available.

Verify:

* Rental licenses
* Landlord registrations
* Business licenses
* Inspection requirements
* Registration renewals

Flag:

* Missing licenses
* Expired licenses
* Missing registrations
* Potential compliance issues

---

## Public Records Module

Analyze:

* Property records
* Deeds
* Tax assessments
* Ownership transfers
* Tax liens
* Code violations
* Permit history
* Eviction filings where publicly available
* Foreclosure records
* Parcel information

---

## Market Monitoring Module

Track:

* New rental listings
* Removed listings
* Price reductions
* Price increases
* Time on market
* Listing history
* Rental inventory
* Market velocity

---

## Broker Analytics Module

Review MLS activity.

Analyze:

* Listing broker activity
* Listing agent activity
* Repeated market participation
* Rental concentration
* Geographic specialization

---

## Geographic Analysis Module

Support:

* National analysis
* State analysis
* County analysis
* Municipality analysis
* ZIP Code analysis
* Neighborhood analysis
* Census tract analysis

Interactive mapping includes:

* Heat maps
* Ownership maps
* Affordability maps
* Compliance maps
* Market activity maps

---

## Historical Analytics Module

Maintain historical datasets for:

* Rent history
* Ownership changes
* Licensing history
* Inventory history
* Market trend history
* Affordability history

Generate:

* Trend comparisons
* Historical reports
* Growth analysis

---

## Reporting Module

Generate:

* ZIP Code reports
* City reports
* County reports
* State reports
* Ownership reports
* Compliance reports
* AI summaries
* Affordability reports
* Market trend reports

Export:

* PDF
* CSV
* JSON
* Excel

---

## Notification Module

Notify users of:

* New affordability issues
* Large rent increases
* Ownership changes
* Licensing issues
* New market anomalies
* Significant market trends

Support:

* Scheduled reports
* Weekly updates
* Monthly summaries
* Custom alerts

---

## Dashboard Module

Interactive dashboard includes:

* Market overview
* Rental trends
* Affordability charts
* Ownership charts
* Compliance status
* Heat maps
* Historical graphs
* AI generated insights

---

## Community Module

Support:

* Community contributions
* Public issue reporting
* Data validation
* Research collaboration
* Documentation improvements

---

## API Module

Provide APIs for:

* Rental statistics
* Affordability calculations
* Ownership lookups
* Licensing verification
* Market reports
* Historical trends
* AI summaries

---

# Artificial Intelligence Features

The AI system can:

* Explain affordability gaps
* Detect market anomalies
* Identify ownership trends
* Analyze rental behavior
* Produce plain language reports
* Forecast rental trends
* Recommend additional investigation
* Compare neighboring markets
* Detect unusual ownership concentration
* Identify emerging housing issues

---

# Technology Stack

## Backend

* Python
* FastAPI
* Celery
* Redis

## Database

* PostgreSQL
* PostGIS

## Data Processing

* Pandas
* NumPy
* Scikit Learn
* TensorFlow

## Artificial Intelligence

* Large Language Models
* LangChain
* Vector Database support
* Retrieval Augmented Generation
* Explainable AI

## Frontend

* React
* Tailwind CSS

## Mapping

* Leaflet
* Mapbox

## Visualization

* Plotly
* D3.js

## Web Collection

* BeautifulSoup
* Playwright
* Selenium

---

# Design Principles

* Modular architecture
* Open source
* Explainable AI
* Transparent calculations
* Privacy conscious
* Public data first
* Extensible plugin architecture
* API first design
* Local deployment support
* Scalable infrastructure

---

# Intended Users

* Researchers
* Housing advocates
* Journalists
* Investors
* Property managers
* Government agencies
* Universities
* Nonprofit organizations
* Community planners
* Consumers

---

# Future Modules

* Fair Housing Analysis
* Rent Control Analytics
* Housing Supply Modeling
* Gentrification Indicators
* Economic Mobility Analysis
* Rental Fraud Detection
* Corporate Portfolio Intelligence
* Tenant Displacement Indicators
* Housing Policy Simulation
* Infrastructure Impact Analysis
* School District Correlation
* Transit Accessibility Analysis
* Environmental Risk Mapping
* Disaster Recovery Monitoring
* Predictive Market Forecasting

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
  - [https://roxanneardary.com/leasetrack/](https://roxanneardary.com/leasetrack/)

---

## License & Notice Requirements

LeaseTrack is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- LeaseTrack specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Contact

For contributions, questions, or inquiries:  
**Roxanne Ardary**  
Website: [https://www.roxanneardary.com/](https://www.roxanneardary.com/)
