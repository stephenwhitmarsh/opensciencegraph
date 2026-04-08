---
{"dg-publish":true,"permalink":"/platforms/synapse-amp-ad/","dg-note-properties":{"name":"Synapse / AMP-AD Knowledge Portal","aliases":["Synapse","AMP-AD","AD Knowledge Portal","Sage Bionetworks"],"website":"https://www.synapse.org","type":"platform","scope":"international","domain":["genomics","multimodal","clinical"],"status":"active","founded":2012,"parent_org":"Sage Bionetworks"}}
---


# Synapse / AMP-AD Knowledge Portal

## Overview
**Synapse** is an open science platform developed and operated by **Sage Bionetworks**, a non-profit biomedical research organisation based in Seattle. Synapse provides infrastructure for storing, sharing, and collaborating on scientific data, code, and analyses, with a strong emphasis on reproducibility and FAIR data practices. It hosts some of the most important open multiomics datasets in neuroscience and psychiatry, including the outputs of the **CommonMind Consortium**, **PsychENCODE**, and the **AMP-AD Knowledge Portal**.

The **AMP-AD Knowledge Portal** (https://adknowledgeportal.synapse.org) is a specialised Synapse portal for the **Accelerating Medicines Partnership for Alzheimer's Disease (AMP-AD)** — a public-private partnership between NIH, the FDA, and pharmaceutical companies. It hosts multiomics data from postmortem human brain tissue across multiple Alzheimer's disease cohorts, making it the largest open collection of Alzheimer's transcriptomics, proteomics, and epigenomics data available.

## Hosted Datasets Relevant to Neuroscience

### AMP-AD / Alzheimer's Multiomics
- **ROSMAP** (Religious Orders Study and Memory and Aging Project) — longitudinal Alzheimer's cohort; RNA-seq, methylation, proteomics, metabolomics
- **MSBB** (Mount Sinai Brain Bank) — postmortem brain transcriptomics by brain region
- **Mayo RNAseq** — temporal cortex and cerebellum RNA-seq from AD and controls
- Data types: bulk RNA-seq, scRNA-seq, spatial transcriptomics, proteomics, methylation, ATAC-seq; all in [[Standards/AnnData\|AnnData]] / h5ad or standard formats

### CommonMind Consortium (CMC)
Lead site: [[Actors/Mount Sinai Neuroscience\|Mount Sinai Neuroscience]]. Brain transcriptomics and epigenomics from schizophrenia, bipolar disorder, and ALS postmortem brain tissue. Formats: RNA-seq counts, ATAC-seq peaks, Hi-C contact matrices; metadata via [[Platforms/NCBI GEO\|NCBI GEO]] cross-links.

### PsychENCODE
Lead sites include [[Actors/Mount Sinai Neuroscience\|Mount Sinai Neuroscience]] and multiple US institutions. Multi-omics atlas of the human brain across psychiatric disorders and developmental stages. All data deposited to Synapse under controlled access aligned with [[Platforms/dbGaP\|dbGaP]].

## Platform Features
- **Controlled access** model: researchers register and agree to data use terms; no DAC approval required for most AMP-AD datasets (open access)
- **Reproducible analysis** — Synapse supports provenance tracking and versioned analysis workflows via the Synapse Python/R clients
- **DOI assignment** — every dataset and analysis on Synapse receives a persistent identifier
- **FAIR alignment** — Synapse implements findability (metadata, DOIs), accessibility (open API), interoperability (standard formats), and reusability (clear licences)
- **Challenge platform** — Synapse hosts open ML/data science challenges (DREAM Challenges) for method development on biomedical data

## Relevance to ICM
Synapse / AMP-AD hosts the largest publicly available collection of human brain RNA-seq and multiomics data — directly accessible to [[Actors/DAC\|DAC]] and [[Actors/iGENSEQ\|iGENSEQ]] at ICM for benchmarking RNA-seq pipelines against large reference datasets, integrating ICM neurological disease cohort data with AMP-AD Alzheimer's multiomics, and accessing CommonMind / PsychENCODE psychiatric brain transcriptomics for comparison with ICM psychiatric genomics data.

## Connections
- Operated by: Sage Bionetworks (non-profit)
- Key portals: AMP-AD Knowledge Portal (Alzheimer's); CommonMind Consortium; PsychENCODE; DREAM Challenges
- Lead data contributors: [[Actors/Mount Sinai Neuroscience\|Mount Sinai Neuroscience]], Mayo Clinic, Rush University, multiple US academic centres
- Standards: [[Standards/AnnData\|AnnData]], [[Standards/VCF\|VCF]], standard bioinformatics formats
- Related repositories: [[Platforms/NCBI GEO\|NCBI GEO]] (cross-linked metadata), [[Platforms/dbGaP\|dbGaP]] (controlled access companion), [[Platforms/EGA\|EGA]] (European controlled-access equivalent)
- Relevant to ICM: [[Actors/DAC\|DAC]], [[Actors/iGENSEQ\|iGENSEQ]], Alzheimer's / psychiatric genomics research

## Resources
- https://www.synapse.org (Synapse platform)
- https://adknowledgeportal.synapse.org (AMP-AD Knowledge Portal)
- https://sagebionetworks.org (Sage Bionetworks)
- https://dreamchallenges.org (DREAM Challenges)
