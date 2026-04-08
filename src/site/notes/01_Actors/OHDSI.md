---
{"dg-publish":true,"permalink":"/01-actors/ohdsi/","dg-note-properties":{"name":"Observational Health Data Sciences and Informatics","aliases":["OHDSI"],"website":"https://ohdsi.org","type":"consortium","scope":"international","domain":["clinical","health"],"status":"active","founded":2014,"parent_org":"Columbia University (coordinating)"}}
---


# OHDSI — Observational Health Data Sciences and Informatics

## Overview
OHDSI (pronounced "Odyssey") is an international, open-science collaborative established in 2014 that generates evidence from observational health data through transparent, reproducible, and multi-database analytics. OHDSI maintains the [[02_Standards/OMOP CDM\|OMOP CDM]] standard, develops the open-source tools that run on it, and coordinates a global network of 500+ data partners covering 700M+ patient records in 30+ countries — enabling large-scale pharmacoepidemiological and outcomes research that no single institution could conduct alone.

While [[02_Standards/OMOP CDM\|OMOP CDM]] is the *standard*, OHDSI is the *community and network* that makes it operationally useful.

## What OHDSI Produces

### Open-Source Tools
OHDSI develops and maintains the **HADES** (Health Analytics Data-to-Evidence Suite) — a collection of R packages for observational research on OMOP CDM data:

| Tool | Purpose |
|---|---|
| **ATLAS** | Web-based cohort definition, characterisation, incidence rates, population-level estimation; no-code interface |
| **ACHILLES** | Automated data quality and characterisation; generates 170+ statistics on CDM contents |
| **CohortDiagnostics** | Diagnose phenotype algorithms across databases |
| **FeatureExtraction** | Extract covariates for patient-level prediction and estimation |
| **PatientLevelPrediction** | Train and validate ML models for clinical outcomes |
| **CohortMethod** | Population-level effect estimation (comparative cohort studies) |
| **SelfControlledCaseSeries** | Self-controlled case series analysis |
| **Cyclops** | Large-scale regression engine (L1/L2 regularised) |
| **DataQualityDashboard** | Systematic data quality assessment against the Kahn framework |
| **White Rabbit** | Source data profiling for ETL design |
| **Rabbit in a Hat** | Visual ETL mapping tool |

### Network Studies
OHDSI coordinates multi-database **network studies** — analytical studies that run identical code across all participating databases, generating site-level results that are meta-analysed centrally:
- The **OHDSI COVID-19 Studies** (2020) characterised 34,000+ hospitalised patients across 34 databases in 13 countries within 3 weeks of the pandemic
- **LEGEND-T2DM** — comparative safety of second-line type 2 diabetes treatments across 11 databases and 1.5M patients
- Neurological disease network studies on dementia, epilepsy, and Parkinson's disease incidence and treatment patterns

### Phenotype Library
OHDSI maintains an open **Phenotype Library** of validated ATLAS cohort definitions for hundreds of clinical conditions, enabling researchers to reuse rigorously validated phenotype algorithms for disease cohorts.

## OHDSI in France
- [[04_Governance/Health Data Hub\|Health Data Hub]] — all SNDS data in the HDH Datalab is OMOP CDM v5.4; ATLAS is the primary analytical interface for HDH users
- [[04_Governance/AP-HP\|AP-HP]] EDS — OMOP CDM-based; ATLAS and ACHILLES deployed
- French OHDSI community — active participation in OHDSI Europe annual symposia

## Connections
- Maintains: [[02_Standards/OMOP CDM\|OMOP CDM]] (the standard)
- Adopted by: [[04_Governance/Health Data Hub\|Health Data Hub]], [[04_Governance/AP-HP\|AP-HP]], [[04_Governance/ECRIN\|ECRIN]], [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]]
- Tools: ATLAS, ACHILLES, HADES R packages, DataQualityDashboard
- Vocabularies (via Athena): [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/MedDRA\|MedDRA]], [[02_Standards/RxNorm\|RxNorm]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]]
- Mandated by: [[04_Governance/EHDS\|EHDS]] (OMOP CDM for secondary use)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (AP-HP EDS access via ATLAS; Health Data Hub neurological disease cohort studies; OMOP CDM phenotyping for research)

## Resources
- https://ohdsi.org
- https://ohdsi.github.io/Hades/ (HADES R packages documentation)
- https://atlas-demo.ohdsi.org (ATLAS public demo instance)
- https://athena.ohdsi.org (Athena — OMOP vocabulary browser)
- https://www.ohdsi.org/data-standardization/ (CDM and tools overview)
