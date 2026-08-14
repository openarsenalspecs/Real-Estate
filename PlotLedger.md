# PlotLedger Specification

**The Future of Parcel Intelligence**

PlotLedger is an open-source AI-powered parcel intelligence platform for identifying, organizing, and analyzing properties of nine or more contiguous acres across the United States. The system combines parcel boundaries, ownership records, sale history, zoning regulations, permits, applications, variances, special districts, and other public records into a unified analytical framework.

PlotLedger is designed to make land-use decisions and regulatory differences discoverable through structured data, geospatial analysis, legal comparison, and AI-assisted research.

## Purpose

PlotLedger shall provide a national parcel intelligence system capable of:

- Identifying parcels containing nine or more acres.
- Identifying groups of contiguous parcels that collectively contain nine or more acres.
- Connecting parcels to current and historical ownership records.
- Connecting parcels to historical sales and transaction records.
- Connecting parcels to permits and permit applications.
- Identifying applicable zoning classifications and overlays.
- Ingesting and interpreting applicable local zoning laws and land-use regulations.
- Comparing permitted development against development actually approved.
- Identifying variances, conditional uses, special exceptions, density bonuses, height increases, special districts, development agreements, and other regulatory privileges.
- Maintaining a verifiable evidence trail for every analytical conclusion.
- Providing searchable national and state-level parcel directories.
- Supporting interactive geographic exploration and parcel comparison.
- Continuously updating records as new public information becomes available.

## Design Principles

PlotLedger shall be designed around the following principles:

- **Open source:** Core functionality shall remain available under the project's open-source license.
- **Modularity:** Data providers, jurisdictions, analytical systems, and optional capabilities shall be independently extensible.
- **Local-first data processing:** Data should be processed and retained locally whenever practical.
- **Source transparency:** AI-generated conclusions must remain connected to their underlying sources.
- **Evidence before inference:** The system shall distinguish documented facts from AI interpretations and predictions.
- **Jurisdictional accuracy:** Zoning analysis must account for the specific jurisdiction and version of law applicable to a property.
- **Historical awareness:** Regulations, ownership, permits, and approvals shall be treated as time-dependent records.
- **Human review:** Legal and regulatory conclusions shall be presented as analytical findings rather than substitutes for professional legal advice.
- **Interoperability:** Data should use documented schemas and standard geospatial formats wherever practical.
- **Vendor independence:** The system shall avoid unnecessary dependence on proprietary data providers or closed platforms.

# Core Modules

## Parcel Discovery Module

The Parcel Discovery Module shall identify properties meeting PlotLedger's acreage criteria.

Capabilities shall include:

- Import parcel boundaries from public GIS and cadastral sources.
- Calculate parcel acreage from authoritative geometry.
- Identify individual parcels containing at least nine acres.
- Identify contiguous parcels that collectively contain at least nine acres.
- Detect shared boundaries and geographic adjacency.
- Distinguish true geographic contiguity from parcels separated by unrelated properties, roads, waterways, or other boundaries when applicable.
- Maintain parcel identifiers from the originating jurisdiction.
- Preserve source geometry and source metadata.
- Track changes to parcel boundaries over time where historical data is available.

## Contiguous Ownership Module

The Contiguous Ownership Module shall determine when multiple parcels should be analyzed as a combined landholding.

Capabilities shall include:

- Compare ownership records across adjacent parcels.
- Normalize variations in owner names.
- Identify corporations, LLCs, trusts, partnerships, government entities, and other ownership structures.
- Detect probable common ownership where legally supportable evidence exists.
- Group qualifying parcels without destroying individual parcel identities.
- Record the evidence supporting ownership relationships.
- Distinguish confirmed ownership relationships from inferred relationships.
- Track ownership changes over time.

## Ownership Intelligence Module

The Ownership Intelligence Module shall create a structured ownership record for each qualifying parcel or parcel group.

Capabilities shall include:

- Current owner identification.
- Historical owner identification.
- Ownership transfer dates.
- Ownership entity type.
- Recorded ownership relationships.
- Related parcel holdings where supported by public records.
- Ownership history normalization.
- Source documentation for ownership claims.
- Historical ownership timelines.
- Search by owner, entity, parcel, county, state, and jurisdiction.

## Sale History Module

The Sale History Module shall connect qualifying parcels to available historical transaction records.

Capabilities shall include:

- Sale dates.
- Recorded sale prices when available.
- Grantor and grantee records.
- Transaction types.
- Deed references.
- Historical transaction timelines.
- Price-per-acre calculations.
- Parcel aggregation and subdivision effects on transaction history.
- Identification of ownership transfers that do not represent conventional market sales.
- Source references for every transaction.

