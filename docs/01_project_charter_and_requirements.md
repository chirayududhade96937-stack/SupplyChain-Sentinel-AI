
# 1. Project Overview

## Project Name
SupplyChain Sentinel AI

## Project Description

SupplyChain Sentinel AI is a data analytics and decision-support project focused on understanding potential risks affecting global supply chains.

The project aims to bring together information from geopolitical events, natural disasters and other external disruptions to identify sourcing regions that may require closer attention.

By combining real-world external data with an illustrative procurement portfolio, the platform will help users explore potential exposure, understand emerging risk signals and investigate the evidence behind them.

## Primary Goal

To develop an explainable platform that transforms scattered external data into meaningful supply chain risk insights and supports better-informed business decisions.

## Project Type

End-to-end Business Analytics, Data Engineering and AI Decision-Support Project.

## Intended Users

- Supply chain analysts
- Procurement teams
- Logistics and operations managers
- Business decision-makers


# 2. Business Problem

## Background

Global supply chains depend on sourcing locations, transport networks and infrastructure spread across different countries. Events such as geopolitical conflicts, natural disasters and infrastructure disruptions can create uncertainty for businesses that rely on international sourcing.

However, information about these events is often scattered across multiple sources. This makes it difficult for businesses to connect external events with their sourcing locations and understand which potential risks deserve attention.

## Key Business Challenges

1. **Late Risk Identification:** Businesses may not identify emerging disruptions early enough to investigate their potential impact.

2. **Geopolitical Uncertainty:** Political instability, conflicts and trade-related developments can create uncertainty around sourcing regions.

3. **Natural Disaster Exposure:** Earthquakes, cyclones and other natural hazards may affect infrastructure and operations near sourcing locations.

4. **Limited Supply Chain Visibility:** Information about external events and procurement locations is often maintained separately, making potential exposure difficult to assess.

5. **Information Overload:** Large volumes of news and event reports can make it difficult to distinguish meaningful signals from irrelevant information.

6. **Inconsistent Risk Assessment:** Without a common assessment framework, different risks may be evaluated subjectively or inconsistently.

7. **Fragmented Reporting:** Decision-makers may lack a single view that connects potential risks with supporting information and evidence.

## Problem Statement

There is a need for a centralised and explainable analytical approach that brings together external disruption information and illustrative procurement data to identify potentially exposed sourcing regions, prioritise further investigation and support better-informed business decisions.


# 3. Business Objectives

The main objective of SupplyChain Sentinel AI is to create an analytical platform that helps users identify, assess and investigate potential supply chain risks.

The project will focus on the following objectives:

1. **Integrate External Data:** Bring together geopolitical events, natural disasters and other relevant disruption information from multiple data sources.

2. **Build a Unified Data Structure:** Organise raw data into a consistent format that supports reliable analysis and reporting.

3. **Identify Potential Exposure:** Connect external events with the illustrative procurement portfolio to highlight sourcing regions that may be affected.

4. **Develop a Risk Assessment Framework:** Create a transparent scoring approach to rank potential risks based on severity, location, recency and supporting evidence.

5. **Enable Business Analysis:** Use SQL, Python and Excel to investigate trends, identify patterns and generate meaningful insights.

6. **Create Interactive Reporting:** Develop Power BI dashboards that provide an overview of potential risks and allow users to investigate individual events.

7. **Incorporate Generative AI:** Explore how AI can summarise event information and explain risk assessments using available evidence.

8. **Support Better Decisions:** Present clear, traceable insights that help users prioritise further investigation and make informed sourcing and logistics decisions.

## Expected Outcome

A working decision-support prototype that transforms external disruption data into explainable risk insights, helping users understand where potential supply chain vulnerabilities may require attention.


# 4. Project Scope

## 4.1 In Scope

The project will include the following activities and components:

1. **External Data Collection:** Collect relevant geopolitical, natural disaster and disruption-related information from selected public data sources.

2. **Data Processing and Storage:** Use Python and Google BigQuery to ingest, validate, clean and organise the collected data.

3. **Data Analysis:** Apply SQL and Python to explore disruption patterns, analyse trends, identify duplicates and investigate relationships between events and sourcing regions.

