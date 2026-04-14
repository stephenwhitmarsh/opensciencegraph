---
{"dg-publish":true,"permalink":"/actors/dac/","tags":["icm/uses"],"dg-note-properties":{"name":"Data Analysis Core","aliases":["DAC","ICM Data Analysis Core"],"website":"https://dac.institutducerveau.org","type":"facility","scope":"french","domain":["multimodal","genomics","neuroimaging"],"status":"active","founded":2010,"parent_org":"Paris Brain Institute","tags":["icm/uses"]}}
---


# DAC — Data Analysis Core

## Overview
The Data Analysis Core (DAC) is [[Actors/Paris Brain Institute\|Paris Brain Institute]]'s bioinformatics and statistical analysis support platform, one of ICM's 10 core technological platforms. It provides computational expertise, analysis pipelines, training, and consultation to ICM research teams and external collaborators, bridging the gap between data production (at platforms like [[Actors/iGENSEQ\|iGENSEQ]], [[Actors/CENIR\|CENIR]], and [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]]) and publication-ready scientific outputs.

The DAC is staffed by bioinformaticians, statisticians, and data scientists who work embedded in or in close collaboration with ICM research teams. It implements [[Governance/FAIR Principles\|FAIR Principles]] in ICM data management workflows and serves as the primary interface between ICM and national infrastructure providers [[Governance/IFB\|IFB]] and [[Governance/OPIDoR\|OPIDoR]].

## Divisions and Services

The DAC is organised into four divisions serving both internal ICM teams and external biomedical research projects, on a fee-for-service.

### Omics Analysis
Processing and visualisation of high-throughput sequencing (NGS) data from [[Actors/iGENSEQ\|iGENSEQ]]:
- **Genomics** — gene panel, whole-exome sequencing (WES), whole-genome sequencing (WGS)
- **Transcriptomics** — bulk RNA-seq, non-coding RNA, small RNA, splice variants
- **Single-cell RNA-seq** and spatial transcriptomics
- **Epigenomics** — DNA methylation, ATAC-seq (chromatin accessibility), ChIP-seq
- **Long-read sequencing** — Oxford Nanopore (ONT)
- Pipelines built with Snakemake and Conda for reproducibility and portability
- **DEJAVU** — ICM-internal tool aggregating exome/genome short variants from ~3,000 ICM project samples
- **QUBY** — [web interface](https://quby.icm-institute.org/) for researchers to self-explore RNA-seq, scRNA-seq, and WES data analysed by DAC

### Biostatistics
- Expert statistical support from study design through to data interpretation
- Responsive helpdesk for researchers at any stage of their project
- Advanced statistical methods for high-dimensional and multimodal data: omics, electrophysiology, cell imaging, neuroimaging, and clinical data

### Data Management
- FAIR data management: databases and secure web interfaces aligned with shared data models
- Develops and implements ICM's data management policy
- Data Management Plans in collaboration with CDO, legal, data protection, and integrity officers, and the innovation office

### Training and Outreach
- Regular training programme spanning bioinformatics, biostatistics, and RDM
- Tools covered: Git, OMERO+, [[Platforms/REDCap\|REDCap]], Tumorotek, [[Governance/OPIDoR\|OPIDoR]]
- DMP writing sessions (mandatory for ANR/Horizon Europe projects)
- Statistics helpdesk every 1st and 3rd Friday
- Custom sessions for research teams available on request
- Recent catalogue (Jan–Mar 2026): survival analysis, MRI segmentation, single-cell workshops, REDCap training, spatial transcriptomics focus groups

## Computing Infrastructure
DAC activities run on ICM IT-managed high-performance computing equipment:
- Illumina DRAGEN Bio-IT Platform
- 800-core compute cluster
- High-performance storage and database servers
- Application servers

## Open Science Role
The DAC is ICM's primary interface with the French and European open science infrastructure:
- **[[Governance/IFB\|IFB]]** — DAC is a member of [[Governance/IFB\|IFB]] and participates in the [[Governance/MUDIS4LS\|MUDIS4LS]] initiative (managed by IFB); IFB computing resources are planned for future use
- Working groups — DAC participates in workgroups including [[Governance/GT-GeDeM\|GT-GeDeM]],  [[Governance/INCF Working Groups\|INCF Working Groups]] and [[Governance/GFRN\|GFRN]]
- **[[Governance/OPIDoR\|OPIDoR]]** — DAC provides DMP training and support using [[Governance/OPIDoR\|OPIDoR]] tools
- **[[Governance/FAIR Principles\|FAIR Principles]]** — the Data Management division implements FAIR data management across ICM through databases, data models, and policy development
- **Reproducibility** — omics pipelines use Snakemake, Conda and open-source tools

## Connections
- Hosted at: [[Actors/Paris Brain Institute\|Paris Brain Institute]]
- Member of: [[Governance/IFB\|IFB]] (participates in IFB missions and executive committee)
- Participates in: [[Governance/MUDIS4LS\|MUDIS4LS]] initiative (managed by [[Governance/IFB\|IFB]])
- REDCap support: [[Platforms/REDCap\|REDCap]] (instance management, training, helpdesk for clinical data collection)
- DMP tools: [[Governance/OPIDoR\|OPIDoR]]
- Affiliated to: Sorbonne Université Omics network (Réseau Omique)
- Upstream platforms: [[Actors/iGENSEQ\|iGENSEQ]] (omics data production), [[Actors/CENIR\|CENIR]] (neuroimaging)
- Standards: [[Standards/VCF\|VCF]], [[Governance/FAIR Principles\|FAIR Principles]], [[Standards/BIDS\|BIDS]]
- Policy: [[Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[Governance/Ouvrir la Science\|Ouvrir la Science]]

## Resources
- https://dac.institutducerveau.org
- https://dac.institutducerveau.org/services/ (full services catalogue)
- https://dac.institutducerveau.org/service/omics/ (omics analysis division)
- https://dac.institutducerveau.org/service/training/ (training programme)
- https://scicrunch.org/resolver/SCR_026138 (RRID:SCR_026138)
