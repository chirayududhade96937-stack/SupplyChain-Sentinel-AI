
# Phase 2: Data Source Research and Validation

**Project:** SupplyChain Sentinel AI  
**Phase:** 2 — Data Source Research and Validation  
**Research period:** November 2026  
**Primary GDELT investigation period:** October 1–31, 2026  
**Status:** Research assessment completed; outstanding empirical validations documented

---

## 1. Purpose

The purpose of Phase 2 was to investigate, assess and validate the external data sources required for SupplyChain Sentinel AI.

The research focused on understanding:

- Data availability and structure.
- Relevant fields and attributes.
- Data completeness and quality.
- Geographic and temporal characteristics.
- Potential anomalies and extraction limitations.
- Suitability for supply-chain risk intelligence.
- Engineering requirements for future data ingestion and transformation.

The objective was to establish whether the selected sources could support a global supply-chain risk intelligence and decision-support platform.

## 2. Research Scope

The investigation covered the following sources:

| Data source | Primary purpose | Research status |
|---|---|---|
| GDELT Events | Geopolitical event intelligence | Investigated |
| GDELT EventMentions | News mention and supporting evidence | Investigated |
| GDELT GKG | Themes, locations and extracted entities | Investigated |
| NOAA IBTrACS | Tropical cyclone observations | Documentation-based assessment |
| USGS Earthquake Catalog | Earthquake observations | Documentation-based assessment |
| World Bank LPI | Background logistics performance context | Optional source assessment |

The GDELT investigation used the public BigQuery dataset:

`gdelt-bq.gdeltv2`

The three partitioned tables investigated were:

- `events_partitioned`
- `eventmentions_partitioned`
- `gkg_partitioned`

October 2026 was used as the principal investigation period for detailed GDELT data-quality and structural analysis.

## 3. GDELT Events

### Purpose

The Events dataset provides structured records of reported events involving people, organisations and countries.

It offers information about event classifications, actors, geographic locations, dates and source reporting activity.

### Research findings

The investigation established that:

- EventCode provides a structured classification based on the CAMEO event taxonomy.
- QuadClass groups events into verbal cooperation, material cooperation, verbal conflict and material conflict.
- GoldsteinScale represents the theoretical potential impact of an event type on political stability.
- AvgTone represents document or event-related tone and should not be treated as event severity.
- ActionGeo fields provide geographic attribution, but individual records may contain misleading or incorrect classifications.
- NumMentions, NumSources and NumArticles describe reporting activity rather than independently verified evidence.
- Historical partitions contain unusual date and coverage patterns that require caution when interpreting long-term trends.

October 2026 contained approximately 5.13 million event records.

Structural checks found no missing event identifiers, event codes or SQLDATE values in the investigated October records.

### Engineering implications

- Preserve original event codes and geographic attributes.
- Maintain a controlled event-category mapping.
- Validate potentially relevant event classifications against contextual evidence.
- Do not interpret reporting volume as confirmed disruption severity.
- Preserve original source URLs for traceability.
- Treat event records as intelligence signals rather than verified real-world incidents.

## 4. GDELT EventMentions

### Purpose

The EventMentions dataset provides information about the news documents and extracted mentions associated with GDELT events.

It supports evidence investigation, source traceability and reporting analysis.

### Research findings

The October 2026 investigation identified:

- Approximately 12.38 million mention records.
- Approximately 5.16 million distinct event identifiers.
- 14,145 distinct source names.
- Approximately 2.75 million distinct URLs.
- Repeated URLs and multiple mentions associated with the same documents.
- Different recording timestamps and extraction-confidence values.
- Translation metadata and document-level tone information.

The investigation established important distinctions:

**EventTimeDate:** Represents when GDELT first recorded the event.

**MentionTimeDate:** Represents the GDELT update time when a mention was recorded.

The difference between these timestamps must not be interpreted as the actual delay between a real-world event and news publication.

Confidence represents confidence in the event extraction process, not whether the reported event is true.

InRawText distinguishes mentions identified directly in the original text from those requiring additional NLP processing.

