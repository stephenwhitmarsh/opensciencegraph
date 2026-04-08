---
{"dg-publish":true,"permalink":"/02-standards/icd-10/","tags":["icm/uses"],"dg-note-properties":{"name":"International Classification of Diseases, 10th Revision","aliases":["ICD-10","CIM-10","International Classification of Diseases"],"website":"https://www.who.int/classifications/icd","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":1994,"parent_org":"World Health Organization (WHO)","tags":["icm/uses"],"icon":"https://www.who.int/images/default-source/infographics/who-emblem.png"}}
---


# ICD-10 / CIM-10 — International Classification of Diseases, 10th Revision

## Overview
ICD-10 is the WHO standard classification of diseases, health conditions, and causes of death, used worldwide for clinical coding, epidemiology, and health statistics. The French translation **CIM-10** (Classification Internationale des Maladies, 10e révision) is the coding system used in all French national health data systems — making it the primary disease terminology in the [[04_Governance/Health Data Hub\|Health Data Hub]] SNDS and all [[04_Governance/AP-HP\|AP-HP]] hospital billing data. Any cohort built from French health data will use CIM-10 codes.

## Key Neurological Codes
| Code range | Domain |
|---|---|
| G00–G99 | Diseases of the nervous system |
| G20 | Parkinson's disease |
| G30 | Alzheimer's disease |
| G35 | Multiple sclerosis |
| G40 | Epilepsy |
| F00–F99 | Mental and behavioural disorders |
| G10–G13 | Hereditary and degenerative diseases of the nervous system |

## French Health System Context
- **SNDS** (Système National des Données de Santé) at [[04_Governance/Health Data Hub\|Health Data Hub]] uses CIM-10 for all diagnostic coding
- **PMSI** (Programme de Médicalisation des Systèmes d'Information) — French hospital activity coding uses CIM-10
- **[[04_Governance/AP-HP\|AP-HP]] billing data** — all hospital discharge summaries coded in CIM-10
- The transition to [[02_Standards/ICD-11\|ICD-11]] is underway but CIM-10 remains the operational standard in France

## Relationship to Other Terminologies
- **[[02_Standards/SNOMED CT\|SNOMED CT]]** — more granular clinical terminology; ICD-10 is used for billing/admin, SNOMED for clinical detail
- **[[02_Standards/MONDO\|MONDO]]** — disease ontology that harmonises ICD-10 with research databases (OMIM, ORDO)
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — maps CIM-10/ICD-10 codes to standard OMOP concepts via OHDSI Athena vocabulary
- **[[02_Standards/HL7 FHIR\|HL7 FHIR]]** — uses ICD-10 as a standard coding system for Condition resources

## Connections
- Used in: [[04_Governance/Health Data Hub\|Health Data Hub]] (SNDS), [[04_Governance/AP-HP\|AP-HP]] (PMSI billing), [[02_Standards/OMOP CDM\|OMOP CDM]] (source vocabulary)
- Maps to: [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]] (for rare diseases), [[02_Standards/ICD-11\|ICD-11]] (successor)
- Related terminologies: [[02_Standards/CCAM\|CCAM]] (procedures), [[02_Standards/LOINC\|LOINC]] (labs), [[02_Standards/MedDRA\|MedDRA]] (adverse events)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (any study using French health data)

## Resources
- https://www.who.int/classifications/icd
- https://www.atih.sante.fr/la-classification-cim (French ATIH CIM-10 reference)
- https://athena.ohdsi.org (OMOP CDM ICD-10 vocabulary browser)
