---
{"dg-publish":true,"permalink":"/02-standards/ern-vocabularies/","dg-note-properties":{"name":"European Reference Network Vocabularies","aliases":["ERN vocabularies","ERN-RND","ERN-EpiCARE"],"website":"https://ern-rnd.eu","type":"terminology","scope":"european","domain":["clinical","health"],"status":"active","founded":2017,"parent_org":"European Commission / DG SANTE"}}
---


# ERN Vocabularies — European Reference Network Terminologies

## Overview
The European Reference Networks (ERNs) are virtual networks connecting healthcare
providers across Europe for rare and complex diseases. Established in 2017 under
the Cross-Border Healthcare Directive (2011/24/EU), there are 24 ERNs covering
different disease domains. Two are directly relevant to [[00_Core/Paris Brain Institute\|Paris Brain Institute]]
and the neurological rare disease ecosystem:

- **ERN-RND** — European Reference Network for Rare Neurological Diseases
  (https://ern-rnd.eu); covers rare movement disorders, neurodegenerative diseases,
  hereditary neurological diseases, and neuroimmunological conditions
- **ERN-EpiCARE** — European Reference Network for Rare and Complex Epilepsies
  (https://epi-care.eu); covers rare and complex epilepsy syndromes

Each ERN develops and maintains **patient registry data models and controlled
vocabularies** for their disease domains — these are the "ERN vocabularies"
referenced in this vault.

## ERN-RND Vocabulary and Registry
ERN-RND coordinates the **RND-registry** — a federated European patient registry
for rare neurological diseases built on a shared data model using:
- [[02_Standards/ORDO\|ORDO]] — Orphanet Rare Disease Ontology for disease coding
- [[02_Standards/HPO\|HPO]] — Human Phenotype Ontology for phenotypic characterisation
- [[02_Standards/OMOP CDM\|OMOP CDM]] — for data standardisation enabling federated analyses
- ICD-10/11 codes alongside ORDO for administrative interoperability
- ERN-RND-specific data dictionaries for disease-specific assessments
  (e.g. ataxia rating scales, dystonia severity, Huntington progression)

## ERN-EpiCARE Vocabulary and Registry
ERN-EpiCARE coordinates the **EpiCARE registry** covering rare epilepsy syndromes:
- [[02_Standards/ORDO\|ORDO]] for rare epilepsy syndrome coding
- [[02_Standards/HPO\|HPO]] for seizure type and phenotype description
- ILAE (International League Against Epilepsy) seizure and syndrome classifications
- EEG and imaging data models aligned with [[02_Standards/BIDS\|BIDS]] (EEG-BIDS)

## Relevance to Paris Brain Institute
[[00_Core/Paris Brain Institute\|Paris Brain Institute]] is a member of multiple ERNs through its clinical
partnership with [[04_Governance/AP-HP\|AP-HP]] (Pitié-Salpêtrière Hospital):
- Movement disorders and neurodegenerative disease programmes → ERN-RND
- Epilepsy programmes (with AP-HP neurology) → ERN-EpiCARE
- Rare disease patient data in these registries uses [[02_Standards/ORDO\|ORDO]] + [[02_Standards/HPO\|HPO]] coding,
  consistent with the vault's existing terminology infrastructure

## Connections
- Governed by: European Commission / DG SANTE
- Disease coding: [[02_Standards/ORDO\|ORDO]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/ICD-11\|ICD-11]]
- Phenotype coding: [[02_Standards/HPO\|HPO]]
- Data model: [[02_Standards/OMOP CDM\|OMOP CDM]] (ERN-RND registry)
- Seizure classification: ILAE (external, not yet in vault)
- French healthcare partner: [[04_Governance/AP-HP\|AP-HP]] (Pitié-Salpêtrière)
- Policy context: [[04_Governance/EHDS\|EHDS]] (ERN registries are primary use health data sources
  under EHDS), [[04_Governance/EOSC\|EOSC]]
- Related standards: [[02_Standards/ORDO\|ORDO]], [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/OMOP CDM\|OMOP CDM]]
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (rare neurological disease clinical
  programmes via AP-HP ERN membership)

## Resources
- https://ern-rnd.eu (ERN-RND — Rare Neurological Diseases)
- https://epi-care.eu (ERN-EpiCARE — Rare Epilepsies)
- https://ern-rnd.eu/research/rnd-registry/ (RND-registry)
- https://www.eurordis.org/ern (EURORDIS ERN overview)
- https://health.ec.europa.eu/rare-diseases-and-erns_en (European Commission ERN portal)
