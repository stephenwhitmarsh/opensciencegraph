---
{"dg-publish":true,"permalink":"/02-standards/n-if-ti/","tags":["icm/uses"],"dg-note-properties":{"name":"Neuroimaging Informatics Technology Initiative File Format","aliases":["NIfTI","NIfTI-1","NIfTI-2",".nii",".nii.gz"],"website":"https://nifti.nimh.nih.gov","type":"standard","scope":"international","domain":["neuroimaging"],"status":"active","founded":2004,"parent_org":"NIfTI Data Format Working Group (NIH / NIMH)","tags":["icm/uses"],"icon":"https://nifti.nimh.nih.gov/favicon.ico"}}
---


# NIfTI - Neuroimaging Informatics Technology Initiative File Format

## Overview
NIfTI (.nii / .nii.gz) is the universal file format for storing processed
neuroimaging data — structural MRI, functional MRI, diffusion MRI, and PET
volumes. Developed in 2004 by a NIH-convened working group to replace the
fragmented ANALYZE 7.5 format, NIfTI is as foundational to neuroimaging as
[[02_Standards/DICOM\|DICOM]] is to clinical imaging and [[02_Standards/VCF\|VCF]] is to genomics. It sits at the
centre of the neuroimaging pipeline: [[02_Standards/DICOM\|DICOM]] files from scanners are converted
to NIfTI (via tools such as dcm2niix), NIfTI files are then organised into
[[02_Standards/BIDS\|BIDS]] datasets, and NIfTI is the input/output format for virtually every
neuroimaging analysis tool (FSL, FreeSurfer, SPM, ANTs, nilearn, MRtrix3, etc.).

## Created / Governed By
- NIfTI Data Format Working Group — NIH/NIMH-convened committee (2003–2004)
- Neuroimaging community — de facto governance through widespread adoption
- NIfTI-2 (2011) extended to 64-bit dimensions for large datasets

## Key Features
- Single-file (.nii) or dual-file (.hdr/.img) format; gzip-compressed (.nii.gz)
  widely used
- Stores 3D/4D image arrays with a rich header encoding voxel dimensions,
  orientation (qform/sform affine matrices), data type, and acquisition parameters
- NIfTI-2 supports array dimensions > 32,767 voxels (required for high-resolution
  and high-temporal-resolution data)
- Carries spatial coordinate system information essential for cross-study alignment
  to standard brain spaces (MNI152, Talairach)
- Lightweight and widely readable; no proprietary dependencies

## Position in the Neuroimaging Pipeline
```
Scanner → DICOM → [dcm2niix / heudiconv] → NIfTI → BIDS → Analysis tools
                                                   ↓
                                            OpenNeuro / EBRAINS / LORIS
```
NIfTI is the pivot format: produced from [[02_Standards/DICOM\|DICOM]], consumed by analysis tools,
and organised by [[02_Standards/BIDS\|BIDS]]. The [[02_Standards/BIDS\|BIDS]] specification mandates NIfTI as the
required image format for MRI and PET data.

## Connections
- Converted from: [[02_Standards/DICOM\|DICOM]] (via dcm2niix, heudiconv, MRIcroGL)
- Required by: [[02_Standards/BIDS\|BIDS]] (mandatory MRI/PET image format within BIDS datasets)
- Used by: [[04_Governance/CATI\|CATI]], [[03_Platforms/OpenNeuro\|OpenNeuro]], [[03_Platforms/LORIS\|LORIS]], [[03_Platforms/XNAT\|XNAT]], [[03_Platforms/EBRAINS\|EBRAINS]],
  [[03_Platforms/BrainLife.io\|BrainLife.io]], [[03_Platforms/NeuroVault\|NeuroVault]], [[03_Platforms/DANDI Archive\|DANDI Archive]] (indirectly via BIDS)
- Analysis ecosystems: FSL, FreeSurfer, SPM, ANTs, nilearn, MRtrix3, AFNI
- Related formats: DICOM (source), [[02_Standards/CIFTI\|CIFTI]] (surface+volume HCP format),
  MGH/MGZ (FreeSurfer native), MINC (Canadian neuroimaging format)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], [[04_Governance/CATI\|CATI]], [[01_Actors/Human Connectome Project\|Human Connectome Project]],
  [[01_Actors/ADNI\|ADNI]], [[01_Actors/UK Biobank\|UK Biobank]], [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]]

## Resources
- https://nifti.nimh.nih.gov
- https://nifti.nimh.nih.gov/nifti-1 (NIfTI-1 specification)
- https://nifti.nimh.nih.gov/nifti-2 (NIfTI-2 specification)
- https://github.com/rordenlab/dcm2niix (primary DICOM→NIfTI converter)
