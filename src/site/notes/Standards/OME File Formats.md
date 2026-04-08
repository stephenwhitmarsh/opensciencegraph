---
{"dg-publish":true,"permalink":"/standards/ome-file-formats/","dg-note-properties":{"name":"OME File Formats (OME-TIFF and OME-NGFF)","aliases":["OME-TIFF","OME-NGFF","OME-Zarr","OME formats","OME File Formats"],"website":"https://www.openmicroscopy.org/ome-files/","type":"standard","scope":"international","domain":["bioimaging"],"status":"active","founded":2005,"parent_org":"OME Consortium"}}
---


# OME File Formats — OME-TIFF and OME-NGFF (OME-Zarr)

## Overview
The OME file formats are the open standards for storing and sharing biological microscopy image data, produced by the [[Actors/OME\|OME]] consortium. They occupy the same position in the microscopy pipeline that [[Standards/NIfTI\|NIfTI]] occupies in the MRI pipeline and [[Standards/VCF\|VCF]] occupies in genomics — the universal intermediate format that proprietary acquisition formats are converted into for analysis, sharing, and archiving. There are two complementary formats covering different use cases: **OME-TIFF** for stable archival and publication, and **OME-Zarr (OME-NGFF)** for large-scale, cloud-native analysis.

## Created / Governed By
- [[Actors/OME\|OME]] Consortium — primary development and governance
- Community specification process via GitHub (OME-NGFF)
- Endorsed by: [[Governance/Euro-BioImaging\|Euro-BioImaging]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/EOSC\|EOSC]]

## OME-TIFF
The established standard, combining the widely-supported TIFF image format with embedded OME-XML metadata in the image header. Key features:
- Embeds rich structured metadata (acquisition parameters, instrument, channels, specimen, experimenter) directly within the TIFF file
- Supports multi-dimensional data: Z-stacks, time series, multichannel, and tiled large images
- Pyramidal multi-resolution support for whole-slide imaging
- Produced from proprietary formats via **Bio-Formats** (the [[Actors/OME\|OME]] conversion library, analogous to dcm2niix for DICOM→NIfTI)
- Required format for deposition to the BioImage Archive and IDR (Image Data Resource at EMBL-EBI)
- Widely supported by ImageJ/Fiji, QuPath, CellProfiler, OMERO, napari

## OME-NGFF (OME-Zarr)
The next-generation format, designed for cloud storage, streaming access, and very large multidimensional datasets (terabyte-scale light-sheet, expansion microscopy, whole-brain imaging):
- Based on **Zarr** — a chunked, compressed array format enabling random access to any region without downloading the full file
- Cloud-native: reads directly from S3, Google Cloud Storage, or HTTP
- Supports multi-resolution pyramids for progressive rendering
- Separate community metadata specification (OME-NGFF spec, versioned openly)
- Increasingly adopted by [[Governance/Euro-BioImaging\|Euro-BioImaging]] nodes and the BioImage Archive
- The OME 2024 NGFF Challenge deposited 422+ TB of public bioimage data in OME-Zarr format

## Position in the Microscopy Pipeline
```
Microscope → Proprietary format (.czi, .lif, .nd2, ...)
                → [Bio-Formats] → OME-TIFF / OME-Zarr
                                    → OMERO / BioImage Archive / Euro-BioImaging
```

## Connections
- Governed by: [[Actors/OME\|OME]]
- Conversion tool: Bio-Formats (part of [[Actors/OME\|OME]])
- Management platform: OMERO (part of [[Actors/OME\|OME]])
- Adopted by: [[Governance/Euro-BioImaging\|Euro-BioImaging]], [[Governance/France BioImaging\|France BioImaging]], BioImage Archive
- Endorsed by: [[Governance/ELIXIR\|ELIXIR]], [[Governance/EOSC\|EOSC]]
- Metadata standards: [[Standards/REMBI\|REMBI]] (Recommended Metadata for Biological Images), [[Governance/QUAREP-LiMi\|QUAREP-LiMi]] (QC metadata)
- Related formats: [[Standards/NIfTI\|NIfTI]] (MRI equivalent), [[Standards/DICOM\|DICOM]] (clinical imaging), [[Standards/VCF\|VCF]] (genomics equivalent)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (cellular and subcellular microscopy, histology, optogenetics imaging)

## Resources
- https://www.openmicroscopy.org/ome-files/ (OME-TIFF)
- https://ngff.openmicroscopy.org (OME-NGFF specification)
- https://github.com/ome/ngff (community specification repository)
