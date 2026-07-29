# CasaBot

CasaBot is an open-source AI-powered real estate companion that continuously monitors property listings and delivers personalized alerts, market insights, and intelligent answers about your target housing market.

**Your AI Companion in Real Estate**

---

## Overview

CasaBot allows users to define precise home-buying criteria and automatically tracks listings across supported data sources. It analyzes new properties, market trends, pricing changes, and inventory levels to help users make informed real estate decisions without manual searching.

---

## Core Features

### Smart Property Matching
- Define exact search criteria:
  - Location (ZIP, city, neighborhood)
  - Price range
  - Bedrooms / bathrooms
  - Property type (house, condo, townhouse, etc.)
  - Lot size, square footage, year built
  - Custom filters (HOA, garage, waterfront, etc.)
- Automatically matches incoming listings to saved profiles

### Real-Time Listing Monitoring
- Continuously scans supported listing sources
- Detects:
  - New listings
  - Price reductions
  - Status changes (active → pending → sold)
- Prevents missed opportunities with automated alerts

### Daily AI Market Reports
- Automated daily or scheduled summaries
- Includes:
  - New matching listings
  - Price movement highlights
  - Market inventory changes
  - Notable trends in your target area

### AI Real Estate Assistant
Ask questions like:
- “Is this market trending up or down?”
- “How long are homes staying on the market?”
- “How many active, pending, and sold listings are there?”
- “What is the average price per square foot in this ZIP?”

### Market Analytics Dashboard
- Active vs pending vs sold breakdowns
- Days-on-market tracking
- Price trend graphs over time
- Inventory heatmaps (optional extension)
- Comparable property insights

### Alert System
- Email notifications for:
  - New matching listings
  - Price drops
  - Market shifts
- Extensible webhook support (Slack, Telegram, etc.)

---

## Tech Stack

### Backend
- Python 3.11+
- FastAPI (REST API layer)
- Pydantic (data validation)

### Data Collection
- RESO Web API (MLS integration where available)
- Scrapy / BeautifulSoup (controlled scraping layer)
- Async ingestion pipelines

### Database
- PostgreSQL (core relational data)
- PostGIS (geospatial queries)
- Redis (caching + job queues)

### Search & Analytics
- Elasticsearch (fast filtering and search)
- pgvector (semantic search for AI matching and embeddings)

### AI Layer
- LLM integration for:
  - Market Q&A
  - Listing summarization
  - Trend interpretation
- Python-based analytics:
  - pandas
  - NumPy
  - scikit-learn (optional predictive modeling)

### Frontend
- Next.js (React)
- Tailwind CSS
- Chart.js or D3.js (market visualizations)

### Background Processing
- Celery + Redis (task scheduling)
- APScheduler (lightweight alternative)

### DevOps
- Docker (local development)
- Docker Compose (multi-service orchestration)
- Kubernetes-ready deployment structure (optional)

---

## System Workflow

1. User defines home criteria and preferences
2. CasaBot stores search profiles in database
3. Background workers ingest listing data continuously
4. Matching engine filters listings against user criteria
5. AI layer analyzes and summarizes relevant data
6. Alerts and reports are generated and delivered daily
7. User interacts with AI assistant for market insights

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
  - [https://roxanneardary.com/casabot/](https://roxanneardary.com/casabot/)

---

## License & Notice Requirements

CasaBot is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- CasaBot specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Contributing

Contributions are welcome and encouraged.

- Fork the repository
- Create a feature branch
- Submit a pull request with clear descriptions
- Ensure compliance with AGPL-3.0+

---

## Vision

CasaBot is designed to replace fragmented home search tools with a unified AI system that continuously monitors the market, explains trends, and ensures you never miss a property that fits your criteria.  
