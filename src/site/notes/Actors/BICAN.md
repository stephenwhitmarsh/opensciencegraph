---
{"dg-publish":true,"permalink":"/actors/bican/","dg-note-properties":{"name":"BRAIN Initiative Cell Atlas Network","aliases":["BICAN"],"website":"https://braininitiative.nih.gov/brain-programs/cell-atlas","type":"consortium","scope":"international","domain":["multimodal","genomics","neuroimaging"],"status":"active","founded":2021,"parent_org":"NIH BRAIN Initiative"}}
---


# BICAN — BRAIN Initiative Cell Atlas Network

## Overview
The BRAIN Initiative Cell Atlas Network (BICAN) is a large-scale NIH programme launched in 2021 to generate a comprehensive, multi-resolution cell atlas of the entire mammalian brain — producing definitive reference maps of all cell types, their molecular profiles, anatomical locations, connectivity, and functional properties across human, non-human primate, and mouse brains.

BICAN is the successor to the BRAIN Initiative Cell Census Network (BICCN), which produced the first comprehensive mouse brain cell atlas. BICAN extends this work to human and primate brains at unprecedented scale, integrating single-cell and single-nucleus RNA-seq, ATAC-seq, spatial transcriptomics, epigenomics, and morphological data with whole-brain connectomics.

## Key Outputs and Data
BICAN data is deposited in multiple specialised archives:
- **NeMO Archive** (https://nemoarchive.org) — primary BICAN multi-omics repository; single-cell and spatial genomics data
- **Brain Image Library (BIL)** — large-scale volumetric microscopy (cleared tissue, EM)
- **DANDI Archive** — electrophysiology data in [[Standards/NWB\|NWB]] format
- **AWS Open Data** — large-scale BICAN datasets via cloud access

## Scientific Scope
BICAN spans several complementary projects:
- **Human Cell Atlas (brain component)** — human single-cell transcriptomics and epigenomics
- **Non-human primate (NHP) atlases** — macaque, marmoset brain atlases
- **Mouse brain atlas** — continuation and expansion of BICCN
- **Spatial transcriptomics** — mapping cell types to anatomical locations using MERFISH, Slide-seq, Visium and related technologies
- **Connectomics** — electron microscopy volumetric reconstructions at synaptic resolution

## Data Standards and Integration
- Single-cell data: [[Standards/NWB\|NWB]] (electrophysiology), AnnData/h5ad (scRNA-seq)
- Spatial data: [[Standards/BIDS\|BIDS]] Microscopy extension
- Anatomical reference: Allen Brain Atlas / [[Standards/UBERON\|UBERON]] for brain region annotation
- Cell type taxonomy: Cell Ontology (CL) — OBO Foundry
- Multi-omics integration aligned with [[Actors/GA4GH\|GA4GH]] standards

## Relevance to Paris Brain Institute
BICAN provides foundational reference data for:
- Neurological disease research at [[Actors/Paris Brain Institute\|Paris Brain Institute]] — cell type context for patient genomics and transcriptomics from [[Actors/iGENSEQ\|iGENSEQ]]
- Comparative analysis with human brain cell type atlases in Alzheimer's, Parkinson's, and ALS research programmes
- Electrophysiology annotation at ePHYS platform — BICAN NHP ephys data provides reference cell-type firing properties

## Connections
- Parent programme: [[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]]
- Data archives: NeMO Archive, DANDI ([[Standards/NWB\|NWB]]), BIL, AWS Open Data
- Standards: [[Standards/NWB\|NWB]], [[Standards/BIDS\|BIDS]], [[Standards/UBERON\|UBERON]], Cell Ontology, [[Actors/GA4GH\|GA4GH]]
- Annotation: [[Standards/GO\|GO]] (gene function)
- Related: Allen Institute for Brain Science ([[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]]) (predecessor atlases), Human Cell Atlas
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (reference cell atlas for disease studies)

## Resources
- https://braininitiative.nih.gov/brain-programs/cell-atlas
- https://nemoarchive.org (NeMO Archive — primary BICAN data)
- https://biccnportal.org (BICCN/BICAN data portal)
- https://portal.brain-map.org (Allen Brain Atlas reference)
