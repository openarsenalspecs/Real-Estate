# PropIntel  
**Tracking Defaults, Forecasting Trends.**  
A national, open-source, AI-driven property intelligence platform.

PropIntel tracks **every property in the United States**, compiling public records into a unified, transparent system that shows:  
- **Notices of Default**  
- **Foreclosures & Auctions**  
- **Full chain-of-title history**  
- **Ownership transfers**  
- **Liens, mortgages, and assignments**  
- **Institutional ownership patterns**  
- **Predictive market and default analytics**

Organized by **Town → County → State**, PropIntel reveals **who owns what** and how properties move through the financial and legal systems of the United States.

---

# 🏛️ Mission  
To build the first **national, open-source property transparency engine** powered by public records, AI analysis, and community-verified data — accessible to homeowners, journalists, researchers, municipalities, and civic innovators.

---

# 🔍 Core Features

## 1. Property Status & Default Tracking
- Notices of Default (NOD)  
- Pre-foreclosure monitoring  
- Foreclosure filings  
- Trustee notices  
- Postponed / canceled auctions  
- Final auction outcomes  
- Transfer after sale (bank-owned, REO, third-party)  

## 2. Full Chain-of-Title Reconstruction
- Complete ownership history  
- All deed types (warranty, quit claim, sheriff, trustee, etc.)  
- Lien releases & reconveyances  
- Mortgage satisfactions  
- Assignment chains (including MERS)  
- Multi-decade historical transfers  

## 3. Mortgage & Lien Intelligence
- Mortgage originator tracking  
- Servicer changes  
- HELOC detection  
- Lienholder identification  
- Assignment history  
- Priority ranking of encumbrances  

## 4. Tax Delinquency & Tax Lien Tracking
- Annual tax delinquency  
- Tax lien certificates  
- Redemption progress  
- Tax deed transfers  
- Historical delinquency analytics  

## 5. Auction Pipeline Visibility
- New auction announcements  
- Sale postponements  
- Cancellations  
- Investor purchases  
- Bank buy-backs  
- Winning bidder analysis  

## 6. Ownership Clustering & Entity Mapping (AI)
- LLC clustering  
- Portfolio landlord identification  
- Institutional buyer detection  
- Shell entity linking  
- Foreign ownership indicators  
- Mailing-address–based clustering  

## 7. Property Condition & Risk Scores (AI)
- Default probability  
- Vacancy risk  
- Distress indicators  
- Ownership churn  
- Neighborhood stability score  

## 8. Geospatial Parcel Intelligence
- Parcel boundary maps  
- Foreclosure heat maps  
- Ownership concentration layers  
- Tax delinquency overlays  
- Historical transfer visual timelines  

## 9. Public Evidence Vault
A searchable archive of:  
- Deeds  
- Notices of Default  
- Liens  
- Affidavits  
- Trustee notices  
- Auction reports  
- Tax sale documents  

All OCR-processed and indexed.

## 10. AI Document Understanding
- Auto-classification of document type  
- OCR extraction of parcel numbers  
- Legal description parsing  
- Party name extraction  
- Recording date identification  
- Structured data creation  

## 11. Analytics Dashboards
- Foreclosure rates  
- Days-in-default metrics  
- Institutional owner distribution  
- Landlord portfolios  
- Tax delinquency trends  
- Market stress indicators  

## 12. Owner Alerts & Protection
- New lien alerts  
- NOD notifications  
- Mortgage assignment alerts  
- Deed recordings  
- Tax delinquency warnings  
- Auction scheduling alerts  

Safeguards against title fraud and unauthorized encumbrances.

## 13. Government & Civic Tools
- Rental registration validation  
- Landlord identification  
- Absentee owner detection  
- Code enforcement ownership checks  
- Public transparency dashboards  
- Open API for agencies  

## 14. Court & Legal Integration
- Evictions  
- Bankruptcy filings  
- Probate transfers  
- Quiet title actions  
- Partition actions  

## 15. Ownership Family Trees (AI)
- LLC relationships  
- Multi-company ownership networks  
- Registry agent matching  
- Family portfolio structures  

## 16. Predictive Market Stress Index
Real-time AI scoring based on:  
- Economic signals  
- Interest rate exposure  
- Investor pressure  
- Default momentum  
- Neighborhood risk factors  

## 17. Community Verification Layer (Optional)
- Occupancy confirmations  
- Property condition updates  
- Photo submissions  
- Suspected vacancy flags  
- Local knowledge integration  

## 18. Full API Layer
- REST & GraphQL  
- Address search  
- Owner lookup  
- Parcel lookup  
- Document search  
- Regional analytics  

## 19. National Hierarchical Structure
- Town → County → State → National Index  
- Standardized parcel crosswalks  
- Unified property ID system  

---

# 🧠 Tech Stack

## Backend
- Python  
- FastAPI  
- Pydantic v2  
- GraphQL (Ariadne / Strawberry)  
- Celery or Dramatiq for async tasks  

## Database
- PostgreSQL  
- PostGIS  
- pg_partman (partitioning)  
- ElasticSearch / OpenSearch  
- MinIO for document storage  

## Frontend
- React  
- TailwindCSS  
- Mapbox GL JS / Leaflet  
- Recharts / ECharts  
- TanStack Query  

## AI & ML
- PyTorch  
- TensorFlow  
- XGBoost / CatBoost  
- spaCy  
- HuggingFace Transformers  
- OCR: Tesseract, PaddleOCR  

## Ingestion & Processing
- Scrapy  
- Playwright  
- Airflow or Prefect  
- pdfplumber  
- Unstructured.io toolkit  

## Infrastructure
- Docker  
- Kubernetes  
- Traefik / NGINX  
- Prometheus  
- Grafana  
- Loki  
- GitLab CI/CD  

---

# 📂 Repository Structure
```
/data_ingestion
/processing
/ai_models
/api
/frontend
/docs
/schemas
/tests
/infrastructure
```

---

# 🤝 Contributing

Contributions are welcome.  
All contributions remain under **AGPL 3.0+ with required attribution**.

Please read:  
- **notice.md**  
- **license**  
- **contribution guidelines** 

before submitting a pull request.

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
  - [https://roxanneardary.com/propintel/](https://roxanneardary.com/propintel/)

---

## License & Notice Requirements

PropIntel is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- PropIntel specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

# 🌐 Project Status

This is an active, growing open-source initiative.  
Data ingestion, AI pipelines, and doc parsing are being built iteratively.

Community contributions are encouraged.

---

# 🔮 Vision

A future where property records are:  
✔ transparent  
✔ accessible  
✔ verifiable  
✔ searchable  
✔ and protected from manipulation

PropIntel is the foundation for a **new era of real estate clarity**.
