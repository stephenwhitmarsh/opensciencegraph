---
{"dg-publish":true,"permalink":"/02-standards/bids/","tags":["icm/uses"],"dg-note-properties":{"name":"Brain Imaging Data Structure","aliases":["BIDS"],"website":"https://bids.neuroimaging.io","type":"standard","scope":"international","domain":["neuroimaging","electrophysiology","behavior","genomics","multimodal"],"status":"active","founded":2016,"parent_org":"INCF","tags":["icm/uses"],"icon":"https://bids.neuroimaging.io/assets/img/bids-logo.png"}}
---


# BIDS — Brain Imaging Data Structure

## Overview
BIDS (Brain Imaging Data Structure) is the de facto community standard for organising and describing neuroimaging and electrophysiology datasets in a consistent, machine-readable directory and file naming structure. Published in 2016 (Gorgolewski et al., *Nature Scientific Data*), BIDS emerged from the need to eliminate the idiosyncratic, lab-specific dataset organisation that made sharing and reuse of neuroimaging data nearly impossible. It is now mandated or strongly recommended by all major neuroscience data repositories and is the primary format for open neuroimaging data worldwide.

BIDS is governed by [[01_Actors/INCF\|INCF]] and the [[04_Governance/BIDS Steering Group\|BIDS Steering Group]] via an open, community-driven extension process. [[04_Governance/CATI\|CATI]] at [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] uses BIDS for all its multi-site cohort data management.

## What BIDS Defines
BIDS specifies:
- **Directory structure** — how to organise `sub-`, `ses-`, `task-`, `run-` folders
- **File naming conventions** — deterministic file names from key-value pairs (e.g. `sub-01_ses-01_task-rest_bold.nii.gz`)
- **Sidecar JSON metadata** — standardised fields describing acquisition parameters alongside each data file
- **Dataset description** — `dataset_description.json`, `participants.tsv`, `README`, `CHANGES` at the root level
- **Derivatives** — a separate conventions layer for processed data (preprocessed, segmentations, statistical maps)

## Covered Modalities
The core BIDS specification and its extensions (BEPs) cover:
- **MRI** — structural (T1w, T2w, FLAIR), functional (BOLD), diffusion (DWI), perfusion (ASL), quantitative MRI
- **PET** — PET brain imaging with blood input function metadata
- **EEG** — scalp electroencephalography
- **MEG** — magnetoencephalography
- **iEEG** — intracranial EEG (stereo-EEG, ECoG)
- **Microscopy** — histology and optical microscopy (BEP031)
- **MRS** — magnetic resonance spectroscopy (BEP038)
- **Genetics** — genomics data associated with imaging participants (BEP018)
- **Motion** — body motion capture data (BEP029)

## BEP Extension Process
New modalities and data types are added via **BIDS Extension Proposals (BEPs)** — a community-driven RFC-style process where anyone can propose, discuss, and implement extensions:
- BEPs are tracked on GitHub with open discussion
- Accepted BEPs are merged into the official BIDS specification
- The [[04_Governance/BIDS Steering Group\|BIDS Steering Group]] governs the process and ratifies proposals

## BIDS Apps
**BIDS Apps** is an ecosystem of containerised (Docker/Singularity) data analysis pipelines that accept BIDS-organised datasets as input and produce BIDS derivatives:
- **fMRIPrep** — robust fMRI preprocessing (used by [[03_Platforms/OpenNeuro\|OpenNeuro]] automated processing)
- **dMRIPrep** — diffusion MRI preprocessing
- **MRIQC** — automated MRI quality metrics and reports
- **HCP Pipelines** — Human Connectome Project minimal preprocessing
- **FreeSurfer** (via fMRIPrep) — cortical surface reconstruction
- **BIDS Validator** — checks dataset compliance with the BIDS specification

## BIDS Raw vs Derivatives
BIDS distinguishes two dataset layers:
- **Raw BIDS** — unprocessed data as acquired; the standard BIDS structure
- **BIDS Derivatives** — processed outputs stored under `derivatives/` with provenance metadata (which pipeline, which version, which parameters) using the BIDS Derivatives convention

## Connections
- Governed by: [[01_Actors/INCF\|INCF]], [[04_Governance/BIDS Steering Group\|BIDS Steering Group]]
- Requires: [[02_Standards/NIfTI\|NIfTI]] (mandatory MRI/PET image format within BIDS)
- Compatible with: [[02_Standards/NIDM\|NIDM]] (provenance layer), [[02_Standards/HED\|HED]] (event annotation)
- Required by: [[03_Platforms/OpenNeuro\|OpenNeuro]], [[03_Platforms/EBRAINS\|EBRAINS]], [[03_Platforms/DANDI Archive\|DANDI Archive]], [[01_Actors/CONP\|CONP]], [[03_Platforms/BrainLife.io\|BrainLife.io]]
- Adopted by: [[01_Actors/ReproNim\|ReproNim]], [[03_Platforms/NeuroVault\|NeuroVault]], [[03_Platforms/LORIS\|LORIS]], [[04_Governance/CATI\|CATI]], [[03_Platforms/Neurobagel\|Neurobagel]], [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]
- Used with: [[02_Standards/DICOM\|DICOM]] (source format, converted via dcm2niix/heudiconv)
- Reference publication: Gorgolewski et al. (2016) *Nature Scientific Data* doi:10.1038/sdata.2016.44

## Resources
- https://bids.neuroimaging.io
- https://bids-specification.readthedocs.io (full specification)
- https://github.com/bids-standard (GitHub organisation)
- https://bids-apps.neuroimaging.io (BIDS Apps ecosystem)
- https://bids.neuroimaging.io/get_started.html (getting started guide)
