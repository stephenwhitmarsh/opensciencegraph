---
{"dg-publish":true,"permalink":"/standards/open-ehr/","dg-note-properties":{"name":"openEHR","aliases":["openEHR Foundation","openEHR specification"],"website":"https://openehr.org","type":"standard","scope":"international","domain":["clinical","health"],"status":"active","founded":1999,"parent_org":"openEHR Foundation"}}
---


# openEHR

## Overview
openEHR is an open specification for electronic health records that separates clinical knowledge (expressed as **archetypes** and **templates**) from the underlying technical infrastructure, enabling vendor-neutral, semantically rich EHR systems. Its key innovation is that clinical concepts — a neurological examination, a medication prescription, a seizure event — are defined once as archetypes in a shared repository (CKM, Clinical Knowledge Manager) and then reused across any openEHR-compliant system. This makes it highly suitable for clinical neuroscience research where structured, reusable phenotype data is essential. openEHR integrates bidirectionally with [[Standards/HL7 FHIR\|HL7 FHIR]] and is used in national EHR rollouts in several European countries.

## Key Concepts
- **Archetypes** — reusable clinical concept definitions (e.g. "Blood Pressure", "Neurological Examination Finding") in a formal, queryable format
- **Templates** — combinations of archetypes for specific use cases (e.g. ICU admission form, epilepsy clinic note)
- **AQL** (Archetype Query Language) — SQL-like query language for openEHR data
- **CKM** (Clinical Knowledge Manager) — international archetype library

## Neuroscience Relevance
The AP-HP ecosystem and French health informatics community use openEHR archetypes for structured clinical data capture. For ICM, openEHR is relevant as the semantic EHR layer that feeds into [[Standards/OMOP CDM\|OMOP CDM]] and [[Standards/HL7 FHIR\|HL7 FHIR]] for research purposes. Neurological archetypes exist for seizures, cognitive assessments, motor function, and more.

## Connections
- Maps to: [[Standards/HL7 FHIR\|HL7 FHIR]] (bidirectional mapping supported)
- Maps to: [[Standards/SNOMED CT\|SNOMED CT]] (archetypes use SNOMED CT terms)
- Maps to: [[Standards/OMOP CDM\|OMOP CDM]] (ETL pipeline from openEHR to OMOP)
- Relevant context: [[Governance/AP-HP\|AP-HP]] informatics ecosystem, [[Governance/Health Data Hub\|Health Data Hub]]
- Related standards: [[Standards/CDISC\|CDISC]] (clinical trials), [[Standards/OMOP CDM\|OMOP CDM]] (observational)

## Resources
- https://openehr.org
- https://ckm.openehr.org (Clinical Knowledge Manager — archetype library)
