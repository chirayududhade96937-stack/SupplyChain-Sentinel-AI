
# SupplyChain Sentinel AI
### Global Supply Chain Risk Intelligence & Decision Support Platform

## About the Project

Global supply chains are connected to events happening all around the world. A natural disaster, geopolitical conflict or disruption at an important transport hub can create problems for businesses that depend on international sourcing. The challenge is that information about these events often comes from different sources, making it difficult to understand the bigger picture.

I started SupplyChain Sentinel AI to explore how data analytics and AI can help make sense of these scattered signals. The idea is to bring information from different sources into one place, analyse what is happening and identify sourcing regions that may need closer attention.

Rather than simply displaying large amounts of data, I want to build something that helps users understand why a region has been flagged, what events may be contributing to the risk and where further investigation might be needed.

## The Problem I'm Trying to Solve

There are a few challenges I want this project to address:

- **Scattered information:** News reports, natural disaster records and other disruption data are available across different platforms and formats.
- **Too much information:** Not every reported event represents a genuine supply chain risk. Understanding which signals matter is just as important as collecting them.
- **Limited visibility:** It can be difficult to connect global events with specific sourcing regions and procurement activities.
- **Unclear risk assessments:** A risk score is only useful when people can understand how it was calculated and what information supports it.

To explore these challenges, I'll use real-world external data alongside an illustrative procurement portfolio consisting of 15 sourcing countries, 5 procurement categories and hypothetical sourcing locations and transport corridors.

The procurement information will be simulated for demonstration purposes. Risk scores will be used to prioritise further investigation, not to predict supplier failures, shipment delays or financial losses.

## How I Plan to Build It

The project will follow an end-to-end analytics workflow.

**1. Data Collection & Validation — Python and BigQuery**

Collect information from public data sources such as GDELT, NOAA IBTrACS and USGS. Check the data, understand its structure and make sure the information can be traced back to its original source.

**2. Data Processing & Analysis — SQL and Python**

Organise the data using Bronze, Silver and Gold layers. Clean and transform records, handle duplicates, connect relevant events with sourcing locations and explore geographical relationships.

**3. Risk Assessment**

Develop an explainable risk-scoring approach using factors such as event severity, geographical exposure, recency, corroborating reports and procurement relevance. Test the scoring method and understand its limitations.

**4. Analysis & Visualisation — Excel and Power BI**

Use Excel for data checks, comparisons and scenario analysis. Build an interactive Power BI dashboard to explore global risks, geopolitical events, natural hazards and potential procurement exposure.

**5. Generative AI Integration**

Explore how AI can help summarise events, explain risk assessments and make information easier to understand. Any AI-generated explanation will need to be grounded in available evidence and checked for unsupported claims.

## Technology Stack

| Technology | Planned Use |
|---|---|
| Google BigQuery | Cloud data storage and processing |
| SQL | Data exploration, cleaning and analysis |
| Python | Data collection, validation and geospatial analysis |
| Microsoft Excel | Data checks and supporting analysis |
| Power BI | Interactive dashboards and reporting |
| Generative AI | Event summaries and risk explanations |
| GitHub | Code, documentation and project tracking |

## Data Sources

The project will explore the following sources:

- **GDELT 2.0:** Global news and event information.
- **NOAA IBTrACS:** Historical and current tropical cyclone track observations.
- **USGS:** Earthquake information and event records.
- **World Bank LPI:** Logistics performance and country-level context, if suitable for the analysis.

Each source will be researched and checked before being included in the final workflow.

## What I Want to Achieve

My goal is to build a working platform that brings different sources of information together and turns them into something useful for business decision-making.

By the end of the project, I want users to be able to explore global disruption events, compare potentially exposed sourcing regions, understand why certain risks have been highlighted and investigate the evidence behind them.

More importantly, I want to build and understand the complete process myself, from collecting raw data to presenting meaningful business insights.

## Scope & Limitations

- **Illustrative procurement data:** Supplier relationships, sourcing locations and transport corridors will be hypothetical.
- **Real-world observations:** External event and hazard information will come from genuine public data sources.
- **Risk prioritisation, not prediction:** A nearby event does not automatically mean a supplier or shipment is affected.
- **Source limitations:** News coverage can be incomplete, duplicated or biased. Multiple reports do not necessarily represent independent confirmation.
- **Resource constraints:** The project will be developed with a zero-monthly-budget approach and an available 8 GB RAM system, prioritising free tools and cloud-based processing.

## Current Status

The project is currently in its planning and GitHub setup stage. The next focus is formalising the requirements, researching the data sources and designing the system architecture.

For ongoing updates, see [PROJECT_PROGRESS.md](PROJECT_PROGRESS.md).

---

*Built as a hands-on business analytics project, with each stage documented as I learn, develop and improve the solution.*
