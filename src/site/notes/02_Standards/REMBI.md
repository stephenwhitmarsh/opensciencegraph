---
{"dg-publish":true,"permalink":"/02-standards/rembi/","dg-note-properties":{"name":"Recommended Metadata for Biological Images","aliases":["REMBI"],"website":"https://www.nature.com/articles/s41592-021-01166-8","type":"standard","scope":"international","domain":["bioimaging"],"status":"active","founded":2021,"parent_org":"EMBL-EBI / BioImage Archive community"}}
---


# REMBI — Recommended Metadata for Biological Images

## Overview
REMBI is a community-developed metadata framework for biological image data, published in 2021 (Sarkans et al., *Nature Methods*) as a consensus output of a broad working group spanning the BioImage Archive (EMBL-EBI), [[04_Governance/Euro-BioImaging\|Euro-BioImaging]], [[01_Actors/OME\|OME]], and the wider bioimaging community. It provides a structured set of recommended metadata fields covering study, biosample, specimen, acquisition, image data, and image analysis — applicable across all biological microscopy modalities. REMBI is the metadata layer used by the BioImage Archive and is increasingly adopted by [[04_Governance/QUAREP-LiMi\|QUAREP-LiMi]], [[04_Governance/France BioImaging\|France BioImaging]], and [[01_Actors/OME\|OME]] tooling. It is the bioimaging equivalent of the structured metadata that [[02_Standards/BIDS\|BIDS]] provides for neuroimaging.

## Created / Governed By
- EMBL-EBI / BioImage Archive — primary development
- [[04_Governance/Euro-BioImaging\|Euro-BioImaging]] — co-development and adoption
- [[01_Actors/OME\|OME]] — integration with OME-Zarr / OME-NGFF metadata
- [[04_Governance/QUAREP-LiMi\|QUAREP-LiMi]] — QC metadata alignment

## Key Metadata Sections
- **Study** — experimental context, funding, publication links
- **Study Component** — individual imaging experiments within a study
- **Biosample** — organism, tissue, cell type, genetic background
- **Specimen** — sample preparation, labelling, fixation
- **Image Acquisition** — instrument, imaging modality, acquisition parameters
- **Image Data** — file format, dimensions, pixel size, coordinate systems
- **Image Correlation** — for correlative (CLEM) imaging studies
- **Image Analysis** — analysis software, algorithms, output types

## Connections
- Adopted by: BioImage Archive (EMBL-EBI), [[04_Governance/Euro-BioImaging\|Euro-BioImaging]]
- Integrated with: [[02_Standards/OME File Formats\|OME File Formats]] (OME-Zarr RO-Crate metadata)
- Aligned with: [[04_Governance/QUAREP-LiMi\|QUAREP-LiMi]] (QC metadata), [[04_Governance/GT-GeDeM\|GT-GeDeM]] (DMP guidelines)
- Complements: [[02_Standards/BIDS\|BIDS]] (BIDS has a microscopy BEP building on REMBI concepts)
- Relevant to: [[04_Governance/France BioImaging\|France BioImaging]], [[01_Actors/Institut Pasteur\|Institut Pasteur]], [[01_Actors/Institut Curie\|Institut Curie]], [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (microscopy data management)

## Resources
- https://www.nature.com/articles/s41592-021-01166-8 (Sarkans et al. 2021)
- https://www.ebi.ac.uk/bioimage-archive/rembi/ (BioImage Archive REMBI guide)
