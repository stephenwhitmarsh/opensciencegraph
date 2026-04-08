---
{"dg-publish":true,"permalink":"/standards/cifti/","tags":["icm/uses"],"dg-note-properties":{"name":"Connectivity Informatics Technology Initiative File Format","aliases":["CIFTI","CIFTI-2",".dscalar.nii",".dtseries.nii",".dlabel.nii"],"website":"https://www.nitrc.org/projects/cifti/","type":"standard","scope":"international","domain":["neuroimaging"],"status":"active","founded":2013,"parent_org":"Human Connectome Project / WU-Minn HCP Consortium","tags":["icm/uses"]}}
---


# CIFTI — Connectivity Informatics Technology Initiative File Format

## Overview
CIFTI is a neuroimaging file format for surface+volume (greyordinate) data, developed by the [[Actors/Human Connectome Project\|Human Connectome Project]] to overcome the limitations of purely volumetric formats like [[Standards/NIfTI\|NIfTI]] for cortical data. Where NIfTI stores brain data as a 3D voxel volume, CIFTI stores data along brain structure axes that combine cortical surface vertices (left and right hemispheres) with subcortical volume voxels — enabling more biologically meaningful spatial representation of cortical activity and connectivity. It is the standard format for HCP-style analyses and is increasingly adopted in high-resolution human neuroimaging studies.

## Created / Governed By
- [[Actors/Human Connectome Project\|Human Connectome Project]] (WU-Minn consortium) — original development
- NITRC community — specification hosting and community governance
- CIFTI-2 (2014) — current stable version

## Key Features
- Stores data along brain structure axes: cortical surface vertices + subcortical voxels
- File extensions encode content type: `.dscalar.nii` (scalars), `.dtseries.nii` (time series), `.dlabel.nii` (parcellations), `.pconn.nii` (parcellated connectivity)
- Built on NIfTI-2 container with XML header extensions
- Enables surface-based smoothing and analysis without volume interpolation artefacts
- Standard for HCP Multimodal Parcellation (MMP) atlas
- Supported by Connectome Workbench, FSL, nibabel, HCP pipelines

## Position in the Neuroimaging Pipeline
```
fMRI/dMRI acquisition → DICOM → NIfTI (volumetric)
                                    → [HCP pipelines / Connectome Workbench]
                                         → CIFTI (surface+volume greyordinates)
```

## Connections
- Developed by: [[Actors/Human Connectome Project\|Human Connectome Project]]
- Built on: [[Standards/NIfTI\|NIfTI]] (uses NIfTI-2 as container format)
- Used with: [[Standards/BIDS\|BIDS]] (BIDS has a CIFTI derivatives BEP)
- Related formats: [[Standards/NIfTI\|NIfTI]] (volumetric), GIfTI (surface geometry), [[Standards/OME File Formats\|OME File Formats]] (microscopy equivalent)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Governance/CATI\|CATI]], [[Actors/Donders Institute\|Donders Institute]], [[Actors/ENIGMA Consortium\|ENIGMA Consortium]]

## Resources
- https://www.nitrc.org/projects/cifti/
- https://humanconnectome.org/software/connectome-workbench (Workbench tools)
- https://github.com/CIFTI/CIFTI-2 (CIFTI-2 specification)