4. **Illustrative Procurement Portfolio:** Develop a synthetic procurement dataset representing 15 sourcing countries, 5 procurement categories and hypothetical sourcing locations and transport corridors.

5. **Geographic Risk Screening:** Assess the potential proximity of external events and natural hazards to the illustrative sourcing locations.

6. **Risk Assessment Framework:** Develop an explainable scoring model to prioritise potential risks using defined assessment factors.

7. **Business Intelligence Reporting:** Use Excel and Power BI to create analytical reports and interactive dashboards.

8. **Generative AI Integration:** Explore evidence-grounded event summaries, risk explanations and investigation briefs.

9. **Documentation and Testing:** Document the architecture, data sources, analytical decisions, limitations, testing results and project progress.

## 4.2 Out of Scope

The following activities are outside the scope of this prototype:

1. **Real Supplier Monitoring:** The project will not access or monitor confidential supplier databases or actual company procurement records.

2. **Confirmed Disruption Detection:** The platform will not claim that a supplier, facility, port or shipment has been directly affected without verified evidence.

3. **Predictive Forecasting:** The initial version will not predict the probability of supplier failure, shipment delays or financial losses.

4. **Live Operational Integration:** The prototype will not connect directly to enterprise ERP, procurement or logistics management systems.

5. **Automated Business Decisions:** The platform will not independently approve suppliers, change sourcing arrangements or make procurement decisions.

6. **Commercial Deployment:** The project is intended as a portfolio and learning prototype, not a production-ready enterprise application.

## 4.3 Scope Boundaries

The project will use real-world external event and hazard observations alongside a clearly labelled synthetic procurement portfolio.

Any geographic matching or risk score will represent a potential exposure signal requiring further investigation, not confirmation of actual business impact.

The initial implementation will prioritise a reliable and explainable analytical workflow over unnecessary complexity or expensive infrastructure.


# 5. Stakeholders

The platform is designed to support different business functions involved in sourcing, procurement, logistics and supply chain risk management.

## 5.1 Primary Stakeholders

1. **Supply Chain Analysts**
   - Monitor external disruption signals.
   - Analyse potential risks across sourcing regions.
   - Investigate trends and supporting evidence.

2. **Procurement Teams**
   - Understand potential risks associated with sourcing countries and procurement categories.
   - Review regions that may require additional attention.
   - Support sourcing risk assessments.

3. **Logistics and Operations Managers**
   - Monitor events that may affect transport infrastructure and logistics networks.
   - Investigate potential geographical exposure.
   - Support operational contingency discussions.

4. **Business Decision-Makers**
   - Review consolidated risk information.
   - Understand priority areas and emerging trends.
   - Use analytical insights to support strategic discussions.

## 5.2 Project Owner and Developer

**Project Owner:** Individual project developer.

The project developer is responsible for:
- Defining business requirements and project objectives.
- Researching and collecting relevant data.
- Designing the data architecture and analytical workflow.
- Developing SQL queries, Python scripts and risk assessment logic.
- Building Excel reports and Power BI dashboards.
- Integrating and evaluating Generative AI capabilities.
- Testing, documenting and maintaining the project.

## 5.3 Stakeholder Expectations

The platform should provide:
- Clear and understandable risk information.
- Traceable evidence behind identified events.
- Consistent and explainable risk assessments.
- Interactive reporting for further investigation.
- Appropriate warnings about data quality and analytical limitations.


# 6. Business Questions

The platform will aim to answer the following business questions:

## 6.1 Global Risk Monitoring

1. Which sourcing countries are currently showing the highest number of potential disruption signals?
2. Which countries have experienced an increase in reported geopolitical or natural hazard events?
3. Which regions require closer monitoring based on recent event activity?

## 6.2 Geopolitical Risk Analysis

4. What types of geopolitical events are being reported across the monitored sourcing countries?
5. Which countries are experiencing recurring geopolitical instability or trade-related developments?
6. How have geopolitical event patterns changed over time?

## 6.3 Natural Hazard Analysis

