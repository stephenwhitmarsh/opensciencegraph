---
{"dg-publish":true,"permalink":"/standards/rembi/","dg-note-properties":{"name":"Recommended Metadata for Biological Images","aliases":["REMBI"],"website":"https://www.nature.com/articles/s41592-021-01166-8","type":"standard","scope":"international","domain":["bioimaging"],"status":"active","founded":2021,"parent_org":"EMBL-EBI / BioImage Archive community"}}
---


# REMBI — Recommended Metadata for Biological Images

## Overview
REMBI is a community-developed metadata framework for biological image data,
published in 2021 (Sarkans et al., *Nature Methods*) as a consensus output of
a broad working group spanning the BioImage Archive (EMBL-EBI), [[Governance/Euro-BioImaging\|Euro-BioImaging]],
[[Actors/OME\|OME]], and the wider bioimaging community. It provides a structured set of
recommended metadata fields covering study, biosample, specimen, acquisition,
image data, and image analysis — applicable across all biological microscopy
modalities. REMBI is the metadata layer used by the BioImage Archive and is
increasingly adopted by [[Governance/QUAREP-LiMi\|QUAREP-LiMi]], [[Governance/France BioImaging\|France BioImaging]], and [[Actors/OME\|OME]]
tooling. It is the bioimaging equivalent of the structured metadata that [[Standards/BIDS\|BIDS]]
provides for neuroimaging.

## Created / Governed By
- EMBL-EBI / BioImage Archive — primary development
- [[Governance/Euro-BioImaging\|Euro-BioImaging]] — co-development and adoption
- [[Actors/OME\|OME]] — integration with OME-Zarr / OME-NGFF metadata
- [[Governance/QUAREP-LiMi\|QUAREP-LiMi]] — QC metadata alignment

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
- Adopted by: BioImage Archive (EMBL-EBI), [[Governance/Euro-BioImaging\|Euro-BioImaging]]
- Integrated with: [[Standards/OME File Formats\|OME File Formats]] (OME-Zarr RO-Crate metadata)
- Aligned with: [[Governance/QUAREP-LiMi\|QUAREP-LiMi]] (QC metadata), [[Governance/GT-GeDeM\|GT-GeDeM]] (DMP guidelines)
- Complements: [[Standards/BIDS\|BIDS]] (BIDS has a microscopy BEP building on REMBI concepts)
- Relevant to: [[Governance/France BioImaging\|France BioImaging]], [[Actors/Institut Pasteur\|Institut Pasteur]], [[Actors/Institut Curie\|Institut Curie]],
  [[Actors/Paris Brain Institute\|Paris Brain Institute]] (microscopy data management)

## Resources
- https://www.nature.com/articles/s41592-021-01166-8 (Sarkans et al. 2021)
- https://www.ebi.ac.uk/bioimage-archive/rembi/ (BioImage Archive REMBI guide)
