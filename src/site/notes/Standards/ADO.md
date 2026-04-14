---
{"dg-publish":true,"permalink":"/standards/ado/","dg-note-properties":{"name":"Alzheimer's Disease Ontology","aliases":["ADO"],"website":"https://bioportal.bioontology.org/ontologies/ADO","type":"terminology","scope":"international","domain":["clinical","neuroimaging"],"status":"active","founded":2016,"parent_org":"University of Michigan / BioPortal community","tags":null}}
---


# ADO — Alzheimer's Disease Ontology

## Overview
The Alzheimer's Disease Ontology (ADO) is a domain ontology covering the concepts relevant to Alzheimer's disease research: biomarkers, pathology, clinical stages, genetic risk factors, therapeutic interventions, and cognitive assessments. It provides a semantic framework that links the biological and clinical dimensions of Alzheimer's disease — connecting amyloid and tau biomarker measurements to NIA-AA clinical staging criteria to genetic risk (APOE, PSEN1/2) to imaging findings. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], which hosts the MEMENTO and INSIGHT-preAD cohorts via [[Governance/CATI\|CATI]], ADO provides the vocabulary for semantically annotating Alzheimer's cohort data in a way that enables cross-study comparison.

## Key Concept Areas
- **Biomarkers** — amyloid-β (CSF, PET), tau (phospho-tau, tangles, PET), NfL, synaptic biomarkers; aligned with [[Standards/LOINC\|LOINC]] codes
- **Clinical stages** — NIA-AA criteria (preclinical, MCI, dementia stages), ATN framework (Amyloid, Tau, Neurodegeneration)
- **Genetic factors** — APOE ε4, PSEN1/2, APP mutations; linked to [[Standards/HPO\|HPO]]/[[Standards/OMIM\|OMIM]]
- **Imaging findings** — hippocampal atrophy, amyloid PET positivity, white matter hyperintensities; aligned with [[Standards/BIDS\|BIDS]] and [[Standards/NIfTI\|NIfTI]] conventions
- **Cognitive assessments** — MMSE, MoCA, CDR, neuropsychological battery results; alignable with [[Standards/LOINC\|LOINC]] clinical scales

## Role in the ICM Data Ecosystem
- **MEMENTO cohort** — multisite French Alzheimer's prevention cohort managed by [[Governance/CATI\|CATI]]; ADO provides semantic annotation of biomarker and imaging data
- **INSIGHT-preAD** — longitudinal Alzheimer's prevention study at ICM; ADO terms bridge biomarker measurements to clinical staging
- **[[Standards/OMOP CDM\|OMOP CDM]]** — ADO concepts can be mapped to OMOP standard vocabulary for cohort queries combining Alzheimer's staging with health data

## Connections
- Complements: [[Standards/HPO\|HPO]] (phenotype terms), [[Standards/MONDO\|MONDO]] (disease-level classification), [[Standards/LOINC\|LOINC]] (biomarker measurements), [[Standards/SNOMED CT\|SNOMED CT]] (clinical findings)
- Relevant platforms: [[Governance/CATI\|CATI]], [[Platforms/EBRAINS\|EBRAINS]], [[Governance/Health Data Hub\|Health Data Hub]]
- Related cohorts: [[Actors/ADNI\|ADNI]] (North American Alzheimer's neuroimaging cohort)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (MEMENTO, INSIGHT-preAD, clinical programmes)

## Resources
- https://bioportal.bioontology.org/ontologies/ADO
- https://www.alzforum.org (Alzheimer's disease research resource portal)