7. Which sourcing regions have recorded nearby earthquakes or tropical cyclone activity?
8. How frequently do natural hazard events occur near the illustrative sourcing locations?
9. Which locations may require further geographical exposure investigation?

## 6.4 Procurement Exposure Analysis

10. Which procurement categories are associated with the highest illustrative exposure?
11. Which sourcing countries represent the largest share of the hypothetical procurement portfolio?
12. Are there sourcing regions where multiple potential disruption signals overlap?

## 6.5 Risk Prioritisation and Investigation

13. Which regions receive the highest scores under the proposed risk assessment framework?
14. What factors contribute most to an individual region's risk score?
15. What supporting evidence is available for each high-priority risk signal?
16. How do risk rankings change when assessment weights or thresholds are adjusted?

## 6.6 Reporting and AI-Assisted Insights

17. Can the platform summarise relevant event information using traceable source evidence?
18. Can users understand why a particular region has been prioritised?
19. Can interactive dashboards help users investigate risk patterns across countries, event types and time periods?

## Expected Analytical Value

Answering these questions should help users move from scattered external information towards structured analysis, explainable risk prioritisation and more informed supply chain investigations.


# 7. Data Requirements and Source Requirements

The platform requires a combination of external disruption data, geographical reference data and illustrative procurement information. These datasets will be used to identify potential risk signals and assess their relevance to the hypothetical procurement portfolio.

## 7.1 Required Data Categories

1. **Geopolitical and News Event Data**
   - Event descriptions and classifications.
   - Event dates and locations.
   - Countries and regions associated with reported events.
   - Source references and available reporting information.

2. **Natural Disaster Data**
   - Earthquake dates, magnitudes, depths and geographical coordinates.
   - Tropical cyclone names, dates, locations and intensity measurements.
   - Historical hazard observations for geographical analysis.

3. **Geographical Reference Data**
   - Country names and standard country codes.
   - Geographic coordinates and regional classifications.
   - Reference information required to match external events with sourcing locations.

4. **Procurement Portfolio Data**
   - Fifteen illustrative sourcing countries.
   - Five hypothetical procurement categories.
   - Synthetic sourcing locations and transport corridors.
   - Illustrative procurement allocation and exposure information.

5. **Historical and Economic Context**
   - Relevant country-level logistics and infrastructure context, where suitable data is available.
   - Historical indicators to support broader country comparisons.

## 7.2 Proposed External Data Sources

The following sources are proposed for the initial development of the platform. Their suitability and technical requirements will be validated before integration.

### 1. GDELT 2.0

**Purpose:** Geopolitical events and news-derived information.

**Potential data:** Event classifications, reporting dates, country references, locations, themes and related news references.

**Planned use:** Identify and analyse reported geopolitical developments and other potentially relevant disruption signals.

**Important limitation:** GDELT is news-derived. Its records may contain duplicates, incomplete information and reporting bias. News coverage does not independently confirm an actual supply chain disruption.

### 2. NOAA IBTrACS

**Purpose:** Global tropical cyclone observations.

**Potential data:** Storm identifiers, names, observation dates, geographical coordinates and available intensity measurements.

**Planned use:** Examine tropical cyclone activity and screen for potential geographical exposure around illustrative sourcing locations.

### 3. USGS Earthquake API

**Purpose:** Earthquake observations.

**Potential data:** Event identifiers, occurrence times, magnitudes, depths and geographical coordinates.

**Planned use:** Identify earthquakes and investigate their geographical proximity to hypothetical sourcing locations.

### 4. World Bank Logistics Performance Index

**Purpose:** Country-level logistics performance context.

**Potential data:** Published logistics performance indicators and available country-level comparisons.

**Planned use:** Provide additional context when comparing sourcing countries.

**Important limitation:** The Logistics Performance Index is a periodically published contextual indicator, not a real-time disruption monitoring source.

## 7.3 Synthetic Procurement Data

A fictional procurement portfolio will be developed to represent the business scenario.

It will include:
- 15 sourcing countries.
- 5 procurement categories.
- Hypothetical sourcing locations.
- Illustrative transport corridors.
- Synthetic procurement allocations and exposure values.

