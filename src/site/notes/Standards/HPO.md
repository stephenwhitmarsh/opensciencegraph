---
{"dg-publish":true,"permalink":"/standards/hpo/","dg-note-properties":{"name":"Human Phenotype Ontology","aliases":["HPO"],"website":"https://hpo.jax.org","type":"terminology","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2008,"parent_org":"The Jackson Laboratory / Monarch Initiative","icon":"https://hpo.jax.org/favicon.ico"}}
---


# HPO - Human Phenotype Ontology

## Overview
The Human Phenotype Ontology is the standard controlled vocabulary for describing human disease phenotypes — abnormal morphological, physiological, and behavioural features — in a machine-readable, hierarchically organised format. With 18,000+ terms covering all organ systems including the nervous system, HPO is the primary phenotype language for rare disease genomics globally. It is directly integrated into [[Standards/Phenopackets\|Phenopackets]] and is used by virtually every rare disease gene discovery programme, including neurological disease cohorts relevant to [[Actors/Paris Brain Institute\|Paris Brain Institute]].

## Created / Governed By
- The Jackson Laboratory (JAX) and the Monarch Initiative — primary development
- International rare disease community — community-curated ontology
- Endorsed by: [[Actors/GA4GH\|GA4GH]] (integrated into [[Standards/Phenopackets\|Phenopackets]])

## Key Features
- 18,000+ terms organised in a directed acyclic graph (DAG) hierarchy
- Covers all organ systems; neurology/psychiatry terms are especially rich (e.g. seizure types, cognitive phenotypes, movement disorders, dementia)
- Linked to OMIM, Orphanet, ClinVar, and DECIPHER disease databases
- Available in OWL and OBO formats for computational use
- Updated monthly; versioned releases with stable term identifiers (HP:XXXXXXX)

## Neuroscience Relevance
HPO's neurological and psychiatric sub-ontologies are among the most detailed, covering terms for epilepsy, intellectual disability, autism spectrum, cerebellar ataxia, movement disorders, dementia, white matter abnormalities, and more. These terms are essential for phenotype-driven gene discovery and patient stratification in rare neurology.

## Connections
- Integrated into: [[Standards/Phenopackets\|Phenopackets]] (primary phenotype vocabulary)
- Used by: [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/ELIXIR\|ELIXIR]], Orphanet, DECIPHER, ClinVar
- Governed by: [[Actors/GA4GH\|GA4GH]] (via Phenopackets Work Stream)
- Maps to: [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/OMOP CDM\|OMOP CDM]] (via concept mapping)
- Complements: [[Standards/MONDO\|MONDO]] (disease-level), [[Standards/ORDO\|ORDO]] (rare disease specifics)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (rare neurological disease research)
- Part of: [[Governance/OBO Foundry\|OBO Foundry]] (https://obofoundry.org/ontology/hp.html)

## Resources
- https://hpo.jax.org
- https://github.com/obophenotype/human-phenotype-ontology
- https://obofoundry.org/ontology/hp.html
