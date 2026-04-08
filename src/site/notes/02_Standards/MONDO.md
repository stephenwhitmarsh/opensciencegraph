---
{"dg-publish":true,"permalink":"/02-standards/mondo/","tags":["icm/uses"],"dg-note-properties":{"name":"Monarch Disease Ontology","aliases":["MONDO","Monarch Disease Ontology"],"website":"https://monarchinitiative.org/disease","type":"terminology","scope":"international","domain":["clinical","genomics"],"status":"active","founded":2018,"parent_org":"Monarch Initiative (EMBL-EBI, Jackson Laboratory, Oregon Health and Science University)","tags":["icm/uses"],"icon":"https://monarchinitiative.org/favicon.ico"}}
---


# MONDO — Monarch Disease Ontology

## Overview
MONDO is an integrated cross-species disease ontology that harmonises major disease classification systems — [[02_Standards/ICD-10\|ICD-10]], ICD-11, OMIM (Mendelian inheritance), [[02_Standards/ORDO\|ORDO]] (Orphanet rare diseases), DOID (Disease Ontology), and others — into a single coherent hierarchy. Developed by the Monarch Initiative, MONDO is the single best ontology for **cross-database disease queries** because it provides a unified identifier (e.g. MONDO:0004975 for Alzheimer's disease) that maps to the corresponding codes in every major system. For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], MONDO is the key bridge between the [[02_Standards/ICD-10\|ICD-10]] / CIM-10 coding used in French health data ([[04_Governance/Health Data Hub\|Health Data Hub]], [[04_Governance/AP-HP\|AP-HP]]) and the research disease databases (OMIM, [[02_Standards/ORDO\|ORDO]]) used in genomics and rare disease research.

## Key Mappings for ICM Research Areas
| Disease | MONDO ID | Maps to |
|---|---|---|
| Alzheimer's disease | MONDO:0004975 | ICD-10 G30, OMIM 104300, ORDO:26929 |
| Parkinson's disease | MONDO:0005180 | ICD-10 G20, OMIM 168600, ORDO:411 |
| Multiple sclerosis | MONDO:0005301 | ICD-10 G35, OMIM 126200, ORDO:802 |
| Amyotrophic lateral sclerosis | MONDO:0004976 | ICD-10 G12.2, OMIM 105400, ORDO:803 |
| Huntington's disease | MONDO:0007739 | ICD-10 G10, OMIM 143100, ORDO:399 |

## Harmonisation Role
MONDO is part of the OBO Foundry ecosystem and is maintained in close alignment with:
- **[[02_Standards/HPO\|HPO]]** — phenotype descriptions linked to MONDO disease concepts
- **[[02_Standards/ORDO\|ORDO]]** — rare disease codes integrated as a MONDO sub-hierarchy
- **OMIM** — Mendelian disease entries mapped to MONDO
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — MONDO disease concepts available in Athena vocabulary

## Connections
- Integrates: [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/ICD-11\|ICD-11]], [[02_Standards/ORDO\|ORDO]], [[02_Standards/HPO\|HPO]], OMIM, DOID
- Used in: [[02_Standards/OMOP CDM\|OMOP CDM]] (disease concepts), [[03_Platforms/EBRAINS\|EBRAINS]], [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]]
- Complements: [[02_Standards/HPO\|HPO]] (phenotypes), [[02_Standards/ORDO\|ORDO]] (rare disease specifics)
- Part of: OBO Foundry
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (harmonising clinical and genomic disease coding)

## Resources
- https://monarchinitiative.org/disease
- https://mondo.monarchinitiative.org (MONDO browser)
- https://obofoundry.org/ontology/mondo.html
- https://github.com/monarch-initiative/mondo (GitHub)
