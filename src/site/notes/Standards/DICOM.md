---
{"dg-publish":true,"permalink":"/standards/dicom/","tags":["icm/uses"],"dg-note-properties":{"name":"Digital Imaging and Communications in Medicine","aliases":["DICOM"],"website":"https://www.dicomstandard.org","type":"standard","scope":"international","domain":["neuroimaging","clinical"],"status":"active","founded":1983,"parent_org":"NEMA / DICOM Standards Committee","tags":["icm/uses"],"icon":"https://www.dicomstandard.org/favicon.ico"}}
---


# DICOM — Digital Imaging and Communications in Medicine

## Overview
DICOM is the universal standard for storing, transmitting, and displaying medical imaging data. Developed jointly by the ACR (American College of Radiology) and NEMA (National Electrical Manufacturers Association) from 1983, DICOM defines both the **file format** for medical images and the **network protocol** for communicating between imaging devices, PACS systems, and clinical applications. Every clinical MRI, CT, PET, ultrasound, and X-ray scanner in the world produces DICOM files. All imaging data at [[Actors/CENIR\|CENIR]] originates as DICOM and is subsequently converted to [[Standards/NIfTI\|NIfTI]] and organised into [[Standards/BIDS\|BIDS]] for research use.

## DICOM Object Model
A DICOM dataset is organised hierarchically:
- **Patient** → **Study** → **Series** → **Instance (Image)**
- Each level has a unique identifier (Patient ID, Study Instance UID, Series Instance UID, SOP Instance UID)
- A **DICOM file** = one or more pixel data frames + a structured header of metadata **tags**
- Tags are identified by (Group, Element) pairs, e.g. (0010,0020) = Patient ID, (0008,0060) = Modality (MR, PT, CT…)

## Key SOP Classes (Modalities)
DICOM defines **Service-Object Pair (SOP) Classes** for each imaging modality and service type:

| SOP Class | Description | ICM relevance |
|---|---|---|
| MR Image Storage | Structural/functional MRI | [[Actors/Paris Brain Institute\|ICM]] CENIR 3T MRI ×2 |
| Enhanced MR Image | Multi-frame MRI (fMRI, diffusion) | [[Actors/Paris Brain Institute\|ICM]] CENIR fMRI/dMRI |
| PET Image Storage | PET molecular imaging | [[Actors/Paris Brain Institute\|ICM]] CENIR PET-MRI |
| Secondary Capture | Screenshots, processed images | QC images |
| CT Image Storage | Computed tomography | AP-HP clinical scans |
| Digital X-Ray | Radiography | AP-HP |
| Encapsulated PDF | PDF reports embedded in DICOM | Radiology reports |
| Structured Report (SR) | Machine-readable clinical reports | AP-HP structured reporting |
| Segmentation | Label maps, segmentations | Research pipelines |
| Parametric Map | Quantitative maps (ADC, T1 maps) | Quantitative MRI |

## DICOM Services (Network)
Beyond file storage, DICOM defines network services for clinical workflow:
- **C-STORE** — send images from modality to PACS
- **C-FIND** — query/retrieve metadata from PACS
- **C-MOVE** — retrieve images from remote PACS
- **C-GET** — retrieve images directly
- **WADO-RS** (Web Access to DICOM Objects) — modern RESTful image retrieval; used by [[Standards/HL7 FHIR\|HL7 FHIR]] ImagingStudy resource

## DICOM to Research Pipeline
At [[Actors/CENIR\|CENIR]] and research sites managed by [[Actors/CATI\|CATI]], DICOM files are converted to research formats via standardised pipelines:

```
Scanner → DICOM (raw) → dcm2niix → NIfTI + JSON sidecar → BIDS
                      → heudiconv (alternative converter with automatic naming)
```

Key tools:
- **dcm2niix** — primary DICOM-to-NIfTI converter; produced by Chris Rorden (MRIcroGL); used by [[Actors/CATI\|CATI]] CATIconv pipeline and most BIDS converters
- **heudiconv** — flexible DICOM organiser for automated [[Standards/BIDS\|BIDS]] conversion; used in [[Actors/ReproNim\|ReproNim]] workflows
- **Orthanc** — open-source DICOM server for local PACS and research DICOM management
- **XNAT** ([[Platforms/XNAT\|XNAT]]) — imaging data management platform built on DICOM

## DICOM Structured Reports (SR)
DICOM SR allows machine-readable, coded clinical findings to be embedded directly in the DICOM object alongside images. Used for radiology reports with coded measurements, AI/CAD findings (lesion measurements, segmentation results), and [[Standards/HL7 FHIR\|HL7 FHIR]] DiagnosticReport which can link to DICOM SR objects via WADO-RS.

## Connections
- Converted to: [[Standards/NIfTI\|NIfTI]] (via dcm2niix, heudiconv), then organised into [[Standards/BIDS\|BIDS]]
- Used by: [[Actors/CATI\|CATI]] (CATIconv pipeline), [[Platforms/XNAT\|XNAT]], [[Platforms/LORIS\|LORIS]], [[Governance/AP-HP\|AP-HP]]
- Compatible with: [[Standards/HL7 FHIR\|HL7 FHIR]] (ImagingStudy and DiagnosticReport resources)
- Tools: dcm2niix, heudiconv, Orthanc, [[Platforms/XNAT\|XNAT]]
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (all CENIR acquisitions; primary source format for all MRI, PET-MRI, and MEG-linked MRI data)

## Resources
- https://www.dicomstandard.org
- https://www.dicomstandard.org/current (current standard — Part 1–20)
- https://github.com/rordenlab/dcm2niix (dcm2niix converter)
- https://heudiconv.readthedocs.io (heudiconv BIDS converter)
- https://www.orthanc-server.com (Orthanc DICOM server)
