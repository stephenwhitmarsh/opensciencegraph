---
{"dg-publish":true,"permalink":"/01-actors/dac/","tags":["icm/uses"],"dg-note-properties":{"name":"Data Analysis Core","aliases":["DAC","ICM Data Analysis Core"],"website":"https://dac.institutducerveau.org","type":"facility","scope":"french","domain":["multimodal","genomics","neuroimaging"],"status":"active","founded":2010,"parent_org":"Paris Brain Institute","tags":["icm/uses"]}}
---


# DAC — Data Analysis Core

## Overview
The Data Analysis Core (DAC) is [[00_Core/Paris Brain Institute\|Paris Brain Institute]]'s bioinformatics
and statistical analysis support platform, one of ICM's 10 core technological
platforms. It provides computational expertise, analysis pipelines, training,
and consultation to ICM research teams and external collaborators, bridging
the gap between data production (at platforms like [[01_Actors/iGENSEQ\|iGENSEQ]], [[01_Actors/CENIR\|CENIR]],
and [[01_Actors/Banque ADN et Cellules\|Banque ADN et Cellules]]) and publication-ready scientific outputs.

The DAC is staffed by bioinformaticians, statisticians, and data scientists
who work embedded in or in close collaboration with ICM research teams. It
implements [[04_Governance/FAIR Principles\|FAIR Principles]] in ICM data management workflows and serves
as the primary interface between ICM and national infrastructure providers
[[04_Governance/IFB\|IFB]] and [[04_Governance/OPIDoR\|OPIDoR]].

## Divisions and Services

The DAC is organised into four divisions serving both internal ICM teams and external
biomedical research projects, on a collaborative basis (co-authorship model) or
fee-for-service for standardised analyses.

### Omics Analysis
Processing and visualisation of high-throughput sequencing (NGS) data from [[01_Actors/iGENSEQ\|iGENSEQ]]:
- **Genomics** — gene panel, whole-exome sequencing (WES), whole-genome sequencing (WGS)
- **Transcriptomics** — bulk RNA-seq, non-coding RNA, small RNA, splice variants
- **Single-cell RNA-seq** and spatial transcriptomics
- **Epigenomics** — DNA methylation, ATAC-seq (chromatin accessibility), ChIP-seq
- **Long-read sequencing** — Oxford Nanopore (ONT)
- Pipelines built with Snakemake, Conda, Docker for reproducibility and portability
- **DEJAVU** — ICM-internal tool aggregating exome/genome short variants from ~3,000
  ICM project samples
- **QUBY** — web interface for researchers to self-explore RNA-seq, scRNA-seq,
  and WES data analysed by DAC

### Biostatistics
- Expert statistical support from study design through to data interpretation
- Responsive helpdesk for researchers at any stage of their project
- Advanced statistical methods for high-dimensional and multimodal data:
  omics, electrophysiology, cell imaging, neuroimaging, and clinical data

### Data Management
- FAIR data management: databases and secure web interfaces aligned with shared
  data models
- Develops and implements ICM's data management policy
- Data Management Plans in collaboration with legal, data protection, and
  integrity officers, and the innovation office
- Provides databases and data warehouse infrastructure to exploit transversal
  potential of ICM data

### Training and Outreach
- Regular training programme spanning bioinformatics, biostatistics, and RDM
- Tools covered: Git, OMERO+, [[03_Platforms/REDCap\|REDCap]], Tumorotek, [[04_Governance/OPIDoR\|OPIDoR]]
- DMP writing sessions (mandatory for ANR/Horizon Europe projects)
- Image analysis courses (ImageJ, MATLAB; available on-demand online)
- Statistics helpdesk every 1st and 3rd Friday
- Custom sessions for research teams available on request
- Recent catalogue (Jan–Mar 2026): survival analysis, MRI segmentation, single-cell
  workshops, REDCap training, spatial transcriptomics focus groups

## Computing Infrastructure
DAC activities run on ICM IT-managed high-performance computing equipment:
- Illumina DRAGEN Bio-IT Platform
- 800-core compute cluster
- High-performance storage and database servers
- Application servers

## Open Science Role
The DAC is ICM's primary interface with the French and European open science
infrastructure:
- **[[04_Governance/IFB\|IFB]]** — DAC is a member of IFB and participates in the coordination of
  several of its missions and its executive committee; uses IFB NNCR computing
  resources; participates in the [[04_Governance/MUDIS4LS\|MUDIS4LS]] initiative (managed by IFB)
- **[[04_Governance/OPIDoR\|OPIDoR]]** — DAC provides DMP training and support using OPIDoR tools;
  DMP writing is part of the regular training programme
- **[[04_Governance/FAIR Principles\|FAIR Principles]]** — the Data Management division implements FAIR data
  management across ICM through databases, data models, and policy development
- **Reproducibility** — omics pipelines use Snakemake, Conda, Docker;
  training covers Git and open-source tools

## Connections
- Hosted at: [[00_Core/Paris Brain Institute\|Paris Brain Institute]]
- Member of: [[04_Governance/IFB\|IFB]] (participates in IFB missions and executive committee)
- Participates in: [[04_Governance/MUDIS4LS\|MUDIS4LS]] initiative (managed by [[04_Governance/IFB\|IFB]])
- REDCap support: [[03_Platforms/REDCap\|REDCap]] (instance management, training, helpdesk for clinical data collection)
- DMP tools: [[04_Governance/OPIDoR\|OPIDoR]]
- Affiliated to: Sorbonne Université Omics network (Réseau Omique)
- Upstream platforms: [[01_Actors/iGENSEQ\|iGENSEQ]] (omics data production), [[01_Actors/CENIR\|CENIR]] (neuroimaging)
- Standards: [[02_Standards/VCF\|VCF]], [[04_Governance/FAIR Principles\|FAIR Principles]], [[02_Standards/BIDS\|BIDS]]
- Policy: [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/Ouvrir la Science\|Ouvrir la Science]]

## Resources
- https://dac.institutducerveau.org
- https://dac.institutducerveau.org/services/ (full services catalogue)
- https://dac.institutducerveau.org/service/omics/ (omics analysis division)
- https://dac.institutducerveau.org/service/training/ (training programme)