### Engineering implications

- Preserve mention-level records separately from event-level records.
- Retain original source URLs and publisher information.
- Avoid treating repeated URLs as independent corroboration.
- Preserve extraction confidence and translation metadata.
- Avoid treating document tone as event severity.
- Retain raw character offsets and flag questionable values rather than automatically discarding them.

## 5. GDELT GKG

### Purpose

The Global Knowledge Graph provides contextual information extracted from news documents.

It contains themes, locations, people, organisations, tone, counts, dates, amounts, quotations and document metadata.

### Research findings

The October 2026 investigation covered:

- Record identifiers and document identity.
- V2Themes.
- V2Locations.
- V2Persons and V2Organizations.
- Legacy Persons and Organizations fields.
- V2Tone and GCAM.
- Counts and V2Counts.
- Dates and Amounts.
- AllNames and Quotations.
- TranslationInfo and Extras.
- SharingImage, RelatedImages, SocialImageEmbeds and SocialVideoEmbeds.

The investigation identified several important data characteristics:

1. GKG record identifiers showed repeated values associated with different documents and publishers. Record identifiers must not automatically be assumed unique.
2. V2Locations contains geographic classifications and feature identifiers, but its country and administrative codes require appropriate geographic reference mapping.
3. GKG geographic names may contain aliases and alternative spellings.
4. Themes provide contextual signals but do not independently establish that a supply-chain disruption occurred.
5. Person and organisation extraction can contain false positives and repeated mentions.
6. V2Tone represents document-level tone, not event severity.
7. Counts and V2Counts contain structured information requiring component-level parsing.
8. Extras contains XML-like metadata fields and was populated throughout the October dataset.
9. Image and video fields may contain publisher or social-media references that do not independently establish an event's authenticity.

### Engineering implications

- Preserve raw GKG records.
- Separate source-record identity from document identity.
- Retain geographic feature identifiers and original location names.
- Use themes and entities as supporting contextual intelligence.
- Apply field-specific parsing and validation.
- Preserve translation and document metadata.
- Flag malformed or unexpected structures rather than silently removing records.
- Avoid treating images, quotations or extracted entities as independently verified evidence.

### Additional validation observations

The earlier 10,000-row sample identified 385 numeric anomalies in both Counts and V2Counts. These anomalies have not yet been individually inspected.

The Dates field passed preliminary numeric and structural checks in the sample, but its observed format did not fully align with the documented structure.

Extras was populated throughout the October dataset, which differs from older descriptions of its historical use.

The initial sample was selected using LIMIT without ORDER BY. It should therefore be treated as a diagnostic sample rather than a reproducible random or statistically representative sample.

A preliminary validation rule was also corrected after it was found to incorrectly apply the name-and-character-offset structure to the legacy Persons and Organizations fields. These fields must be distinguished from V2Persons and V2Organizations.

## 6. NOAA IBTrACS

### Purpose

The International Best Track Archive for Climate Stewardship provides historical tropical cyclone observations.

It is intended to support natural-hazard intelligence and geographic exposure assessment.

### Expected useful information

- Storm identifier and name.
- Observation timestamp.
- Latitude and longitude.
- Wind speed.
- Atmospheric pressure.
- Storm classification and basin.
- Reporting agency.

### Research assessment

IBTrACS is a suitable candidate for global tropical cyclone observations.

However, agency-specific measurement conventions, historical coverage and observation intervals must be considered.

Wind-speed measurements from different agencies should not automatically be treated as directly comparable.

A storm track near a sourcing location indicates potential geographic exposure, not confirmed damage or operational disruption.

**Validation limitation:** An empirical dataset sample and field-level quality assessment remain outstanding.

Official source: https://www.ncei.noaa.gov/products/international-best-track-archive

## 7. USGS Earthquake Catalog

### Purpose

The USGS Earthquake Catalog provides structured earthquake observations and geographic information.

It is intended to support earthquake-related natural-hazard intelligence.

### Expected useful information