All generated procurement information will be clearly labelled as synthetic. It will not represent actual supplier relationships, company purchases or verified shipment movements.

## 7.4 Data Quality Requirements

Collected data should meet the following requirements wherever the source permits:

1. **Completeness:** Required fields should be available for meaningful analysis.
2. **Accuracy:** Values should be checked against source documentation and validation rules.
3. **Consistency:** Dates, country codes, event categories and geographical formats should be standardised.
4. **Uniqueness:** Duplicate records should be identified and handled appropriately.
5. **Traceability:** Records should retain source identifiers and relevant source references.
6. **Timeliness:** Data collection dates and event occurrence dates should be distinguishable.
7. **Reproducibility:** Data extraction and transformation steps should be documented.

## 7.5 Data Source Validation

Before integrating a source, the project will assess:

- Public availability and access requirements.
- Data structure, schema and supported formats.
- Historical coverage and update frequency.
- Geographic coverage and level of detail.
- Usage restrictions and licensing conditions.
- Suitability for the intended analytical questions.
- Storage and processing requirements within the available budget.

Only sources that meet the project's technical and analytical requirements will be included in the implemented solution.


# 8. Functional and Non-Functional Requirements

## 8.1 Functional Requirements

The platform should provide the following capabilities:

1. **Data Collection:** Retrieve relevant external event and natural hazard information from selected public data sources.

2. **Data Ingestion:** Load collected datasets into Google BigQuery using documented and repeatable ingestion processes.

3. **Data Cleaning:** Identify missing values, duplicates, inconsistent formats and invalid records before analytical use.

4. **Data Transformation:** Standardise event classifications, dates, geographical references and other relevant fields.

5. **Data Integration:** Connect external event information with geographical reference data and the synthetic procurement portfolio.

6. **Exploratory Analysis:** Use SQL and Python to investigate event patterns, historical trends, geographical distributions and potential exposure.

7. **Risk Assessment:** Calculate explainable risk scores using defined assessment factors and documented scoring rules.

8. **Risk Prioritisation:** Classify and rank potential risks to help users identify regions requiring further investigation.

9. **Interactive Reporting:** Provide Power BI dashboards with filters, comparisons, KPIs and supporting event information.

10. **AI-Assisted Investigation:** Generate evidence-grounded event summaries and risk explanations using relevant source information.

11. **Documentation:** Maintain technical documentation covering data sources, architecture, transformations, analytical methods and project decisions.

## 8.2 Non-Functional Requirements

The platform should satisfy the following quality requirements:

1. **Cost Efficiency:** Development and operation should use free-tier services and tools wherever possible, with no planned monthly expenditure.

2. **Performance:** Data processing and analytical queries should be designed to operate efficiently within the available hardware and cloud resources.

3. **Scalability:** The architecture should allow additional countries, data sources and analytical capabilities to be incorporated later.

4. **Reliability:** Data ingestion and transformation processes should include appropriate validation and error handling.

5. **Data Traceability:** Important analytical results should be traceable to their underlying records and original sources wherever available.

6. **Explainability:** Risk scores and classifications should have clearly documented contributing factors and calculation methods.

7. **Usability:** Dashboards and reports should present information in a clear and understandable format for business users.

8. **Maintainability:** Code, SQL queries, documentation and project structure should be organised for future updates.

9. **Responsible AI:** Generative AI outputs should be grounded in available evidence, reviewed for unsupported claims and presented with appropriate limitations.

10. **Data Security:** Public and synthetic datasets should be used, with credentials and access tokens kept out of public repositories.

## 8.3 Technical Environment and Constraints

The initial implementation will be designed around the following environment:

- **Cloud Data Warehouse:** Google BigQuery.
- **Programming Language:** Python.
- **Query Language:** GoogleSQL.
- **Business Intelligence:** Microsoft Power BI.
- **Spreadsheet Analysis:** Microsoft Excel.
- **Version Control:** GitHub.
- **Available Hardware:** 8 GB RAM.
- **Development Budget:** ₹0 planned monthly expenditure.

The implementation will favour cloud-based processing, bounded data extraction and lightweight local development to avoid unnecessary hardware and infrastructure requirements.


