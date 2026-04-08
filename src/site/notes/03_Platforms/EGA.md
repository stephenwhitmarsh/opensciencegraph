---
{"dg-publish":true,"permalink":"/03-platforms/ega/","tags":["icm/uses"],"dg-note-properties":{"name":"European Genome-phenome Archive","aliases":["EGA"],"website":"https://ega-archive.org","type":"repository","scope":"european","domain":["genomics","clinical"],"status":"active","founded":2008,"parent_org":"EMBL-EBI / Centre for Genomic Regulation (CRG)","tags":["icm/uses"]}}
---


# EGA — European Genome-phenome Archive

## Overview
The European Genome-phenome Archive (EGA) is the primary European controlled-access
repository for human genomic and phenotypic data from biomedical research studies.
Operated jointly by EMBL-EBI (Hinxton) and the Centre for Genomic Regulation (CRG,
Barcelona), EGA stores data that cannot be publicly released due to patient privacy
and consent restrictions — requiring researchers to apply for access through a
Data Access Committee (DAC) established by the data submitter.

EGA is directly relevant to [[00_Core/Paris Brain Institute\|Paris Brain Institute]] for depositing and accessing
genomic and multi-omics data from neurological disease studies involving human
participants, where privacy constraints preclude open release in repositories
like [[03_Platforms/NCBI GEO\|NCBI GEO]].

## What EGA Stores
- **Whole genome sequencing (WGS)** — germline and somatic variant data
- **Whole exome sequencing (WES)** — targeted coding variant data
- **SNP genotyping arrays** — GWAS data
- **RNA-seq** — bulk and single-cell transcriptomics with phenotypic linkage
- **Epigenomics** — methylation, ChIP-seq, ATAC-seq
- **Phenotypic data** — clinical annotations, diagnoses, biomarkers linked
  to genomic data
- **Multi-omics** — integrated datasets combining several data types

## Access Model
EGA uses a **two-tier access model**:
1. **Data submission** — researchers submit data and establish a DAC with defined
   access conditions (consent-based, IRB-linked)
2. **Data access** — external researchers apply to the DAC for access; approved
   applicants receive secure download credentials

This model complies with GDPR and enables sharing of sensitive health data under
controlled conditions — aligned with [[04_Governance/EHDS\|EHDS]] secondary use frameworks.

## Federated EGA (FEGA)
The **Federated EGA** initiative extends the EGA model to national nodes,
allowing countries to host sensitive genomic data locally while maintaining
discoverability in the central EGA catalogue. French sensitive genomic data
may eventually be hosted via a French FEGA node aligned with [[04_Governance/Health Data Hub\|Health Data Hub]]
and [[04_Governance/EHDS\|EHDS]] requirements.

## Connections
- Operated by: EMBL-EBI + CRG (Barcelona)
- Part of: [[04_Governance/ELIXIR\|ELIXIR]] data services, [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] (biobank data)
- Access governance: [[01_Actors/GA4GH\|GA4GH]] Data Use Ontology (DUO) for machine-readable
  consent terms; [[02_Standards/Phenopackets\|Phenopackets]] for phenotype linkage
- Standards: [[02_Standards/VCF\|VCF]], [[01_Actors/GA4GH\|GA4GH]] standards (Beacon API, DRS)
- Complementary open-access: [[03_Platforms/NCBI GEO\|NCBI GEO]], [[03_Platforms/DDBJ\|DDBJ]]
- French alignment: [[04_Governance/Health Data Hub\|Health Data Hub]] (health data), [[04_Governance/IFB\|IFB]] (ELIXIR-FR node)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (controlled-access genomics from
  neurological disease cohorts, GWAS data, multi-omics)

## Resources
- https://ega-archive.org
- https://ega-archive.org/federated (Federated EGA)
- https://www.ga4gh.org/product/data-use-ontology-duo/ (DUO for access conditions)
