---
{"dg-publish":true,"permalink":"/platforms/db-ga-p/","dg-note-properties":{"name":"Database of Genotypes and Phenotypes","aliases":["dbGaP"],"website":"https://dbgap.ncbi.nlm.nih.gov","type":"repository","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2006,"parent_org":"National Center for Biotechnology Information (NCBI) / NIH"}}
---


# dbGaP — Database of Genotypes and Phenotypes

## Overview
The Database of Genotypes and Phenotypes (dbGaP) is the NIH repository for controlled-access human genomic and phenotypic data from studies investigating the relationship between genotype and phenotype — particularly genome-wide association studies (GWAS), sequencing studies, and epidemiological cohorts. Operated by NCBI/NIH, it is the US counterpart to the European [[Platforms/EGA\|EGA]] for controlled-access genomic research data.

dbGaP hosts data from major NIH-funded neurological and psychiatric research initiatives including ADSP (Alzheimer's Disease Sequencing Project), ABCD Study, UK Biobank-linked studies, and numerous GWAS for neurological diseases.

## Access Model
dbGaP uses a **controlled-access model** managed by NIH: **open access** — aggregate-level summary statistics and metadata are freely accessible without approval; **controlled access** — individual-level genotype and phenotype data requires a Data Access Request (DAR) approved by the relevant Data Access Committee (DAC). Access requests are submitted through NIH's eRA Commons system. Approved researchers receive dbGaP data via the SRA Toolkit or cloud platforms.

## Key Neuroscience Datasets
Notable neurological/psychiatric datasets hosted in dbGaP:
- **ADSP** — Alzheimer's Disease Sequencing Project (WGS + WES, 20,000+ samples)
- **ABCD Study** — Adolescent Brain Cognitive Development (longitudinal, 11,000+ children)
- **ENIGMA** — summary statistics from multiple ENIGMA working groups
- **NIMH collections** — schizophrenia, bipolar disorder, ASD GWAS datasets
- **UK Biobank GWAS** — neuroimaging and cognitive GWAS summary statistics

## Relationship to Other Repositories
dbGaP is the NIH-primary controlled-access repository, complementing: **[[Platforms/NCBI GEO\|NCBI GEO]]** — open-access gene expression data (GEO hosts open data; dbGaP hosts controlled-access); **[[Platforms/EGA\|EGA]]** — European equivalent for controlled-access genomics; **[[Platforms/DDBJ\|DDBJ]]** — Japanese partner for sequence data (INSDC member); and **SRA** — raw sequencing reads linked from dbGaP studies.

## Connections
- Operated by: NCBI / NIH
- Complementary controlled-access: [[Platforms/EGA\|EGA]] (European equivalent)
- Open-access companion: [[Platforms/NCBI GEO\|NCBI GEO]]
- Standards: [[Standards/VCF\|VCF]], [[Actors/GA4GH\|GA4GH]] (Beacon, DRS), [[Standards/Phenopackets\|Phenopackets]]
- Uses: [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/HPO\|HPO]] for phenotype annotation
- Part of: INSDC data sharing ecosystem (with [[Platforms/DDBJ\|DDBJ]], ENA)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (access to ADSP, ENIGMA GWAS; deposition of neurogenomics data from international collaborations)

## Resources
- https://dbgap.ncbi.nlm.nih.gov
- https://dbgap.ncbi.nlm.nih.gov/aa/wga.cgi?page=login (access request portal)
