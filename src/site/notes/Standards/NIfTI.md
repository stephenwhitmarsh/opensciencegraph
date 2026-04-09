---
{"dg-publish":true,"permalink":"/standards/n-if-ti/","tags":["icm/uses"],"dg-note-properties":{"name":"Neuroimaging Informatics Technology Initiative File Format","aliases":["NIfTI","NIfTI-1","NIfTI-2",".nii",".nii.gz"],"website":"https://nifti.nimh.nih.gov","type":"standard","scope":"international","domain":["neuroimaging"],"status":"active","founded":2004,"parent_org":"NIfTI Data Format Working Group (NIH / NIMH)","tags":["icm/uses"],"icon":"https://nifti.nimh.nih.gov/favicon.ico"}}
---


# NIfTI - Neuroimaging Informatics Technology Initiative File Format

## Overview
NIfTI (.nii / .nii.gz) is the universal file format for storing processed
neuroimaging data — structural MRI, functional MRI, diffusion MRI, and PET
volumes. Developed in 2004 by a NIH-convened working group to replace the
fragmented ANALYZE 7.5 format, NIfTI is as foundational to neuroimaging as
[[Standards/DICOM\|DICOM]] is to clinical imaging and [[Standards/VCF\|VCF]] is to genomics. It sits at the
centre of the neuroimaging pipeline: [[Standards/DICOM\|DICOM]] files from scanners are converted
to NIfTI (via tools such as dcm2niix), NIfTI files are then organised into
[[Standards/BIDS\|BIDS]] datasets, and NIfTI is the input/output format for virtually every
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
NIfTI is the pivot format: produced from [[Standards/DICOM\|DICOM]], consumed by analysis tools,
and organised by [[Standards/BIDS\|BIDS]]. The [[Standards/BIDS\|BIDS]] specification mandates NIfTI as the
required image format for MRI and PET data.

## Connections
- Converted from: [[Standards/DICOM\|DICOM]] (via dcm2niix, heudiconv, MRIcroGL)
- Required by: [[Standards/BIDS\|BIDS]] (mandatory MRI/PET image format within BIDS datasets)
- Used by: [[Governance/CATI\|CATI]], [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/LORIS\|LORIS]], [[Platforms/XNAT\|XNAT]], [[Platforms/EBRAINS\|EBRAINS]],
  [[Platforms/BrainLife.io\|BrainLife.io]], [[Platforms/NeuroVault\|NeuroVault]], [[Platforms/DANDI Archive\|DANDI Archive]] (indirectly via BIDS)
- Analysis ecosystems: FSL, FreeSurfer, SPM, ANTs, nilearn, MRtrix3, AFNI
- Related formats: DICOM (source), [[Standards/CIFTI\|CIFTI]] (surface+volume HCP format),
  MGH/MGZ (FreeSurfer native), MINC (Canadian neuroimaging format)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Governance/CATI\|CATI]], [[Actors/Human Connectome Project\|Human Connectome Project]],
  [[Actors/ADNI\|ADNI]], [[Actors/UK Biobank\|UK Biobank]], [[Actors/ENIGMA Consortium\|ENIGMA Consortium]]

## Resources
- https://nifti.nimh.nih.gov
- https://nifti.nimh.nih.gov/nifti-1 (NIfTI-1 specification)
- https://nifti.nimh.nih.gov/nifti-2 (NIfTI-2 specification)
- https://github.com/rordenlab/dcm2niix (primary DICOM→NIfTI converter)
