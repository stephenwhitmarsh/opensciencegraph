---
{"dg-publish":true,"permalink":"/governance/mudis-4-ls/","tags":["icm/participates"],"dg-note-properties":{"name":"MUDIS4LS","aliases":["Mutualised Digital Spaces for FAIR Data in Life and Health Sciences","MuDiS4LS"],"website":"https://www.france-bioinformatique.fr/en/mudis4ls/","type":"infrastructure","scope":"french","domain":["genomics","multimodal","health"],"status":"active","founded":2021,"parent_org":"IFB / ANR Equipex+ PIA3","tags":["icm/participates"]}}
---


# MUDIS4LS — Mutualised Digital Spaces for FAIR Data in Life and Health Sciences

## Overview
MUDIS4LS (Mutualized Digital Spaces for FAIR data in Life and Health Sciences) is a French national infrastructure project funded under the ANR Equipex+ PIA3 programme, coordinated by [[Governance/IFB\|IFB]] (Institut Français de Bioinformatique / ELIXIR-FR). Running from 2021, it brings together 39 teams from 14 organisations, 4 national data centres, 7 regional data centres, and 6 national data-producing infrastructures to build a shared, scalable, FAIR-compliant digital infrastructure for French life and health sciences research data.

MUDIS4LS is the next-generation evolution of IFB's National Network of Computing Resources (NNCR), extending its scope, capacity, and governance to cover the full data lifecycle — from production through analysis, secure mid-term storage, and eventual public release in national or international repositories.

## Key Objectives

### Data Flow Orchestration
A central goal is enabling scientists to control biological data flows throughout their lifecycle: from origin at national data-producing infrastructures (France Génomique, France BioImaging, France Life Imaging, etc.) through
intermediate analysis phases to public release in repositories such as [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Platforms/EBRAINS\|EBRAINS]], [[Platforms/OpenNeuro\|OpenNeuro]], or international archives (EGA, NCBI GEO, ENA).

### Shared Computing Infrastructure
Builds on and extends the NNCR: mutualized HPC and cloud resources across IFB's 21 member platforms in 9 regions of France. Provides hosting, computing, and storage services under a shared governance model with permanent staff from platforms contributing to operations.

### FAIR Data Management and AI
- Develops FAIR-compliant data management frameworks for multi-omics, imaging, and phenotype data integration
- Addresses AI for life sciences through standardised data pipelines compatible with machine learning workflows
- Provides structured DMP support via [[Governance/OPIDoR\|OPIDoR]] tooling

### Implementation Studies (Thematic Pilots)
Five case studies demonstrating the framework across different communities:
1. **IS1** — multi-omics and imaging integration (most relevant to neuroscience)
2. **IS2** — marine ecology (EMBRC France)
3. **IS3** — health data (interfaces with [[Governance/Health Data Hub\|Health Data Hub]] ecosystem)
4. **IS4** — microbial research
5. **IS5** — agriculture

## Relevance to Paris Brain Institute
For [[Actors/Paris Brain Institute\|Paris Brain Institute]], MUDIS4LS is relevant through:
- **IS1 (multi-omics + imaging integration)** — directly addresses the challenge of combining neuroimaging data ([[Standards/BIDS\|BIDS]] / [[Governance/CATI\|CATI]]) with genomics ([[Actors/iGENSEQ\|iGENSEQ]]) and clinical data ([[Standards/OMOP CDM\|OMOP CDM]]) in a FAIR-compliant framework
- **IS3 (health data)** — interfaces with [[Governance/Health Data Hub\|Health Data Hub]] and [[Governance/EHDS\|EHDS]] secondary use infrastructure
- **DAC connectivity** — ICM's Data Analysis Core uses IFB platforms and benefits from the NNCR computing resources extended under MUDIS4LS

## Connections
- Coordinated by: [[Governance/IFB\|IFB]] (IFB manages MUDIS4LS)
- Part of: [[Governance/INBS\|INBS]] ecosystem
- Data-producing infrastructure partners: France Génomique, [[Governance/France BioImaging\|France BioImaging]], [[Governance/France Life Imaging\|France Life Imaging]], EMBRC France, and others
- Repository alignment: [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Governance/EOSC\|EOSC]], [[Governance/OpenAIRE\|OpenAIRE]]
- DMP tooling: [[Governance/OPIDoR\|OPIDoR]] (FAIR compliance and data management plans)
- Standards: [[Governance/FAIR Principles\|FAIR Principles]], [[Standards/BIDS\|BIDS]], [[Standards/VCF\|VCF]], [[Standards/OME File Formats\|OME File Formats]]
- Policy: [[Governance/Ouvrir la Science\|Ouvrir la Science]], [[Governance/ANR Open Science Policy\|ANR Open Science Policy]]
- Funded by: ANR Equipex+ PIA3 (France 2030 programme)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (multi-omics integration, computing)

## Resources
- https://www.france-bioinformatique.fr/en/mudis4ls/
- https://zenodo.org/records/5229331 (IFB roadmap describing MUDIS4LS)
