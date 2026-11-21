
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