# 9. Risk Scoring Methodology

## 9.1 Purpose

The purpose of the risk assessment framework is to evaluate and prioritise potential supply chain exposure by combining relevant external disruption signals with the illustrative procurement portfolio.

The framework will produce an explainable risk score for monitored sourcing regions, helping users understand why certain locations may require further investigation.

## 9.2 Proposed Risk Assessment Factors

The initial framework will consider five assessment factors:

1. **Event Severity — 30%**
   - Evaluates the reported severity or intensity of an identified disruption.
   - Considers available event classifications and hazard measurements.

2. **Geographic Exposure — 25%**
   - Evaluates the geographical relationship between an external event and an illustrative sourcing location.
   - Considers proximity and available location information.

3. **Recency — 20%**
   - Considers how recently the event occurred or was reported.
   - Gives greater consideration to recent disruption signals.

4. **Supporting Evidence — 15%**
   - Considers the availability and quality of supporting information.
   - Distinguishes independent reporting from duplicated or syndicated coverage wherever possible.

5. **Procurement Relevance — 10%**
   - Evaluates the relevance of an event to the illustrative procurement portfolio.
   - Considers sourcing locations and associated procurement categories.

## 9.3 Initial Risk Score

The proposed weighted scoring formula is:

Risk Score =

(Event Severity × 0.30) +

(Geographic Exposure × 0.25) +

(Recency × 0.20) +

(Supporting Evidence × 0.15) +

(Procurement Relevance × 0.10)

Each assessment factor will initially use a normalised score between 0 and 100.

The resulting overall score will also fall between 0 and 100.

## 9.4 Proposed Risk Classification

The initial risk categories will be:

| Risk Score | Classification |
|---|---|
| 0–24 | Low |
| 25–49 | Moderate |
| 50–74 | High |
| 75–100 | Critical |

These thresholds are provisional and will be reviewed during model development and testing.

## 9.5 Risk Assessment Principles

The framework will follow these principles:

- Risk scores must be explainable and traceable to their contributing factors.
- Missing or unreliable information must not automatically be treated as evidence of low risk.
- Duplicate news reports must not be counted as independent corroboration.
- Geographic proximity must be treated as a screening indicator, not proof of direct impact.
- Different event types may require different severity and proximity assessment rules.
- Risk scores should be reviewed for sensitivity to changes in weights and thresholds.

## 9.6 Model Limitations

The proposed framework is a prioritisation model rather than a statistically validated predictive model.

Its scores will not represent:
- The probability of supplier failure.
- The probability of shipment delays.
- Confirmed infrastructure damage.
- Actual financial losses.
- Verified disruption to a real organisation.

The framework will be tested and refined using available data, documented assumptions and sensitivity analysis before being used in the final prototype.

## 9.7 Methodology Status

The weights, scoring rules and classification thresholds defined in this section are initial design assumptions.

They will remain provisional until the underlying datasets, scoring logic and validation results have been examined.


# 10. KPIs and Success Criteria

## 10.1 Data Collection and Quality

The project will evaluate data collection and preparation using the following indicators:

1. **Data Source Integration:** Successfully integrate the selected and validated external data sources.

2. **Data Completeness:** Measure the percentage of records containing the required fields for analysis.

3. **Duplicate Records:** Identify and measure duplicate records before and after data cleaning.

4. **Data Validation:** Track records that pass or fail defined validation checks.

5. **Data Traceability:** Ensure analytical records retain source identifiers or references wherever available.

## 10.2 Analytical Performance

The analytical workflow will be evaluated using:

1. **Event Classification:** Ability to organise external events into meaningful categories.

2. **Geographical Matching:** Ability to associate eligible external events with relevant sourcing locations using documented geographical rules.

3. **Risk Score Calculation:** Ability to calculate consistent scores using the defined assessment methodology.

4. **Risk Explainability:** Ability to show the individual factors contributing to each risk score.

5. **Historical Analysis:** Ability to identify changes and trends in disruption activity over time.

## 10.3 Dashboard and Reporting

The reporting solution should demonstrate:

