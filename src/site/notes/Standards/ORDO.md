---
{"dg-publish":true,"permalink":"/standards/ordo/","tags":["icm/uses"],"dg-note-properties":{"name":"Orphanet Rare Disease Ontology","aliases":["ORDO","Orphanet","ORPHA"],"website":"https://www.orpha.net","type":"terminology","scope":"international","domain":["clinical","genomics"],"status":"active","founded":2012,"parent_org":"Orphanet (INSERM / European Commission)","tags":["icm/uses"],"icon":"https://www.orpha.net/favicon.ico"}}
---


# ORDO — Orphanet Rare Disease Ontology

## Overview
ORDO is the Orphanet Rare Disease Ontology, providing the European standard classification of rare diseases with 10,000+ rare conditions, their clinical descriptions, genetic causes, epidemiological data, and relationships. Maintained by the **Orphanet** consortium (coordinated by INSERM in France), ORDO is the mandatory coding system for rare diseases in European Reference Networks (ERNs) and is deeply integrated into French rare disease research infrastructure. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], which conducts extensive research on rare neurological diseases (rare epilepsies, rare ataxias, rare dementias, rare movement disorders), ORDO is the primary coding system.

## Structure
ORDO organises rare diseases using ORPHA codes (e.g. ORPHA:411 for Parkinson's disease, ORPHA:282 for Huntington's disease) at five levels of classification:
- **Disorder** — a specific rare condition (e.g. ORPHA:899 Rett syndrome)
- **Group of disorders** — clinical or aetiological groupings
- **Subtype** — clinical or genetic subtypes
- **Morphological anomaly** — structural malformations
- **Biological anomaly** — abnormal biological findings

## French Relevance
- **Orphanet** is headquartered in Paris, coordinated by INSERM — making it a direct ICM neighbour institution
- All French **Centres de Référence Maladies Rares (CRMR)** use ORPHA codes
- [[Governance/Health Data Hub\|Health Data Hub]] rare disease module uses ORDO for coding
- European Reference Networks (ERNs) — ERN-RND (rare neurological diseases) and ERN-EpiCARE (rare epilepsies) use ORDO for patient registry coding

## Key Neurological ORPHA Codes
| ORPHA Code | Disease |
|---|---|
| ORPHA:411 | Parkinson's disease |
| ORPHA:26929 | Alzheimer's disease |
| ORPHA:282 | Huntington's disease |
| ORPHA:98895 | Rare cerebellar ataxia (group) |
| ORPHA:208 | Friedreich's ataxia |
| ORPHA:306695 | CARASIL |

## Connections
- Part of: [[Standards/MONDO\|MONDO]] (ORDO integrated as MONDO sub-hierarchy)
- Complements: [[Standards/HPO\|HPO]] (phenotype description alongside ORPHA disease codes)
- Integrated in: [[Governance/Health Data Hub\|Health Data Hub]] (rare disease), [[Governance/BBMRI-ERIC\|BBMRI-ERIC]] (biobank coding)
- French parent: INSERM (→ [[Governance/Inserm Open Science\|Inserm Open Science]])
- Part of: [[Governance/OBO Foundry\|OBO Foundry]] ecosystem
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (rare neurological disease research, CRMR)

## Resources
- https://www.orpha.net
- https://www.orphadata.com (ORDO SPARQL endpoint and downloads)
- https://www.orpha.net/consor/cgi-bin/Disease.php (disease browser)