## Zoning Intelligence Module

The Zoning Intelligence Module shall identify the regulatory framework applicable to each parcel.

Capabilities shall include:

- Current zoning designation.
- Historical zoning designations.
- Future land-use classifications.
- Overlay districts.
- Special districts.
- Comprehensive plan designations.
- Development standards.
- Permitted uses.
- Conditional uses.
- Special exceptions.
- Density limitations.
- Intensity limitations.
- Height restrictions.
- Setback requirements.
- Lot requirements.
- Parking requirements.
- Open-space requirements.
- Applicable jurisdiction.
- Effective dates of applicable regulations.

## Zoning Law Analysis Module

The Zoning Law Analysis Module shall ingest and structure local zoning laws, ordinances, land-development regulations, comprehensive plans, municipal codes, and related regulatory documents.

AI shall:

- Extract zoning rules from authoritative legal sources.
- Identify definitions relevant to development rights.
- Identify applicable acreage thresholds.
- Identify special district requirements.
- Identify conditional use requirements.
- Identify variance standards.
- Identify density and intensity provisions.
- Identify height and dimensional standards.
- Identify procedural requirements.
- Associate regulations with jurisdictions and effective dates.
- Preserve citations to the source documents.
- Identify conflicts between multiple applicable regulatory provisions.
- Flag uncertain or ambiguous interpretations for human review.

## Permit Intelligence Module

The Permit Intelligence Module shall connect permits and permit applications to individual parcels and qualifying parcel groups.

Capabilities shall include:

- Building permits.
- Demolition permits.
- Land-development permits.
- Site-plan applications.
- Rezoning applications.
- Conditional-use applications.
- Special-exception applications.
- Variance applications.
- Environmental applications.
- Subdivision applications.
- Development agreements.
- Other publicly available regulatory applications.

The module shall maintain:

- Application numbers.
- Permit numbers.
- Application dates.
- Decision dates.
- Applicant information.
- Owner information where available.
- Project descriptions.
- Permit status.
- Approval status.
- Expiration information.
- Associated documents.
- Parcel identifiers.
- Source references.

## Regulatory Comparison Module

The Regulatory Comparison Module shall compare what local law permits with what was actually requested, approved, or constructed.

AI shall evaluate:

- Permitted development versus proposed development.
- Permitted development versus approved development.
- Standard zoning requirements versus granted variances.
- Standard density versus approved density.
- Standard height versus approved height.
- Standard uses versus approved uses.
- Standard setbacks versus approved setbacks.
- Standard parking requirements versus approved requirements.
- Standard dimensional requirements versus approved modifications.
- Applicable procedures versus procedures documented in the record.

The system shall classify findings as:

- **Standard:** Consistent with documented regulations.
- **Modified:** Approval contains documented modifications to ordinary requirements.
- **Exception:** Approval relies on a variance, conditional use, special exception, or comparable mechanism.
- **Special District:** Property receives rights associated with a special zoning or development district.
- **Unresolved:** Available records are insufficient to establish the applicable regulatory basis.

The system shall never label an approval as unlawful solely because it differs from a standard zoning rule. A difference shall be investigated against the applicable variance, special district, ordinance, development agreement, or other legal authority.

## Special Privilege Detection Module

The Special Privilege Detection Module shall identify documented regulatory advantages or exceptions associated with qualifying parcels.

Potential findings shall include:

- Density increases.
- Height increases.
- Reduced setbacks.
- Expanded permitted uses.
- Conditional uses.
- Special exceptions.
- Variances.
- Overlay benefits.
- Special district rights.
- Development agreements.
- Planned development approvals.
- Transferable development rights.
- Incentive-based development rights.
- Expedited development procedures.
- Other documented deviations from baseline regulations.

Every finding shall include:

- The applicable baseline rule.
- The actual approved condition.
- The legal mechanism authorizing the difference.
- The relevant decision-making body.
- The approval date.
- The supporting source.
- Confidence level.
- AI interpretation.
- Human-review status.

## Legal Evidence Module

The Legal Evidence Module shall provide an auditable evidence chain for zoning and regulatory findings.

Each analytical claim shall be traceable to:

- Source document.
- Source URL or document identifier.
- Jurisdiction.
- Publication or adoption date when available.
- Effective date.
- Relevant section or provision.
- Permit or application record.
- Parcel identifier.
- Date accessed.
- Data provider.
- Extraction method.

AI-generated conclusions shall remain distinguishable from source facts.

## Permit-to-Parcel Linking Module

The Permit-to-Parcel Linking Module shall associate permits and applications with the correct geographic property.

Matching methods shall include:

