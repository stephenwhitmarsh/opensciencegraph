---
{"dg-publish":true,"permalink":"/standards/loinc/","tags":["icm/uses"],"dg-note-properties":{"name":"Logical Observation Identifiers Names and Codes","aliases":["LOINC"],"website":"https://loinc.org","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":1994,"parent_org":"Regenstrief Institute","tags":["icm/uses"],"icon":"https://loinc.org/favicon.ico"}}
---


# LOINC — Logical Observation Identifiers Names and Codes

## Overview
LOINC is the universal standard for identifying medical laboratory tests, clinical observations, outcomes measures, imaging studies, and clinical documents. Developed by the Regenstrief Institute (Indiana University), LOINC provides a common language for exchanging clinical results between systems — meaning a serum amyloid-beta measurement at Pitié-Salpêtrière can be unambiguously identified and compared with one from any other institution worldwide. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], LOINC is the key standard for coding biomarker data (CSF amyloid, tau, NfL), imaging reports, and clinical assessment scales.

## Key Uses for ICM
- **CSF and blood biomarkers** — amyloid-β 42/40, phospho-tau 181, NfL (neurofilament light chain) used in Alzheimer's and neurodegeneration research
- **Imaging reports** — MRI and PET report coding
- **Clinical scales** — MMSE (Mini-Mental State Examination), MoCA (Montreal Cognitive Assessment), UPDRS (Parkinson's rating scale)
- **Lab panels** — standard blood work in clinical cohorts

## Selected Neuroscience LOINC Codes
| LOINC Code | Description |
|---|---|
| 71585-7 | Amyloid beta 42/40 ratio [Moles/volume] in CSF |
| 33203-0 | Tau protein [Mass/volume] in CSF |
| 72153-3 | Phospho-tau 181 [Mass/volume] in CSF |
| 99771-2 | Neurofilament light chain [Mass/volume] in Serum |
| 11523-5 | EEG study |
| 36643-5 | Brain MRI |
| 72106-1 | MMSE total score |

## Integration in the Data Ecosystem
- **[[Standards/OMOP CDM\|OMOP CDM]]** — LOINC is one of the core standard vocabularies for measurement and observation concepts; AP-HP EDS uses LOINC extensively
- **[[Standards/HL7 FHIR\|HL7 FHIR]]** — Observation resources use LOINC as the primary coding system
- **[[Governance/Health Data Hub\|Health Data Hub]]** — LOINC codes present in SNDS lab data
- **[[Governance/AP-HP\|AP-HP]]** — EDS AP-HP maps hospital lab results to LOINC

## Connections
- Integrated into: [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]], [[Governance/AP-HP\|AP-HP]], [[Governance/Health Data Hub\|Health Data Hub]]
- Complements: [[Standards/SNOMED CT\|SNOMED CT]] (procedures and findings), [[Standards/ICD-10\|ICD-10]] (diagnoses), [[Standards/CCAM\|CCAM]] (French procedures)
- Used with: [[Standards/openEHR\|openEHR]] (archetypes reference LOINC codes)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (biomarker studies, clinical cohorts)

## Resources
- https://loinc.org
- https://loinc.org/search/ (LOINC search interface)
- https://athena.ohdsi.org (OMOP CDM LOINC vocabulary browser)