- Interactive filtering by country, event type and date.
- Clear presentation of risk classifications and trends.
- Visibility into the factors contributing to individual risk scores.
- Access to supporting event information.
- Consistent results between the analytical tables and dashboard measures.

## 10.4 Generative AI Evaluation

The AI component will be evaluated based on:

- Accuracy of event summaries against available source information.
- Consistency between generated explanations and calculated risk scores.
- Ability to reference supporting evidence.
- Frequency of unsupported or fabricated claims.
- Ability to acknowledge missing or insufficient information.

## 10.5 Project Success Criteria

The project will be considered successful when:

1. Selected external datasets have been collected and integrated successfully.
2. A documented data pipeline processes and validates the selected information.
3. SQL and Python analyses answer the defined business questions.
4. The synthetic procurement portfolio is connected to relevant external event information.
5. The risk assessment framework produces explainable and reproducible results.
6. Interactive Power BI dashboards communicate the findings effectively.
7. The Generative AI component demonstrates useful, evidence-grounded capabilities.
8. Testing, limitations and analytical decisions are documented.
9. The complete project is reproducible using the documented setup instructions.

## 10.6 Measurement Approach

Actual KPI values and performance targets will be established during implementation.

The project will record baseline results, validation outcomes and final measurements rather than assume improvements or accuracy figures before testing.


# 11. Assumptions and Constraints

## 11.1 Project Assumptions

The project will operate under the following assumptions:

1. **Public Data Availability:** Relevant external event and natural hazard information will be available through selected public data sources.

2. **Synthetic Procurement Portfolio:** The illustrative procurement portfolio will represent a hypothetical multinational manufacturer rather than an actual business.

3. **Geographical Relevance:** The proximity of an external event to a sourcing location may indicate potential exposure but does not confirm operational impact.

4. **Data Reliability:** External datasets may contain incomplete, inconsistent or duplicated information and will require validation.

5. **Risk Assessment:** The proposed scoring methodology will initially use defined assumptions and will be refined through testing.

6. **AI-Generated Insights:** Generative AI outputs will be treated as analytical assistance and will require evidence-based evaluation.

## 11.2 Technical Constraints

The project must account for the following limitations:

- **Hardware:** Development is restricted to a computer with 8 GB RAM.
- **Budget:** The planned monthly development budget is ₹0.
- **Cloud Resources:** Free-tier services and available public datasets will be prioritised.
- **Data Volume:** Large datasets will be queried or processed using bounded extracts wherever possible.
- **Internet Access:** Data collection and cloud operations depend on an available internet connection.
- **Software Access:** Implementation will depend on available free tools, licenses and service eligibility.

## 11.3 Data and Analytical Constraints

1. **Reporting Bias:** News-derived datasets may overrepresent certain countries, languages or types of events.

2. **Historical Coverage:** Different data sources may provide different historical periods and update frequencies.

3. **Geographical Accuracy:** Event coordinates and location descriptions may be incomplete or imprecise.

4. **Duplicate Reporting:** Multiple records may describe the same underlying event.

5. **Limited Ground Truth:** The synthetic procurement portfolio cannot establish actual supplier or shipment disruption outcomes.

6. **Model Calibration:** The initial risk weights and thresholds will not have proven predictive validity.

7. **AI Limitations:** Generated summaries and explanations may contain unsupported statements and must be checked against source evidence.

## 11.4 Cost and Resource Management

The project will prioritise:

- Free and open-source tools wherever practical.
- BigQuery Sandbox or other verified no-cost options where eligible.
- Efficient SQL queries with appropriate date and partition filters.
- Limited data extraction instead of unnecessary large downloads.
- Lightweight Python processing.
- Manual evaluation where paid AI services are not feasible.

Any service with potential charges will be assessed before use. The project will not assume that a free trial or free tier provides unlimited access.

## 11.5 Risk Management

Potential project risks will be managed through:

- Validating data sources before integration.
- Documenting data limitations and assumptions.
- Monitoring query usage and cloud resource consumption.
- Maintaining source references and processing logs.
- Testing risk calculations against sample cases.
- Reviewing AI-generated outputs for unsupported claims.
- Keeping credentials and sensitive configuration files out of the public repository.


