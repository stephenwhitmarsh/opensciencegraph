---
{"dg-publish":true,"permalink":"/platforms/idr/","dg-note-properties":{"name":"Image Data Resource","aliases":["IDR"],"website":"https://idr.openmicroscopy.org","type":"repository","scope":"international","domain":["bioimaging","multimodal"],"status":"active","founded":2016,"parent_org":"EMBL-EBI / University of Dundee / OME Consortium"}}
---


# IDR — Image Data Resource

## Overview
The Image Data Resource (IDR) is a public repository for reference image datasets from published scientific studies, hosted at EMBL-EBI and built on [[Actors/OME\|OME]] infrastructure (OMERO). IDR serves as the primary open-access repository for biological microscopy and biomedical imaging data, analogous to what [[Platforms/OpenNeuro\|OpenNeuro]] is for neuroimaging — a curated, FAIR-compliant public archive of imaging datasets associated with peer-reviewed publications.

IDR is operated jointly by EMBL-EBI and the University of Dundee OME team, and is part of the BioImage Archive ecosystem. It focuses on reference datasets — meaning datasets that support reproducibility and reanalysis of published findings — rather than raw data submissions.

## Scope and Content
IDR hosts imaging datasets across a wide range of biological imaging modalities including light microscopy (fluorescence, confocal, super-resolution, high-content screening), electron microscopy (TEM, SEM, correlative CLEM), medical imaging (clinical radiology and pathology datasets), high-content screening (phenotypic screens with associated compound libraries), and spatial transcriptomics and multiplexed imaging.

All datasets are linked to their source publications and curated with structured metadata following [[Standards/REMBI\|REMBI]] (Recommended Metadata for Biological Images) and [[Standards/OME File Formats\|OME File Formats]] standards.

## Technical Infrastructure
IDR runs on [[Actors/OME\|OME]]'s OMERO platform, providing programmatic access via OMERO Python/Java/R APIs, web-based image browsing and annotation, integration with Jupyter notebooks for remote analysis, metadata in [[Standards/OME File Formats\|OME File Formats]] (OME-TIFF, OME-Zarr) for interoperability, and DOI assignment via EMBL-EBI data submission system.

## Relationship to BioImage Archive
IDR and the BioImage Archive (BIA, https://www.ebi.ac.uk/biostudies/bioimages) are complementary EMBL-EBI services: **IDR** — curated reference datasets from published studies; OMERO-based; rich metadata and re-analysis tools; **BIA** — broader submission repository for all biological image data supporting open access mandates (analogous to ENA for sequences).

## Connections
- Built on: [[Actors/OME\|OME]] (OMERO platform)
- File formats: [[Standards/OME File Formats\|OME File Formats]] (OME-TIFF, OME-Zarr)
- Metadata standard: [[Standards/REMBI\|REMBI]]
- Hosted by: EMBL-EBI / University of Dundee
- Part of: [[Governance/Euro-BioImaging\|Euro-BioImaging]] data services ecosystem
- Complements: BioImage Archive (broader image submission), [[Platforms/OpenNeuro\|OpenNeuro]] (neuroimaging)
- Used by: [[Governance/France BioImaging\|France BioImaging]] nodes (data deposition pathway)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (ICM Quant microscopy data deposition)

## Resources
- https://idr.openmicroscopy.org
- https://idr.openmicroscopy.org/about/
- https://www.ebi.ac.uk/biostudies/bioimages (BioImage Archive)
