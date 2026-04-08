---
{"dg-publish":true,"permalink":"/02-standards/ado/","tags":["icm/uses"],"dg-note-properties":{"name":"Alzheimer's Disease Ontology","aliases":["ADO"],"website":"https://bioportal.bioontology.org/ontologies/ADO","type":"terminology","scope":"international","domain":["clinical","neuroimaging"],"status":"active","founded":2016,"parent_org":"University of Michigan / BioPortal community","tags":["icm/uses"]}}
---


# ADO — Alzheimer's Disease Ontology

## Overview
The Alzheimer's Disease Ontology (ADO) is a domain ontology covering the concepts
relevant to Alzheimer's disease research: biomarkers, pathology, clinical stages,
genetic risk factors, therapeutic interventions, and cognitive assessments. It
provides a semantic framework that links the biological and clinical dimensions
of Alzheimer's disease — connecting amyloid and tau biomarker measurements
to NIA-AA clinical staging criteria to genetic risk (APOE, PSEN1/2) to imaging
findings. For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], which hosts the MEMENTO and
INSIGHT-preAD cohorts via [[04_Governance/CATI\|CATI]], ADO provides the vocabulary for semantically
annotating Alzheimer's cohort data in a way that enables cross-study comparison.

## Key Concept Areas
- **Biomarkers** — amyloid-β (CSF, PET), tau (phospho-tau, tangles, PET),
  NfL, synaptic biomarkers; aligned with [[02_Standards/LOINC\|LOINC]] codes
- **Clinical stages** — NIA-AA criteria (preclinical, MCI, dementia stages),
  ATN framework (Amyloid, Tau, Neurodegeneration)
- **Genetic factors** — APOE ε4, PSEN1/2, APP mutations; linked to [[02_Standards/HPO\|HPO]]/[[02_Standards/OMIM\|OMIM]]
- **Imaging findings** — hippocampal atrophy, amyloid PET positivity,
  white matter hyperintensities; aligned with [[02_Standards/BIDS\|BIDS]] and [[02_Standards/NIfTI\|NIfTI]] conventions
- **Cognitive assessments** — MMSE, MoCA, CDR, neuropsychological battery results;
  alignable with [[02_Standards/LOINC\|LOINC]] clinical scales

## Role in the ICM Data Ecosystem
- **MEMENTO cohort** — multisite French Alzheimer's prevention cohort managed
  by [[04_Governance/CATI\|CATI]]; ADO provides semantic annotation of biomarker and imaging data
- **INSIGHT-preAD** — longitudinal Alzheimer's prevention study at ICM;
  ADO terms bridge biomarker measurements to clinical staging
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — ADO concepts can be mapped to OMOP standard vocabulary
  for cohort queries combining Alzheimer's staging with health data

## Connections
- Complements: [[02_Standards/HPO\|HPO]] (phenotype terms), [[02_Standards/MONDO\|MONDO]] (disease-level classification),
  [[02_Standards/LOINC\|LOINC]] (biomarker measurements), [[02_Standards/SNOMED CT\|SNOMED CT]] (clinical findings)
- Relevant platforms: [[04_Governance/CATI\|CATI]], [[03_Platforms/EBRAINS\|EBRAINS]], [[04_Governance/Health Data Hub\|Health Data Hub]]
- Related cohorts: [[01_Actors/ADNI\|ADNI]] (North American Alzheimer's neuroimaging cohort)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (MEMENTO, INSIGHT-preAD, clinical programmes)

## Resources
- https://bioportal.bioontology.org/ontologies/ADO
- https://www.alzforum.org (Alzheimer's disease research resource portal)