- Parcel identification numbers.
- Addresses.
- Legal descriptions.
- Geographic coordinates.
- Applicant information.
- Owner information.
- Project names.
- Subdivision references.
- Document references.
- Spatial intersection.
- Historical parcel relationships.

The system shall assign confidence levels to automated matches and allow human correction.

## State Directory Module

The State Directory Module shall maintain a national directory organized by state, county, municipality, and other applicable jurisdictions.

Each state directory shall support:

- Qualifying parcels.
- Qualifying parcel groups.
- Owners.
- Sale history.
- Zoning.
- Permits.
- Applications.
- Special districts.
- Variances.
- Regulatory comparisons.
- Development activity.
- Source records.

The architecture shall allow states and jurisdictions to be added independently without redesigning the core system.

## Geographic Intelligence Module

The Geographic Intelligence Module shall provide spatial analysis and visualization.

Capabilities shall include:

- Interactive parcel maps.
- Parcel boundary visualization.
- Contiguous parcel visualization.
- Zoning overlays.
- Permit locations.
- Special district boundaries.
- Ownership group visualization.
- Development activity mapping.
- Geographic filtering.
- Distance analysis.
- Adjacency analysis.
- Acreage calculations.
- Historical boundary comparison.

## Search and Discovery Module

The Search and Discovery Module shall allow users to search by:

- State.
- County.
- Municipality.
- Parcel identifier.
- Address.
- Owner.
- Ownership entity.
- Acreage.
- Zoning classification.
- Permit type.
- Permit status.
- Application status.
- Special privilege type.
- Development activity.
- Sale history.
- Geographic area.

Search results shall link directly to supporting parcel records and source evidence.

## AI Research Module

The AI Research Module shall provide natural-language analysis across PlotLedger's structured records and source documents.

Users shall be able to ask questions such as:

- Which qualifying parcels received density increases?
- Which parcels received zoning variances?
- Which properties have active development applications?
- Which owners control contiguous qualifying parcels?
- Which parcels changed ownership recently?
- Which jurisdictions have approved special development districts?
- What special permissions were granted to a specific parcel?
- What did local zoning allow before an approval?
- What changed after the approval?

AI responses shall cite the underlying records and distinguish verified facts from analytical conclusions.

## Data Quality Module

The Data Quality Module shall detect and manage:

- Missing records.
- Duplicate parcels.
- Duplicate permits.
- Conflicting ownership records.
- Inconsistent acreage measurements.
- Broken source links.
- Outdated zoning information.
- Conflicting effective dates.
- Low-confidence parcel matches.
- Low-confidence ownership matches.
- AI extraction errors.

Data quality issues shall be surfaced rather than silently corrected.

## Historical Versioning Module

The Historical Versioning Module shall preserve changes to:

- Parcel boundaries.
- Ownership.
- Sale history.
- Zoning.
- Ordinances.
- Permits.
- Applications.
- Variances.
- Special districts.
- Development approvals.

Historical analysis shall use the law and parcel configuration applicable to the relevant date whenever sufficient records are available.

## Reporting Module

The Reporting Module shall generate parcel intelligence reports containing:

- Parcel overview.
- Acreage.
- Ownership.
- Sale history.
- Zoning.
- Applicable regulations.
- Permit history.
- Active applications.
- Special approvals.
- Regulatory comparisons.
- AI findings.
- Evidence sources.
- Confidence levels.
- Data quality warnings.

Reports shall clearly distinguish public-record facts from AI-generated analysis.

## Notification Module

The Notification Module shall optionally notify users when relevant records change.

Events may include:

- New qualifying parcels.
- Ownership changes.
- New sales.
- New permit applications.
- Permit approvals.
- New variances.
- New zoning applications.
- Zoning changes.
- New special districts.
- Development agreements.
- Changes to applicable regulations.

# Optional Plugin Modules

## Data Provider Plugins

Data Provider Plugins shall allow jurisdictions and public data providers to be added without modifying core functionality.

Plugins may support:

- GIS services.
- Parcel databases.
- Assessor records.
- Recorder records.
- Permit systems.
- Planning systems.
- Municipal open-data portals.
- State data systems.

## Jurisdiction Plugins

Jurisdiction Plugins shall provide jurisdiction-specific:

- Zoning schemas.
- Regulatory terminology.
- Parcel identifiers.
- Permit types.
- Data mappings.
- Legal document sources.
- Special district classifications.
- Development procedures.

## Legal Document Plugins

Legal Document Plugins may provide specialized ingestion and analysis for:

- Municipal codes.
- County ordinances.
- Zoning codes.
- Comprehensive plans.
- Development agreements.
- Planning commission records.
- Board decisions.
- Public hearing documents.

## AI Model Plugins

AI Model Plugins may allow users to select different models for:

