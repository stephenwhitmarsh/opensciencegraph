---
{"dg-publish":true,"permalink":"/02-standards/clin-var/","dg-note-properties":{"name":"ClinVar","aliases":["NCBI ClinVar"],"website":"https://www.ncbi.nlm.nih.gov/clinvar/","type":"repository","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2013,"parent_org":"National Center for Biotechnology Information (NCBI) / NIH"}}
---


# ClinVar — NCBI Clinical Variant Database

## Overview
ClinVar is the authoritative public database for clinical interpretations of
genomic variants, operated by NCBI/NIH. It aggregates variant-phenotype
relationships submitted by clinical laboratories, research groups, and expert
panels worldwide, and assigns each variant a **clinical significance
classification** based on submitted evidence. ClinVar is the primary reference
for variant interpretation in clinical genetics and is directly referenced by
[[02_Standards/OMIM\|OMIM]], [[02_Standards/VCF\|VCF]] annotation pipelines, and [[02_Standards/Phenopackets\|Phenopackets]].

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], ClinVar is the key resource for interpreting
genetic variants identified in neurological disease patients through [[01_Actors/iGENSEQ\|iGENSEQ]]
sequencing, linking variants to established pathogenicity evidence for Alzheimer's,
Parkinson's, ALS, and rare neurological diseases.

## What ClinVar Contains
- **Variants** — single nucleotide variants (SNVs), indels, copy number variants,
  structural variants; identified by chromosomal position and HGVS notation
- **Clinical significance** — five-tier classification:
  - Pathogenic / Likely pathogenic
  - Uncertain significance (VUS — Variant of Uncertain Significance)
  - Likely benign / Benign
- **Conditions** — diseases associated with each variant, coded with [[02_Standards/OMIM\|OMIM]]
  MIM numbers, MedGen identifiers (https://www.ncbi.nlm.nih.gov/medgen/), [[02_Standards/MONDO\|MONDO]] and [[02_Standards/HPO\|HPO]] terms
- **Evidence** — PubMed citations, functional studies, population data (gnomAD)
- **Submitters** — laboratories, expert panels (ClinGen), and research groups

## ClinVar and ClinGen
**ClinGen** (Clinical Genome Resource, https://clinicalgenome.org) is a
complementary NIH-funded resource that provides expert panel curation of
variant pathogenicity and gene-disease validity:
- ClinGen Expert Panels (e.g. Hereditary Spastic Paraplegia, Hereditary Ataxia,
  Brain Malformations) submit curated classifications to ClinVar
- ClinGen Gene Curation establishes which genes are definitively associated
  with specific diseases using standardised evidence frameworks
- ClinGen classifications supersede individual laboratory submissions in ClinVar

## Relationship to OMIM and EVA
ClinVar sits at the intersection of variant databases and disease databases:
- **[[02_Standards/OMIM\|OMIM]]** — describes the gene-disease relationship; ClinVar describes
  the specific variant-disease evidence
- **[[03_Platforms/EVA\|EVA]]** — EMBL-EBI's open variant archive; EVA and ClinVar cross-reference
  each other for variants with clinical significance
- **gnomAD** — population allele frequency database used by ClinVar submitters
  to calibrate pathogenicity (rare variants more likely pathogenic)

## Connections
- Operated by: NCBI / NIH
- Cross-references: [[02_Standards/OMIM\|OMIM]] (disease entries), [[02_Standards/HPO\|HPO]] (phenotype terms),
  [[02_Standards/MONDO\|MONDO]] (disease ontology), [[02_Standards/VCF\|VCF]] (variant format for data download)
- Used in: variant annotation pipelines (Ensembl VEP, ANNOVAR, Franklin)
- Related: [[03_Platforms/EVA\|EVA]] (EMBL-EBI open variant archive), ClinGen (expert curation)
- Standards: [[02_Standards/VCF\|VCF]] (variant format), [[02_Standards/Phenopackets\|Phenopackets]] (variant-phenotype linking)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (variant interpretation for neurological
  disease genomics from [[01_Actors/iGENSEQ\|iGENSEQ]]; rare disease diagnosis)

## Resources
- https://www.ncbi.nlm.nih.gov/clinvar/
- https://clinicalgenome.org (ClinGen — expert variant curation)
- https://gnomad.broadinstitute.org (gnomAD — population allele frequencies)
- https://www.ncbi.nlm.nih.gov/clinvar/docs/ftp_primer/ (ClinVar FTP data download)
