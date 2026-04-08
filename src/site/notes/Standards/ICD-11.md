---
{"dg-publish":true,"permalink":"/standards/icd-11/","dg-note-properties":{"name":"International Classification of Diseases, 11th Revision","aliases":["ICD-11"],"website":"https://icd.who.int/en","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":2022,"parent_org":"World Health Organization (WHO)"}}
---


# ICD-11 — International Classification of Diseases, 11th Revision

## Overview
ICD-11 is the WHO's updated disease classification, officially endorsed in 2019 and in effect from 1 January 2022. It replaces [[Standards/ICD-10\|ICD-10]] with a fully digital, ontology-aligned structure featuring a foundation layer (all concepts) and linearisations (context-specific views including morbidity and mortality). France is in transition toward ICD-11 adoption. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], ICD-11 brings significant improvements for neuroscience: richer coverage of neurodegenerative diseases, movement disorders, and rare neurological conditions.

## Key Improvements over ICD-10 for Neuroscience
- **Chapter 8** (Diseases of the nervous system) is substantially expanded and restructured with better specificity for Parkinson's disease and parkinsonisms (detailed subtypes), Alzheimer's disease stages, rare neurodegenerative diseases, epilepsy (aligned with ILAE classification), and neuromuscular diseases
- **Chapter 6** (Mental, behavioural, or neurodevelopmental disorders) — revised taxonomy aligned with DSM-5 and current neuroscience evidence
- Digital-first: each concept has a stable URI and is linked to SNOMED CT
- **Postcoordination** — allows combining codes to express complex conditions
- Full **SNOMED CT mapping** — official cross-map between ICD-11 and SNOMED CT

## French Adoption Timeline
France has committed to ICD-11 adoption. The transition is coordinated by the **ATIH** (Agence Technique de l'Information sur l'Hospitalisation). CIM-11 (the French translation) will progressively replace CIM-10 in PMSI, SNDS, and AP-HP systems. [[Governance/Health Data Hub\|Health Data Hub]] and [[Governance/AP-HP\|AP-HP]] datasets will carry both codes during the transition period.

## Connections
- Successor to: [[Standards/ICD-10\|ICD-10]] (replaces CIM-10 in French health systems)
- Official mapping: [[Standards/SNOMED CT\|SNOMED CT]] ↔ ICD-11 (WHO-maintained cross-map)
- Harmonised by: [[Standards/MONDO\|MONDO]] (integrates ICD-11 into unified disease ontology)
- Used in: [[Standards/OMOP CDM\|OMOP CDM]] (ICD-11 vocabulary being integrated in Athena)
- Relevant to: [[Governance/Health Data Hub\|Health Data Hub]], [[Governance/AP-HP\|AP-HP]], [[Actors/Paris Brain Institute\|Paris Brain Institute]]

## Resources
- https://icd.who.int/en (WHO ICD-11 browser)
- https://icd.who.int/browse/2024-01/mms/en (Mortality and Morbidity Statistics)
- https://www.atih.sante.fr (French ATIH — CIM adoption coordination)