- Document extraction.
- Legal classification.
- Entity resolution.
- Permit matching.
- Regulatory comparison.
- Natural-language search.
- Summarization.
- Anomaly detection.

## Ownership Entity Resolution Plugin

This plugin may identify relationships between:

- LLCs.
- Corporations.
- Trusts.
- Partnerships.
- Parent entities.
- Subsidiaries.
- Commonly controlled entities.

All inferred relationships shall be clearly labeled as inferred rather than established facts.

## Market Intelligence Plugin

This optional plugin may analyze:

- Comparable sales.
- Price-per-acre trends.
- Transaction frequency.
- Ownership concentration.
- Development activity.
- Market changes around qualifying parcels.

## Development Scenario Plugin

This optional plugin may model hypothetical development scenarios using documented zoning constraints and approvals.

It shall distinguish:

- Existing rights.
- Documented exceptions.
- Hypothetical assumptions.
- AI-generated scenarios.

## Alert and Monitoring Plugin

This plugin may provide continuous monitoring of selected:

- Parcels.
- Owners.
- Jurisdictions.
- Zoning changes.
- Permit systems.
- Planning agendas.
- Public records.

## Export Plugin

This plugin may support export to:

- CSV.
- GeoJSON.
- Shapefile-compatible formats.
- GeoPackage.
- JSON.
- PDF reports.
- Other documented formats.

# AI Governance

PlotLedger's AI systems shall operate under evidence-based rules.

AI shall:

- Identify the sources used for conclusions.
- Preserve source references.
- State uncertainty.
- Avoid presenting legal interpretations as definitive legal advice.
- Distinguish facts from inference.
- Identify missing information.
- Allow human review.
- Preserve corrections.
- Avoid fabricating records, permits, laws, owners, or approvals.

AI shall not infer that a regulatory difference constitutes corruption, favoritism, illegality, or misconduct without sufficient documented evidence.

The preferred terminology for documented regulatory differences shall include terms such as **variance**, **special exception**, **conditional approval**, **density bonus**, **special district**, **development agreement**, **regulatory modification**, or another legally supported classification.

# Data Provenance

Every significant record shall maintain provenance metadata.

Provenance shall include, when available:

- Original source.
- Source publisher.
- Source URL.
- Dataset identifier.
- Document identifier.
- Retrieval date.
- Publication date.
- Effective date.
- Jurisdiction.
- Transformation history.
- AI processing history.
- Confidence level.

Derived records shall remain connected to their source records.

# Privacy and Responsible Data Use

PlotLedger shall prioritize public-record property intelligence while limiting unnecessary exposure of sensitive personal information.

The system shall:

- Use publicly available property and regulatory records.
- Avoid collecting unnecessary personal information.
- Avoid publishing sensitive contact information when it is not necessary for the application's purpose.
- Respect applicable data-use restrictions.
- Respect source licensing requirements.
- Clearly identify third-party datasets and their licensing conditions.
- Provide mechanisms for correcting inaccurate records where appropriate.

# Legal and Regulatory Disclaimer

PlotLedger is an information and analytical system. It does not provide legal advice, determine legal rights, or replace review by qualified professionals.

A difference between a baseline zoning requirement and an approved development condition does not by itself establish that an unlawful action occurred. Regulatory findings shall be supported by source records and presented according to the legal mechanism documented in the applicable record.

# Data Source Requirements

PlotLedger should prioritize authoritative sources, including:

- County property appraisers.
- County assessors.
- County GIS systems.
- Municipal GIS systems.
- County recorders.
- Municipal permit systems.
- Planning departments.
- Zoning departments.
- Public legislative records.
- Official municipal and county codes.
- Official state records.
- Other authoritative public sources.

Secondary sources may supplement authoritative records but shall not silently replace them.

# Security

PlotLedger shall protect stored credentials, API keys, private configuration, and other sensitive technical information.

The system shall:

- Never expose provider credentials in public datasets.
- Separate credentials from source code.
- Validate imported data.
- Sanitize externally supplied content.
- Log relevant system events.
- Protect administrative functions.
- Provide configurable access controls where required.
- Preserve audit information for important data transformations.

# Testing

Testing shall cover:

- Parcel geometry.
- Acreage calculations.
- Contiguity detection.
- Ownership matching.
- Sale history matching.
- Permit-to-parcel matching.
- Zoning classification.
- Legal document extraction.
- Regulatory comparison.
- AI output validation.
- Source provenance.
- Historical versioning.
- Data update processes.

Tests shall include edge cases involving irregular parcels, ownership changes, parcel splits, parcel mergers, annexations, jurisdictional changes, and conflicting source records.

---

**PlotLedger**  
*The Future of Parcel Intelligence*

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
