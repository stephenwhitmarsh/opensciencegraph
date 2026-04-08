---
{"dg-publish":true,"permalink":"/platforms/platforms/","tags":["MOC"],"dg-note-properties":{"type":"MOC","tags":["MOC"]}}
---

# Platforms and Repositories

*[[MOC\|MOC]]*

This index covers all data platforms, repositories, and data capture systems in the graph. Sections are organised by data domain and research phase, from primary data deposition through to clinical trial infrastructure and general-purpose research data sharing.

---

## Neuroimaging Repositories

- [[Platforms/DANDI Archive\|DANDI Archive]] — [[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]] archive for neurophysiology ([[Standards/NWB\|NWB]] required)
- [[Platforms/EBRAINS\|EBRAINS]] — EU brain research infrastructure; [[Standards/BIDS\|BIDS]] + [[Standards/NWB\|NWB]] + [[Standards/openMINDS\|openMINDS]]; ICM is member
- [[Platforms/NeuroVault\|NeuroVault]] — unthresholded statistical maps, parcellations, atlases; meta-analysis via Neurosynth
- [[Platforms/OpenNeuro\|OpenNeuro]] — leading open [[Standards/BIDS\|BIDS]] repository (MRI, EEG, MEG, iEEG, PET); CC0/PDDL; DataLad

## Neuroimaging Data Management

- [[Platforms/BrainLife.io\|BrainLife.io]] — cloud platform for [[Standards/BIDS\|BIDS]]/[[Standards/NWB\|NWB]] analysis with provenance tracking
- [[Platforms/LORIS\|LORIS]] — open-source data management for multisite neuroimaging studies ([[Actors/ADNI\|ADNI]], [[Actors/CONP\|CONP]], [[Governance/CATI\|CATI]])
- [[Platforms/Neurobagel\|Neurobagel]] — federated participant-level cohort search across [[Standards/BIDS\|BIDS]] datasets; DataLad backend
- [[Platforms/XNAT\|XNAT]] — [[Standards/DICOM\|DICOM]] management and pipeline platform; used at [[Platforms/EBRAINS\|EBRAINS]] member sites

## Neuroscience Multiomics

- [[Platforms/Brain-CODE\|Brain-CODE]] — [[Actors/OBI\|OBI]] neuroinformatics platform; 240+ researchers; [[Platforms/LORIS\|LORIS]]/[[Platforms/XNAT\|XNAT]]/[[Actors/CONP\|CONP]] federation; FAIR; multimodal brain disorder data
- [[Platforms/Synapse AMP-AD\|Synapse AMP-AD]] — Sage Bionetworks; AMP-AD Knowledge Portal; CommonMind; PsychENCODE; open Alzheimer's and psychiatric brain multiomics

## Genomics and Sequence Archives

- [[Platforms/dbGaP\|dbGaP]] — NIH controlled-access repository for GWAS and human genotype-phenotype data
- [[Platforms/DDBJ\|DDBJ]] — Japanese national sequence database; INSDC partner (mirrors NCBI/ENA)
- [[Platforms/EGA\|EGA]] — [[Actors/EMBL\|EMBL]]-EBI/CRG controlled-access repository for human genomics and phenotypic data
- [[Platforms/EVA\|EVA]] — [[Actors/EMBL\|EMBL]]-EBI open-access variant archive; short variants and structural variants
- [[Platforms/NCBI GEO\|NCBI GEO]] — primary open-access repository for gene expression and functional genomics data
- [[Platforms/NeMO Archive\|NeMO Archive]] — primary [[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]] / [[Actors/BICAN\|BICAN]] multi-omics repository; single-cell brain atlas data

## Bioimaging

- [[Platforms/IDR\|IDR]] — [[Actors/EMBL\|EMBL]]-EBI reference image repository ([[Platforms/OMERO\|OMERO]]-based); published microscopy datasets
- [[Platforms/OMERO\|OMERO]] — [[Actors/OME\|OME]]'s institutional image management platform; deployed at [[Governance/Euro-BioImaging\|Euro-BioImaging]] and [[Governance/France BioImaging\|France BioImaging]] nodes

## Clinical Research

- [[Platforms/CleanWEB\|CleanWEB]] — Telemedicine Technologies eClinical suite; [[Governance/AP-HP\|AP-HP]] institutional eCRF platform since 2003; regulatory-grade clinical trials
- [[Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]] — world's largest clinical trial registry and results database (NLM/NIH)
- [[Platforms/REDCap\|REDCap]] — secure web-based eCRF and clinical data capture platform; supported at ICM by [[Actors/DAC\|DAC]]
- [[Platforms/SNDS\|SNDS]] — Systeme National des Donnees de Sante; French national health data system; managed by [[Governance/Health Data Hub\|Health Data Hub]]; core resource for epidemiological and health economics research
- [[Platforms/VIVLI\|VIVLI]] — global clinical trial individual patient data sharing platform; controlled access enclave

## General Research Data and Publications

- [[Platforms/OSF\|OSF]] — Open Science Framework / Center for Open Science; pre-registration, data/code sharing, preprints
- [[Platforms/Preprint Servers\|Preprint Servers]] — bioRxiv (life sciences) and medRxiv (clinical research); open access by default; DOI; ORCID
- [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] — national multidisciplinary research data repository; recommended by [[Governance/ANR Open Science Policy\|ANR]], [[Governance/CNRS Open Science\|CNRS]], [[Governance/Inserm Open Science\|Inserm]]
- [[Platforms/Zenodo\|Zenodo]] — CERN/[[Governance/OpenAIRE\|OpenAIRE]] general-purpose repository; DOIs; recommended for EU-funded projects

---

## Filtering

`type:` — `repository` | `platform`

`domain:` — `neuroimaging` | `genomics` | `bioimaging` | `clinical` | `multimodal` | `health`

`scope:` — `french` | `european` | `international`