---
{"dg-publish":true,"permalink":"/02-standards/vcf/","dg-note-properties":{"name":"Variant Call Format","aliases":["VCF","BCF"],"website":"https://samtools.github.io/hts-specs/VCFv4.4.pdf","type":"standard","scope":"international","domain":["genomics"],"status":"active","founded":2010,"parent_org":"GA4GH / hts-specs community","icon":"https://www.ga4gh.org/favicon.ico"}}
---


# VCF - Variant Call Format

## Overview
VCF is the universal file format for storing genomic variant data — single nucleotide polymorphisms (SNPs), insertions/deletions (indels), structural variants, and copy number variants. Originally developed by the 1000 Genomes Project in 2010, it is now maintained by [[01_Actors/GA4GH\|GA4GH]] through the hts-specs community and is as foundational to genomics as [[02_Standards/DICOM\|DICOM]] is to medical imaging. Every genomics study, including neurogenomics and psychiatric genetics research, produces and exchanges data in VCF format. BCF (Binary Call Format) is the compressed binary equivalent.

## Created / Governed By
- [[01_Actors/GA4GH\|GA4GH]] — maintains the VCF specification via the hts-specs repository
- 1000 Genomes Project — original development (2010)

## Key Features
- Tab-delimited text format with structured header and data sections
- Supports multi-sample genotyping across cohorts of any size
- Encodes genotype quality scores, read depths, and filter flags
- BCF binary equivalent for efficient storage and random access
- Widely supported by all major genomics tools (GATK, bcftools, Plink, etc.)

## Connections
- Governed by: [[01_Actors/GA4GH\|GA4GH]]
- Companion formats: SAM/BAM/CRAM (sequence alignments, also GA4GH-maintained)
- Used in conjunction with: [[02_Standards/Phenopackets\|Phenopackets]] (links variants to phenotype)
- Relevant data resources: [[01_Actors/UK Biobank\|UK Biobank]] (whole-exome/genome data), [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] (biobank genomics), [[01_Actors/ADNI\|ADNI]] (genetics)
- Mandated for: [[04_Governance/EHDS\|EHDS]] secondary use of genomic data (from March 2031)
- FAIR deposit: requires persistent identifiers and rich metadata per [[01_Actors/GA4GH\|GA4GH]] guidelines

## Resources
- https://samtools.github.io/hts-specs/VCFv4.4.pdf
- https://github.com/samtools/hts-specs