- Earthquake event identifier.
- Origin timestamp.
- Magnitude and magnitude type.
- Latitude and longitude.
- Depth.
- Geographic place description.
- Updated timestamp and review status.

### Research assessment

The USGS Earthquake Catalog is suitable for obtaining structured earthquake observations.

Magnitude types, event revisions, geographic coverage and reporting thresholds must be considered during ingestion and analysis.

Earthquake proximity alone does not establish infrastructure damage or supply-chain disruption.

**Validation limitation:** An empirical API response sample and field-level quality assessment remain outstanding.

Official source: https://earthquake.usgs.gov/fdsnws/event/1/

## 8. World Bank Logistics Performance Index

### Purpose

The Logistics Performance Index can provide background information about national logistics capabilities and trade-related performance.

### Research assessment

The LPI may provide useful contextual information when comparing sourcing-country environments.

However, it is not a real-time disruption monitoring source.

Its reporting periods and indicator availability must be considered before incorporating it into the platform.

It remains an optional contextual source rather than a primary operational risk signal.

Official source: https://lpi.worldbank.org/

## 9. Overall Data Source Assessment

The research indicates that the selected primary sources provide complementary information:

| Source | Intelligence provided | Intended use |
|---|---|---|
| GDELT Events | Reported geopolitical events | Event discovery and classification |
| GDELT EventMentions | News-source mentions | Supporting evidence and provenance |
| GDELT GKG | Themes, locations and entities | Contextual enrichment |
| NOAA IBTrACS | Tropical cyclone observations | Natural-hazard exposure |
| USGS | Earthquake observations | Natural-hazard exposure |
| World Bank LPI | National logistics context | Optional background enrichment |

No individual source provides complete confirmation of supply-chain disruption.

The platform must combine relevant observations with synthetic procurement exposure information and clearly distinguish reported intelligence from confirmed operational impact.

## 10. Cross-Source Limitations

The following limitations will influence the design of the platform:

- News coverage is uneven across countries and languages.
- Multiple reports may refer to the same underlying incident.
- GDELT extraction can contain incorrect classifications and entity matches.
- Geographic proximity does not prove physical damage.
- Event severity cannot be inferred directly from document tone or reporting volume.
- Natural-hazard datasets do not establish the impact on a specific supplier, port or shipment.
- Historical source coverage and update behaviour can vary.
- Missing or malformed information must not silently become a zero-risk assessment.

## 11. Phase 2 Research Outcome

The research established that the selected data sources are suitable candidates for a global supply-chain risk intelligence and decision-support platform, subject to appropriate ingestion, validation, standardisation and contextual interpretation.

GDELT provides the primary geopolitical and news-derived intelligence layer.

NOAA IBTrACS and USGS provide complementary natural-hazard observations.

The procurement exposure dataset will be synthetic and will be used to demonstrate how external intelligence can be related to hypothetical sourcing locations and procurement categories.

The platform will identify and prioritise potential risks for investigation. It will not claim to predict supplier failure, shipment delays, confirmed infrastructure damage or financial losses.

## 12. Outstanding Validation Items

The following limitations must remain visible in subsequent development:

| Item | Outstanding work |
|---|---|
| Counts and V2Counts | Inspect the 385 numeric anomalies identified in the earlier sample |
| Dates | Resolve the observed format discrepancy against the documented structure |
| NOAA IBTrACS | Perform an empirical sample and field-level validation |
| USGS | Perform an empirical API sample and field-level validation |
| Risk model | Conduct sensitivity testing and assess proposed scoring weights |
| Geographic mapping | Validate geographic reference mappings during transformation |

These outstanding items do not invalidate the research assessment. They must be addressed or explicitly carried as limitations before the relevant fields or calculations are used in production-style processing.

---

## 13. Phase 2 Conclusion

Source research and preliminary validation have been consolidated.

The findings provide the basis for subsequent engineering design, with outstanding empirical checks documented as limitations rather than treated as completed tests.

Phase 2 is considered complete at the research-assessment level. Outstanding empirical validations will be carried forward as explicit requirements for the relevant implementation stages.

