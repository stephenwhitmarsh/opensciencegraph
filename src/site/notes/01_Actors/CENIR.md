---
{"dg-publish":true,"permalink":"/01-actors/cenir/","tags":["icm/uses"],"dg-note-properties":{"name":"CENIR","aliases":["Centre de NeuroImagerie de Recherche","ICM Neuroimaging Centre"],"website":"https://cenir.institutducerveau.org","type":"facility","scope":"french","domain":["neuroimaging","electrophysiology","clinical"],"status":"active","founded":2010,"parent_org":"Paris Brain Institute","tags":["icm/uses"]}}
---


# CENIR — Centre de NeuroImagerie de Recherche

## Overview
CENIR (Centre de NeuroImagerie de Recherche) is [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]'s
human neuroimaging research centre, one of ICM's 10 core technological platforms.
Located at Pitié-Salpêtrière Hospital, it provides state-of-the-art multimodal
human neuroimaging for research and translational studies, serving ICM research
teams, [[04_Governance/NeurATRIS\|NeurATRIS]] external users, and academic and industrial collaborators.

## Equipment
- **3T MRI × 2** — structural, functional (fMRI), diffusion, spectroscopy
- **PET-MRI** — Siemens Biograph mMR simultaneous PET and MRI; 18F-FDG,
  amyloid, tau, and dopaminergic tracers
- **MEG** — Elekta Neuromag 306-channel magnetoencephalography
- **EEG** — high-density EEG systems
- **TMS** — transcranial magnetic stimulation (combined with EEG/MRI)
- **Eye-tracking** — compatible with MRI and MEG environments

## Research Role
CENIR is the primary neuroimaging node for:
- Multisite cohort studies managed by [[04_Governance/CATI\|CATI]] (MEMENTO, INSIGHT-preAD, iShare)
- [[04_Governance/NeurATRIS\|NeurATRIS]] clinical neuroimaging services (Phase I/II trial imaging endpoints)
- Molecular neuroimaging (PET tracers for Alzheimer's, Parkinson's biomarkers)
- Cognitive neuroscience (fMRI, MEG, EEG combined protocols)

## Data Management
All CENIR data is processed through [[04_Governance/CATI\|CATI]] pipelines:
- Raw DICOM → [[02_Standards/NIfTI\|NIfTI]] conversion and [[02_Standards/BIDS\|BIDS]] organisation via CATIconv
- Multi-site MRI harmonisation and automated QC
- Data deposited on [[03_Platforms/OpenNeuro\|OpenNeuro]] (open datasets) or secure platforms
  for controlled-access cohorts

## Connections
- Hosted at: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]
- Data management: [[04_Governance/CATI\|CATI]] (all data flows through CATI pipelines; DICOM → NIfTI → BIDS)
- Part of: [[04_Governance/France Life Imaging\|France Life Imaging]] (FLI primary neuroimaging node at ICM)
- External access: [[04_Governance/NeurATRIS\|NeurATRIS]] (clinical neuroimaging for Phase I/II trial endpoints)
- Standards: [[02_Standards/BIDS\|BIDS]], [[02_Standards/NIfTI\|NIfTI]], [[02_Standards/DICOM\|DICOM]]
- Cohorts: MEMENTO, INSIGHT-preAD, iShare (multisite longitudinal via CATI)
- Molecular imaging: PET tracers for amyloid, tau, dopamine (Alzheimer's, Parkinson's)

## Resources
- https://cenir.institutducerveau.org
