---
{"dg-publish":true,"permalink":"/standards/me-sh/","dg-note-properties":{"name":"Medical Subject Headings","aliases":["MeSH","MeSH terms"],"website":"https://www.nlm.nih.gov/mesh/","type":"terminology","scope":"international","domain":["clinical","multimodal"],"status":"active","founded":1960,"parent_org":"National Library of Medicine (NLM) / NIH"}}
---


# MeSH — Medical Subject Headings

## Overview
Medical Subject Headings (MeSH) is the controlled vocabulary thesaurus produced and maintained by the US National Library of Medicine (NLM) for indexing, cataloguing, and searching biomedical and health-related literature. Established in 1960, MeSH is the primary indexing system for **PubMed** — the world's largest biomedical literature database — meaning every article indexed in PubMed is tagged with MeSH terms describing its subject matter.

MeSH provides a hierarchically organised vocabulary of ~30,000 descriptors covering diseases, anatomy, organisms, drugs, chemicals, biological processes, and research methodology. It is one of the most widely used biomedical controlled vocabularies in the world, and is referenced across clinical research infrastructure including [[Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]] (condition coding), [[Standards/OMOP CDM\|OMOP CDM]] (concept mapping), and [[Platforms/dbGaP\|dbGaP]] (phenotype description).

## Structure
MeSH is organised into **Descriptor Records** (main concepts) and **Supplementary Concept Records** (chemicals, drugs, rare diseases). Descriptors are arranged in a polyhierarchical tree structure (MeSH Tree) with 16 top-level categories:
- **C — Diseases** — the most relevant category for clinical neuroscience; includes neurological diseases (C10), psychiatric disorders (F03), etc.
- **A — Anatomy** — brain structures, cell types, nervous system anatomy
- **D — Chemicals and Drugs** — neurotransmitters, drugs, chemical compounds
- **G — Phenomena and Processes** — biological and physiological processes
- **F — Psychiatry and Psychology** — cognitive processes, behaviour
- **E — Analytical, Diagnostic and Therapeutic Techniques** — imaging, electrophysiology, clinical procedures

## Role in Clinical Research Infrastructure
- **PubMed indexing** — all PubMed articles are MeSH-tagged; MeSH terms are the primary controlled vocabulary for literature search
- **[[Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]]** — condition and intervention fields use MeSH terms for standardised trial registration and search
- **[[Standards/OMOP CDM\|OMOP CDM]]** — MeSH concepts mapped in the OMOP vocabulary (via Athena) for conditions and drug classes
- **[[Platforms/dbGaP\|dbGaP]]** — phenotype descriptions in GWAS studies use MeSH disease terms
- **[[Platforms/NIF\|NIF]]** — RRID registry uses MeSH for resource categorisation
- **[[Standards/GO\|GO]]** / **[[Standards/HPO\|HPO]]** alignment — MeSH disease terms cross-referenced with HPO phenotype terms and GO biological process terms

## Relationship to Other Disease Terminologies
MeSH, [[Standards/ICD-10\|ICD-10]], [[Standards/SNOMED CT\|SNOMED CT]], and [[Standards/MONDO\|MONDO]] serve different purposes but overlap:

| Terminology | Primary use | Granularity |
|---|---|---|
| MeSH | Literature indexing (PubMed) | Moderate; optimised for search |
| [[Standards/ICD-10\|ICD-10]] | Clinical billing / epidemiology | High; codeable diagnoses |
| [[Standards/SNOMED CT\|SNOMED CT]] | Clinical records / EHR | Very high; post-coordinated |
| [[Standards/MONDO\|MONDO]] | Cross-database harmonisation | High; maps all others |
| [[Standards/HPO\|HPO]] | Phenotype description | Very high; symptom-level |

## Connections
- Produced by: NLM / NIH
- Used by: PubMed, [[Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]], [[Platforms/dbGaP\|dbGaP]], [[Standards/OMOP CDM\|OMOP CDM]], [[Platforms/NIF\|NIF]]
- Maps to: [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/ICD-10\|ICD-10]], [[Standards/MONDO\|MONDO]], [[Standards/HPO\|HPO]] (via cross-references)
- Complements: [[Standards/RxNorm\|RxNorm]] (MeSH covers drug classes; RxNorm covers clinical formulations)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (PubMed literature search; ClinicalTrials.gov registration; OMOP CDM concept mapping)

## Resources
- https://www.nlm.nih.gov/mesh/ (MeSH homepage)
- https://meshb.nlm.nih.gov (MeSH Browser)
- https://pubmed.ncbi.nlm.nih.gov (PubMed — primary MeSH-indexed literature database)
