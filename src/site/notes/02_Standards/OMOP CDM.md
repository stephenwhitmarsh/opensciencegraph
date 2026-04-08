---
{"dg-publish":true,"permalink":"/02-standards/omop-cdm/","tags":["icm/uses"],"dg-note-properties":{"name":"Observational Medical Outcomes Partnership Common Data Model","aliases":["OMOP CDM","OMOP"],"website":"https://ohdsi.org/omop/","type":"standard","scope":"international","domain":["clinical","health"],"status":"active","founded":2009,"parent_org":"OHDSI","tags":["icm/uses"],"icon":"https://ohdsi.org/wp-content/uploads/2023/02/OHDSI_logo_flat.png"}}
---


# OMOP CDM — Observational Medical Outcomes Partnership Common Data Model

## Overview
The OMOP Common Data Model (CDM) is the open standard for structuring observational health data — EHR records, insurance claims, registries — into a common format that enables federated analytical studies across institutions without sharing raw patient data. Developed within the OMOP initiative (funded by the FDA) and now maintained by the **OHDSI** (Observational Health Data Sciences and Informatics) open-science community, the OMOP CDM is deployed in 300+ databases covering 700 million+ patient records across 30+ countries.

In France, [[04_Governance/Health Data Hub\|Health Data Hub]] and [[04_Governance/AP-HP\|AP-HP]] have adopted OMOP CDM as the standard for their health data warehouses, making it the primary analytical framework for clinical research using French health data. All data accessible via the Health Data Hub Datalab is standardised to OMOP CDM version 5.4.

## CDM Structure
The OMOP CDM organises clinical data into standardised **domain tables**:

| Domain | Table | Contents |
|---|---|---|
| **Person** | PERSON | Demographics; one row per patient |
| **Observation Period** | OBSERVATION_PERIOD | Periods of clinical data availability |
| **Visit** | VISIT_OCCURRENCE | Hospital stays, outpatient visits, ED |
| **Condition** | CONDITION_OCCURRENCE | Diagnoses (coded to [[02_Standards/SNOMED CT\|SNOMED CT]]) |
| **Drug** | DRUG_EXPOSURE | Prescriptions, administrations (coded to [[02_Standards/RxNorm\|RxNorm]]) |
| **Procedure** | PROCEDURE_OCCURRENCE | Clinical procedures (coded to [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/CCAM\|CCAM]]) |
| **Measurement** | MEASUREMENT | Lab results, vitals (coded to [[02_Standards/LOINC\|LOINC]]) |
| **Observation** | OBSERVATION | Clinical findings not fitting other domains |
| **Note** | NOTE | Unstructured clinical notes (text) |
| **Death** | DEATH | Date and cause of death |
| **Specimen** | SPECIMEN | Biological samples (linked to biobanks) |

All clinical concepts are mapped to the **OMOP Standard Vocabulary** — a harmonised vocabulary space where source codes ([[02_Standards/ICD-10\|ICD-10]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/MedDRA\|MedDRA]], local codes) are mapped to standard concepts primarily drawn from [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/RxNorm\|RxNorm]], and [[02_Standards/MedDRA\|MedDRA]].

## OHDSI Vocabulary (Athena)
The OMOP vocabulary system is managed via **Athena** (https://athena.ohdsi.org):
- Browse and download all OMOP standard vocabularies
- Map local codes (ICD-10, CCAM, MedDRA, local lab codes) to OMOP standard concepts
- Free, open access; updated regularly
- Vocabularies include: [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/ICD-11\|ICD-11]], [[02_Standards/MedDRA\|MedDRA]], [[02_Standards/RxNorm\|RxNorm]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/MeSH\|MeSH]], [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]], NDC

## OHDSI Tools
The OHDSI community develops open-source analytical tools that run on OMOP CDM:
- **ATLAS** — web-based cohort definition, characterisation, and analysis tool; no coding required; creates reproducible phenotype algorithms
- **ACHILLES** — automated data quality and characterisation: generates statistics on the CDM contents to identify data quality issues
- **HADES** — R package library for epidemiology, population-level estimation, and patient-level prediction on OMOP data
- **White Rabbit / Rabbit in a Hat** — ETL design tools: profile source data and design source-to-CDM mapping

## Federated Network Analysis
OMOP CDM's key innovation is enabling **federated distributed network studies**: each site runs the same analytical code locally on their OMOP database; only aggregate results (counts, summary statistics) are shared — no raw data transfer; enables enormous effective sample sizes (OHDSI network studies routinely include 100M+ patients across 20+ databases); EHDS mandates OMOP CDM for secondary use of European health data under the European Health Data Space regulation.

## OMOP CDM in France
- **[[04_Governance/Health Data Hub\|Health Data Hub]]** — all SNDS data accessible via HDH Datalab is in OMOP CDM v5.4
- **[[04_Governance/AP-HP\|AP-HP]] EDS** — AP-HP's Entrepôt de Données de Santé is OMOP CDM-based; covers 8M+ patients from 39 AP-HP hospitals
- **i2b2 → OMOP migration** — many French hospitals are migrating from [[04_Governance/i2b2\|i2b2]] to OMOP CDM for better international interoperability
- **[[04_Governance/ECRIN\|ECRIN]]** — uses OMOP CDM for observational study data standardisation
- **[[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]]** — promotes OMOP CDM for biobank-linked clinical data

## Connections
- Adopted by: [[04_Governance/Health Data Hub\|Health Data Hub]], [[04_Governance/AP-HP\|AP-HP]], [[04_Governance/ECRIN\|ECRIN]], [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[04_Governance/i2b2\|i2b2]]
- Maps to: [[02_Standards/HL7 FHIR\|HL7 FHIR]] (bidirectional ETL; OMOP-on-FHIR mapping), [[02_Standards/CDISC\|CDISC]] (OMOP↔SDTM mapping for trial data)
- Vocabularies: [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/ICD-11\|ICD-11]], [[02_Standards/MedDRA\|MedDRA]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/RxNorm\|RxNorm]], [[02_Standards/MeSH\|MeSH]], [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]]
- Mandated by: [[04_Governance/EHDS\|EHDS]] (secondary use standardisation for European health data)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (AP-HP EDS clinical data access for neurological disease research; Health Data Hub population neurology studies)

## Resources
- https://ohdsi.org
- https://ohdsi.github.io/CommonDataModel/ (CDM specification)
- https://github.com/OHDSI/CommonDataModel (GitHub)
- https://athena.ohdsi.org (OMOP vocabulary browser and download)
- https://atlas-demo.ohdsi.org (ATLAS demo instance)
