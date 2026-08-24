# AppealRight Specification
**Know Before You Appeal.**
- HTML Mirror:  [https://roxanneardary.com/appealright-specification/](https://roxanneardary.com/appealright-specification/)  

---

## Overview

**AppealRight** is an AI-powered property tax assessment analysis specification designed to help property owners understand, evaluate, and potentially reduce their property tax assessments.

AppealRight analyzes detailed property information, tax assessments, jurisdictional assessment methodologies, recent comparable sales, pending transactions, assessment anomalies, tax relief programs, and potential appeal risks. The system seeks to identify the lowest reasonably supportable property tax assessment while protecting the property owner from making an appeal that could result in little benefit or a potentially higher assessment.

AppealRight is designed as a modular, jurisdiction-aware system. Core modules provide the universal property assessment, valuation, tax analysis, appeal, risk, and tax relief capabilities. Optional plugin modules provide jurisdiction-specific data sources, government systems, assessment rules, property types, and specialized tax programs.

## Purpose

The purpose of AppealRight is to provide property owners with an evidence-based system for evaluating whether their property may be over-assessed and whether pursuing a tax assessment appeal may be financially beneficial.

The system shall:

- Analyze the current property tax assessment.
- Determine how the assessment was mathematically calculated when sufficient information is available.
- Search for recent comparable property sales.
- Prioritize recent and highly similar comparable properties.
- Give priority to the lowest credible indicated comparable values.
- Determine a supportable market value range.
- Determine the lowest reasonably supportable assessment.
- Identify potential assessment anomalies.
- Warn property owners when evidence suggests their current assessment may already be favorable.
- Calculate potential property tax savings from an assessment reduction.
- Identify potentially applicable tax relief programs.
- Monitor pending comparable transactions for market direction.
- Help property owners make an informed decision about whether to appeal.

---

## Core Principles

### Property Owner Tax Minimization

AppealRight shall seek to identify the lowest property tax assessment that can be reasonably supported by applicable law, verified property information, assessment methodology, and available market evidence.

The system shall not manufacture or manipulate evidence to produce an artificially low assessment.

### Evidence-Based Analysis

Every material valuation, assessment, appeal, or tax relief recommendation shall be supported by identifiable evidence whenever such evidence is available.

### Closed Sales Priority

Verified closed sales shall be the primary market evidence used for comparable-sales valuation.

Pending transactions, asking prices, and other non-closed transactions shall not be treated as equivalent to verified closed sale prices.

### Recent Sales Priority

Only qualifying closed sales occurring within the previous six months shall be used as standard comparable sales for the core valuation analysis.

More recent qualifying sales shall receive greater priority than older qualifying sales.

### Geographic Priority

The system shall initially search for comparable sales within five miles of the subject property.

For property tax assessment purposes, qualifying comparable properties shall be located within the same municipality unless a human-authorized geographic override is used.

### Human Oversight

AppealRight shall maintain human review and override capabilities for circumstances where jurisdictional rules, incomplete data, unusual properties, or insufficient comparable sales require human judgment.

Human overrides shall be documented and auditable.

### Transparent Uncertainty

AppealRight shall distinguish between verified information, calculated information, estimated information, assumptions, and unresolved information.

The system shall not present uncertain conclusions as established facts.

---

## Core Modules

### Property Intake Module

The Property Intake Module shall collect and validate the information required to perform a property assessment analysis.

The module shall support:

- Property address.
- Municipality.
- County.
- State.
- Parcel or property identification number.
- Property type.
- Year built.
- Living area.
- Lot size.
- Bedrooms.
- Bathrooms.
- Stories.
- Garage or parking characteristics.
- Basement characteristics.
- Pool and other major improvements.
- Construction characteristics.
- Condition.
- Renovations and improvements.
- Waterfront, view, or other location characteristics.
- Current assessment.
- Assessment year.
- Assessment date.
- Taxable value where available.
- Property tax information where available.

The module shall allow verified government records and owner-supplied information to be distinguished.

### Property Identification Module

The Property Identification Module shall verify the subject property and establish the authoritative property record used by the analysis.

The module shall identify:

- Legal or official property address.
- Municipality.
- County.
- State.
- Parcel identifier.
- Property classification.
- Assessment jurisdiction.
- Applicable taxing authorities where available.

The module shall detect conflicting property records and flag unresolved discrepancies.

### Property Characteristics Module

The Property Characteristics Module shall normalize property characteristics so that the subject property can be compared with other properties.

The module shall identify and normalize:

- Property type.
- Living area.
- Lot size.
- Age.
- Bedrooms.
- Bathrooms.
- Stories.
- Garage.
- Basement.
- Pool.
- Construction.
- Condition.
- Renovations.
- Special features.
- Location characteristics.

### Municipality Verification Module

The Municipality Verification Module shall establish the official municipality associated with the subject property and comparable properties.

The municipality shall be treated as a primary geographic constraint for normal property tax comparable analysis.

The module shall identify boundary discrepancies and flag properties whose municipal classification is uncertain.

### Tax Assessment Module

The Tax Assessment Module shall retrieve, accept, and analyze the current property tax assessment.

The module shall distinguish between:

- Market value.
- Appraised value.
- Assessed value.
- Taxable value.
- Exempt value.
- Tax liability.
- Assessment ratio.
- Tax rate.

The module shall preserve the applicable assessment year and valuation date.

### Assessment Mathematics Module

The Assessment Mathematics Module shall determine how a property assessment was calculated whenever sufficient jurisdictional information is available.

The module shall support mathematical relationships involving:

- Market value.
- Assessment ratios.
- Classification ratios.
- Equalization ratios.
- Assessment rates.
- Taxable value.
- Exemptions.
- Deductions.
- Caps.
- Freezes.
- Assessment limitations.
- Reassessment factors.
- Other jurisdiction-specific mathematical rules.

The module shall attempt to reproduce the recorded assessment using available official inputs.

If the recorded assessment cannot be reconstructed, the system shall identify the missing inputs, unknown rules, or unresolved calculations.

### Assessment Ratio Module

The Assessment Ratio Module shall identify applicable ratios used to convert market or appraised value into assessed value.

The module shall calculate applicable ratios where sufficient information exists and shall distinguish statutory ratios from calculated or inferred ratios.

### Taxable Value Module

The Taxable Value Module shall determine the property's taxable value after applying applicable exemptions, deductions, caps, freezes, and other legally recognized adjustments.

### Tax Rate Module

The Tax Rate Module shall identify applicable property tax rates and taxing authority components when available.

The module shall support calculations involving:

- Municipal rates.
- County rates.
- School district rates.
- Special district rates.
- Millage rates.
- Combined effective rates.

### Jurisdiction Rules Module

The Jurisdiction Rules Module shall identify assessment and tax rules applicable to the subject property.

The module shall support jurisdiction-specific rules concerning:

- Assessment dates.
- Reassessment cycles.
- Assessment ratios.
- Tax rates.
- Exemptions.
- Assessment caps.
- Assessment freezes.
- Appeal procedures.
- Appeal deadlines.
- Reassessment procedures.
- Tax relief programs.

### Sales Data Acquisition Module

The Sales Data Acquisition Module shall acquire available property sales information from authorized and reliable sources.

The module shall capture:

- Property identifier.
- Address.
- Municipality.
- Sale date.
- Sale price.
- Property characteristics.
- Sale conditions.
- Data source.
- Source date.
- Verification status.

### Comparable Search Module

The Comparable Search Module shall search for potentially comparable closed sales.

The initial search shall be limited to:

- Five miles from the subject property.
- The same municipality.
- Closed sales.
- Sales occurring within the previous six months.

The module shall prioritize the most recent qualifying transactions.

### Six-Month Sales Module

The Six-Month Sales Module shall enforce the six-month qualifying period for standard closed-sale comparable analysis.

The applicable six-month period shall be calculated from the relevant valuation or assessment date when the jurisdiction establishes a specific valuation date.

Sales outside the qualifying period shall not be used as standard comparable sales unless specifically permitted by a jurisdiction-specific rule or human override.

### Municipality Restriction Module

The Municipality Restriction Module shall prevent properties outside the subject property's municipality from entering the normal comparable set for tax assessment analysis.

An outside-municipality property may only be included through the Human Override Module when the required conditions are satisfied.

### Comparable Qualification Module

The Comparable Qualification Module shall determine whether a property is sufficiently similar and reliable to be considered a comparable.

The module shall evaluate:

- Property type.
- Location.
- Sale date.
- Sale conditions.
- Living area.
- Lot size.
- Age.
- Bedrooms.
- Bathrooms.
- Condition.
- Improvements.
- Features.
- Other relevant characteristics.

### Comparable Similarity Module

The Comparable Similarity Module shall calculate a similarity assessment for each candidate comparable.

Similarity shall consider multiple property characteristics rather than relying solely on distance or sale price.

The weighting of characteristics shall be configurable by property type and jurisdiction.

### Comparable Adjustment Module

The Comparable Adjustment Module shall identify meaningful differences between the subject property and comparable properties.

Where sufficient evidence exists, the module shall estimate appropriate adjustments for differences in:

- Size.
- Lot.
- Age.
- Condition.
- Improvements.
- Features.
- Location.
- Other material characteristics.

Adjustments shall be transparent and documented.

### Comparable Ranking Module

The Comparable Ranking Module shall rank qualifying properties according to:

- Sale recency.
- Similarity.
- Geographic proximity.
- Property characteristics.
- Sale reliability.
- Required adjustments.
- Data quality.
- Indicated value.

The most recent and most similar qualifying properties shall generally receive greater priority.

### Lowest Credible Indicated Value Module

The Lowest Credible Indicated Value Module shall identify the lowest credible market value indicated by sufficiently comparable evidence.

The system shall not automatically select the lowest sale price.

A low-value comparable shall receive priority only when it remains sufficiently comparable and credible after evaluating property characteristics, sale conditions, adjustments, and data quality.

The module shall seek the lowest supportable valuation rather than an artificially minimized valuation.

### Comparable Exclusion Module

The Comparable Exclusion Module shall identify sales that should not be treated as reliable market evidence.

Potential exclusions shall include:

- Non-arm's-length transactions.
- Family transfers.
- Nominal consideration.
- Estate transfers where market conditions are unclear.
- Transfers involving unusual conditions.
- Insufficiently documented sales.
- Duplicate records.
- Incorrect property matches.
- Other transactions determined to be unreliable.

Excluded transactions shall remain documented in the audit trail with the reason for exclusion.

### Market Value Analysis Module

The Market Value Analysis Module shall calculate an evidence-based indication of current market value.

The module shall support:

- Unadjusted sale analysis.
- Median sale analysis.
- Weighted comparable analysis.
- Price-per-square-foot analysis.
- Adjusted comparable analysis.
- Market value ranges.
- Central market value estimates.
- Lower and upper supportable values.

### Lowest Supportable Value Module

The Lowest Supportable Value Module shall determine the lowest market value that can reasonably be supported by qualified evidence.

The module shall consider:

- Lowest credible indicated comparable value.
- Comparable similarity.
- Sale recency.
- Sale reliability.
- Adjustment requirements.
- Number of qualifying comparables.
- Dispersion among comparable values.
- Data quality.

The system shall never select a lower value solely because it produces a more favorable tax result.

### Value Reconciliation Module

The Value Reconciliation Module shall reconcile multiple valuation indicators into a final supportable market value range.

The system shall explain why particular evidence receives greater or lesser weight.

### Confidence Analysis Module

The Confidence Analysis Module shall calculate a confidence classification based on:

- Number of qualifying comparables.
- Similarity of comparables.
- Recency.
- Geographic concentration.
- Data quality.
- Adjustment magnitude.
- Agreement between valuation methods.

Possible classifications shall include:

- High Confidence.
- Moderate Confidence.
- Low Confidence.
- Insufficient Evidence.

### Pending Sales Module

The Pending Sales Module shall identify comparable properties that are:

- Listed.
- Under contract.
- Pending.
- Awaiting settlement.
- Awaiting closing.

Pending properties shall be monitored separately from closed sales.

Pending transactions shall not be used as closed-sale comparables for the core market value calculation.

### Pending Price Tracking Module

The Pending Price Tracking Module shall monitor, where available:

- Original asking price.
- Current asking price.
- Price reductions.
- Contract price.
- Pending date.
- Days on market.
- Eventual closed price.

The module shall preserve the historical progression from listing to contract to closing.

### Market Direction Module

The Market Direction Module shall analyze pending and under-contract comparable properties for indications of market movement.

The module may identify:

- Upward market trends.
- Downward market trends.
- Stable market conditions.
- Increasing negotiation discounts.
- Increasing premiums over asking price.
- Increasing price reductions.
- Changes in marketing time.

Pending and asking prices shall be treated as forward-looking market intelligence and shall not be substituted for verified closed sale prices.

### Pending Sale Warning Module

The Pending Sale Warning Module shall notify property owners when pending transactions suggest that market conditions may be moving materially higher or lower than recent closed-sale evidence.

The system shall clearly explain that pending sales provide market direction information rather than definitive appraisal or assessment evidence.

### Search Expansion Module

If insufficient qualifying comparable sales are found within five miles, the Search Expansion Module may expand the geographic search.

The system shall expand the search only when the available qualifying evidence is insufficient.

The system shall record:

- Original search radius.
- Expanded search radius.
- Number of qualifying properties found.
- Reason for expansion.
- Municipalities included.

### Human Override Module

The Human Override Module shall allow an authorized human reviewer to expand the comparable search outside the subject municipality when no sufficiently similar qualifying properties have sold within the municipality.

The system shall record:

- Human reviewer.
- Date and time.
- Reason for override.
- Original geographic restriction.
- Expanded geographic area.
- Properties added through the override.
- Reason each outside-municipality property was considered relevant.

Out-of-municipality comparables shall be clearly identified in all reports.

### Assessment Anomaly Detection Module

The Assessment Anomaly Detection Module shall identify material discrepancies between the current assessment and the system's independent assessment analysis.

A discrepancy of **20% or greater** shall trigger an Assessment Anomaly Alert and require further research into the property's tax assessment.

The module shall identify:

- Potential overassessment.
- Potential underassessment.
- Assessment ratio anomalies.
- Comparative assessment anomalies.
- Unusual assessment calculations.
- Significant discrepancies between comparable properties.

A 20% anomaly shall trigger investigation and shall not automatically be treated as proof of an incorrect assessment.

### Comparative Assessment Anomaly Module

The system shall compare assessment-to-value relationships among similar properties when sufficient data is available.

The module shall identify materially different assessment ratios among otherwise similar properties and flag potential inequities for additional research.

### Tax Appeal Module

The Tax Appeal Module shall be a core component of AppealRight.

The module shall evaluate whether the available evidence supports seeking a lower property tax assessment.

The system shall compare:

- Current assessment.
- Lowest supportable market value.
- Applicable assessment ratio.
- Calculated target assessment.
- Existing taxable value.
- Potential reduced taxable value.
- Current tax burden.
- Projected tax burden.
- Potential annual savings.
- Potential appeal risks.

When comparable sales and applicable calculations indicate that a lower assessment is reasonably supportable, the system shall recommend considering an appeal.

### Appeal Recommendation Module

The Appeal Recommendation Module shall evaluate both potential benefit and potential downside.

Possible recommendations shall include:

- Appeal Recommended.
- Appeal Recommended With Caution.
- Possible Appeal.
- Appeal Not Recommended.
- Do Not Appeal.
- Insufficient Evidence.

The recommendation shall explain the evidence supporting the conclusion.

### Target Assessment Module

The Target Assessment Module shall calculate the lowest reasonably supportable assessment based on the available market evidence and applicable jurisdictional assessment methodology.

The target assessment shall not be based solely on the lowest sale price.

The system shall show the mathematical path from market evidence to target assessment.

### Assessment Risk Analysis Module

Before recommending an appeal, the system shall analyze whether recent comparable sales indicate that the current assessment may already be favorable.

The system shall identify:

- Potential higher market value.
- Potential higher assessment.
- Potential assessment increase.
- Potential tax increase.
- Current assessment advantage.
- Appeal downside risk.

### Appeal Downside Analysis Module

The system shall determine whether applicable jurisdictional rules permit an assessment increase, reassessment, or other adverse consequence during an appeal.

If the rules are unknown, the system shall identify the risk as unknown rather than assuming that an assessment cannot increase.

### Tax Savings Calculation Module

The Tax Savings Calculation Module shall calculate potential savings resulting from a supportable assessment reduction.

The system shall calculate:

- Current assessment.
- Target assessment.
- Assessment reduction.
- Current estimated tax.
- Projected estimated tax.
- Estimated annual savings.
- Monthly equivalent savings.
- Projected multi-year savings when appropriate.

Where multiple taxing authorities apply different rates, the system shall calculate the components separately and provide a combined estimate.

### Tax Relief and Assistance Module

The Tax Relief and Assistance Module shall allow property owners to enter existing tax assistance, rebates, exemptions, credits, deductions, freezes, caps, and other benefits.

The module shall support information concerning:

- Homestead exemptions.
- Age-based exemptions.
- Senior tax freezes.
- Income-based programs.
- Veteran benefits.
- Surviving spouse benefits.
- Disability-related programs where applicable.
- Tax rebates.
- Tax credits.
- Tax deferrals.
- Assessment caps.
- Assessment freezes.
- Agricultural benefits.
- Local tax assistance.
- County tax assistance.
- State tax assistance.
- Other jurisdiction-specific programs.

### Tax Relief Discovery Module

The Tax Relief Discovery Module shall search applicable municipal, county, state, and other governmental programs to identify potentially qualifying tax relief opportunities.

The system shall evaluate available eligibility requirements including:

- Age.
- Income.
- Ownership.
- Residency.
- Property use.
- Primary residence status.
- Veteran status.
- Disability qualifications where applicable.
- Filing requirements.
- Program-specific conditions.

### Tax Relief Eligibility Module

The system shall classify potential program eligibility as:

- Likely Eligible.
- Possibly Eligible.
- Likely Ineligible.
- Unknown.

The system shall not represent an unverified eligibility determination as a guarantee of benefits.

### Tax Benefit Stacking Module

The Tax Benefit Stacking Module shall determine whether multiple tax benefits may legally be combined.

When benefits cannot be combined, the system shall identify the most financially advantageous permissible combination when sufficient information is available.

### Tax Burden Optimization Module

The Tax Burden Optimization Module shall evaluate the combined effect of:

- Assessment reduction.
- Exemptions.
- Rebates.
- Credits.
- Deductions.
- Freezes.
- Caps.
- Deferrals.
- Other applicable tax relief.

The module shall identify the lowest legally supportable property tax burden based on available evidence and applicable rules.

### Appeal Evidence Module

The Appeal Evidence Module shall collect and organize evidence supporting or opposing an appeal.

Evidence may include:

- Property records.
- Assessment records.
- Comparable sales.
- Comparable property characteristics.
- Assessment calculations.
- Assessment ratios.
- Tax rates.
- Tax relief programs.
- Jurisdictional rules.
- Pending market indicators.
- Anomaly findings.

### Appeal Report Module

The Appeal Report Module shall produce an appraisal-style property tax assessment analysis.

The report shall include:

- Property identification.
- Property characteristics.
- Current assessment.
- Assessment date.
- Assessment methodology.
- Comparable search methodology.
- Comparable sales.
- Comparable ranking.
- Comparable adjustments.
- Lowest credible indicated value.
- Market value range.
- Target assessment.
- Assessment anomaly findings.
- Pending market analysis.
- Appeal recommendation.
- Appeal downside analysis.
- Estimated tax savings.
- Tax relief opportunities.
- Sources.
- Confidence level.
- Limitations.
- Human overrides.

### Source Verification Module

The Source Verification Module shall identify and verify the origin of material data used by the system.

The system shall preserve:

- Source name.
- Source location.
- Retrieval date.
- Data type.
- Verification status.
- Relevant jurisdiction.

### Data Provenance Module

The Data Provenance Module shall maintain a traceable record of information used to reach material conclusions.

Each material calculation shall be traceable to its underlying inputs whenever technically possible.

### Data Freshness Module

The Data Freshness Module shall identify the age of important data and warn when information may no longer accurately represent the current assessment or market.

### Audit Trail Module

The Audit Trail Module shall record material system actions and decisions, including:

- Data retrieval.
- Comparable selection.
- Comparable exclusion.
- Search expansion.
- Human overrides.
- Assessment calculations.
- Tax calculations.
- Anomaly detection.
- Appeal recommendations.
- Tax relief recommendations.

### Human Review Module

The Human Review Module shall provide mechanisms for reviewing, correcting, or overriding system conclusions where appropriate.

Human decisions shall not silently overwrite AI analysis.

The system shall preserve the original AI conclusion and the subsequent human action.

### Decision Transparency Module

The Decision Transparency Module shall explain the major factors that contributed to:

- Comparable selection.
- Valuation.
- Target assessment.
- Anomaly detection.
- Appeal recommendation.
- Tax savings calculation.
- Tax relief recommendation.

### Error Detection Module

The Error Detection Module shall identify:

- Conflicting property records.
- Duplicate sales.
- Invalid dates.
- Missing sale prices.
- Inconsistent assessment values.
- Mathematical inconsistencies.
- Geographic inconsistencies.
- Incorrect municipality assignments.
- Insufficient comparable evidence.

## Core Decision Framework

AppealRight shall use the following general analytical sequence:

**Property Identification**

→ **Assessment Retrieval**

→ **Assessment Mathematics**

→ **Tax Rule Analysis**

→ **Five-Mile Comparable Search**

→ **Six-Month Closed-Sale Qualification**

→ **Municipality Verification**

→ **Comparable Similarity Analysis**

→ **Comparable Ranking**

→ **Lowest Credible Indicated Value**

→ **Market Value Analysis**

→ **Target Assessment Calculation**

→ **Assessment Anomaly Analysis**

→ **Appeal Risk Analysis**

→ **Tax Savings Analysis**

→ **Tax Relief Analysis**

→ **Pending Market Analysis**

→ **Final Appeal Recommendation**

## Comparable Sales Rules

The following rules shall govern standard comparable sales analysis:

- Only closed sales shall qualify as standard comparable sales.
- Standard comparable sales must have closed within the previous six months.
- The initial geographic search shall be five miles from the subject property.
- Standard tax assessment comparables shall be within the same municipality.
- More recent qualifying sales shall receive priority.
- More similar properties shall receive priority.
- The lowest credible indicated value shall receive priority when supported by comparable evidence.
- Sale price alone shall not determine comparability.
- Non-market transactions shall be excluded or flagged.
- Insufficient comparable evidence shall result in an insufficient-evidence finding rather than forced valuation.
- Geographic expansion shall occur only when sufficient comparable evidence cannot be found.
- Out-of-municipality comparables require human authorization.

## Pending Sales Rules

Pending and under-contract transactions shall be treated as forward-looking market intelligence.

The system shall:

- Monitor pending comparable properties.
- Track asking prices.
- Track price reductions.
- Track pending prices where available.
- Compare asking prices with pending prices.
- Monitor time to contract.
- Track eventual closing prices.
- Identify potential upward or downward market trends.

The system shall not use pending sales as substitutes for closed comparable sales in the core valuation calculation.

## Assessment Anomaly Rules

Any discrepancy of **20% or greater** between the recorded assessment and the independently calculated supportable assessment shall trigger an Assessment Anomaly Alert.

The system shall investigate potential explanations before determining whether the anomaly represents a likely assessment error.

Comparable-property assessment disparities shall also be evaluated where sufficient data exists.

## Appeal Decision Rules

AppealRight shall recommend an appeal when the available evidence indicates that:

- A lower assessment is reasonably supportable.
- The assessment calculation supports a reduction.
- Comparable sales support a lower value.
- The potential tax savings are material.
- Applicable appeal rules permit the proposed action.
- The expected benefit reasonably outweighs identified risks.

The system shall warn the owner when:

- Recent comparable sales indicate a higher value.
- The existing assessment appears favorable.
- The appeal may expose the property to a higher assessment.
- Jurisdictional appeal risks are unknown.
- The potential savings are insufficient to justify the identified risks.

## Tax Burden Objective

AppealRight shall seek to identify the lowest legally supportable tax burden rather than simply the lowest market value.

The system shall evaluate the combined effect of:

- Market value.
- Assessment methodology.
- Assessment ratios.
- Taxable value.
- Exemptions.
- Credits.
- Rebates.
- Freezes.
- Caps.
- Deferrals.
- Other available tax relief.

---

## Optional Plugin Modules

Optional plugins may extend the core system without altering the core specification.

### Government Assessment Data Plugin

Provides direct access to government assessment databases where authorized.

### Property Records Plugin

Provides property ownership, parcel, deed, and property characteristic information.

### Sales Records Plugin

Provides verified closed-sale records from authorized sources.

### MLS and Listing Data Plugin

Provides authorized listing and pending transaction information.

### GIS and Mapping Plugin

Provides parcel boundaries, municipality boundaries, geographic calculations, and mapping capabilities.

### Jurisdiction Rules Plugin

Provides jurisdiction-specific assessment, taxation, and appeal rules.

### Tax Relief Programs Plugin

Provides jurisdiction-specific exemptions, rebates, credits, freezes, caps, deferrals, and other tax relief programs.

### Appeal Deadline Plugin

Provides jurisdiction-specific filing deadlines and appeal schedules.

### Residential Property Plugin

Provides specialized analysis for single-family residential properties.

### Condominium Plugin

Provides specialized analysis for condominium properties.

### Multifamily Plugin

Provides specialized analysis for multifamily properties.

### Commercial Property Plugin

Provides specialized analysis for commercial properties.

### Vacant Land Plugin

Provides specialized analysis for vacant land.

### Agricultural Property Plugin

Provides specialized analysis for agricultural and special-use properties.

### Waterfront Property Plugin

Provides specialized analysis for waterfront and water-access properties.

### Data Verification Plugin

Provides additional verification of property and transaction records.

### Notification Plugin

Provides alerts for:

- New comparable sales.
- Pending comparable transactions.
- Assessment changes.
- Tax relief opportunities.
- Appeal deadlines.
- Market direction changes.
- Assessment anomalies.

### Document Generation Plugin

Provides enhanced generation of property assessment analyses, appeal packages, supporting evidence, and jurisdiction-specific documentation.

### Historical Assessment Plugin

Provides historical assessment and tax records for longitudinal analysis.

### Market Trend Plugin

Provides expanded historical and predictive market trend analysis using authorized data.

---

## Privacy and Security

AppealRight shall protect property owner information and minimize collection of unnecessary personal information.

Sensitive owner information used for tax relief eligibility shall be protected through appropriate access controls and data security practices.

The system shall distinguish publicly available property information from owner-provided private information.

---

## Data Integrity

AppealRight shall prioritize verified and authoritative information for material decisions.

When conflicting sources exist, the system shall identify the conflict and provide the basis for selecting a source.

The system shall not silently substitute estimated data for verified data.

---

## Limitations and Disclaimers

AppealRight is an AI-powered analytical system and shall not represent its output as a legally binding property assessment, government determination, or licensed appraisal unless the applicable implementation independently satisfies all relevant professional and legal requirements.

The system shall clearly distinguish:

- Market analysis.
- Appraisal.
- Tax assessment.
- Taxable value.
- Tax liability.
- Appeal recommendation.
- Tax relief eligibility.

AppealRight shall advise users to verify material conclusions with the applicable taxing authority or qualified professional when appropriate.

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
  - [https://roxanneardary.com/appealright/](https://roxanneardary.com/appealright/)  

---

## License & Notice Requirements

AppealRight is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- AppealRight specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
