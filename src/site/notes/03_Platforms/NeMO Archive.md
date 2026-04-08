---
{"dg-publish":true,"permalink":"/03-platforms/ne-mo-archive/","dg-note-properties":{"name":"NeMO Archive","aliases":["Neuroscience Multi-Omic Archive"],"website":"https://nemoarchive.org","type":"repository","scope":"international","domain":["genomics","multimodal"],"status":"active","founded":2017,"parent_org":"University of Maryland / NIH BRAIN Initiative"}}
---


# NeMO Archive — Neuroscience Multi-Omic Archive

## Overview
The NeMO Archive (Neuroscience Multi-Omic Archive) is the primary data repository
for multi-omic single-cell data from the **[[01_Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]]** and specifically
the primary archive for [[01_Actors/BICAN\|BICAN]] (BRAIN Initiative Cell Atlas Network) datasets.
Hosted at the University of Maryland Institute for Genome Sciences, NeMO stores
and distributes single-cell and single-nucleus sequencing data — scRNA-seq,
snRNA-seq, scATAC-seq, spatial transcriptomics, multi-omics — from human,
non-human primate, and mouse brain studies.

## What NeMO Stores
- **scRNA-seq / snRNA-seq** — single-cell and single-nucleus transcriptomics
  of brain tissue; the primary data type; stored as [[02_Standards/AnnData\|AnnData]]/h5ad files
- **scATAC-seq** — chromatin accessibility at single-cell resolution
- **Spatial transcriptomics** — MERFISH, Slide-seq, Visium brain tissue maps
- **Multi-omics** — joint transcriptome + chromatin accessibility (SHARE-seq, SNARE-seq)
- **Epigenomics** — DNA methylation (snmC-seq, bisulfite sequencing)
- **Processed data** — cell type annotations, dimensionality reductions,
  clustering results alongside raw counts

## Access Model
NeMO operates a **tiered access model**:
- **Open access** — processed data (cell type annotations, metadata, summary files)
  freely downloadable without registration
- **Controlled access** — raw data from human subjects requires data access
  request (similar to [[03_Platforms/dbGaP\|dbGaP]]); managed through NeMO Access portal
- **NeMO Analytics** — cloud-based analysis workspace for controlled-access data
  (analogous to [[03_Platforms/VIVLI\|VIVLI]] Enclave or [[04_Governance/Health Data Hub\|Health Data Hub]] Datalab)

## BICAN Datasets
NeMO is the primary repository for [[01_Actors/BICAN\|BICAN]] data:
- **Human Brain Cell Atlas** — comprehensive human brain single-cell taxonomy;
  millions of cells across all major brain regions
- **Non-human primate atlases** — macaque and marmoset brain cell atlases
- **Mouse brain atlas** — continuation and expansion of BICCN mouse data
- **Spatial transcriptomics** — MERFISH brain maps with cell type spatial distributions
- These datasets provide the reference cell type framework for neurological
  disease research at [[00_Core/Paris Brain Institute\|Paris Brain Institute]]

## Data Standards
- Primary format: [[02_Standards/AnnData\|AnnData]] / h5ad (processed data)
- Raw reads: FASTQ → deposited in [[03_Platforms/NCBI GEO\|NCBI GEO]] / SRA (cross-linked)
- Cell type annotations: [[02_Standards/Cell Ontology\|Cell Ontology]] (CL) terms
- Anatomy: [[02_Standards/UBERON\|UBERON]] brain region terms
- Access: REST API and AWS S3 for large-scale data transfer

## Connections
- Funded by: [[01_Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]]
- Primary archive for: [[01_Actors/BICAN\|BICAN]] (BRAIN Initiative Cell Atlas)
- Formats: [[02_Standards/AnnData\|AnnData]] / h5ad, FASTQ (raw reads → [[03_Platforms/NCBI GEO\|NCBI GEO]])
- Annotations use: [[02_Standards/Cell Ontology\|Cell Ontology]], [[02_Standards/UBERON\|UBERON]]
- Related: [[03_Platforms/DANDI Archive\|DANDI Archive]] (electrophysiology), Brain Image Library (microscopy),
  [[03_Platforms/dbGaP\|dbGaP]] (controlled-access human genomics)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (reference cell atlas data for
  neurological disease single-cell studies; [[01_Actors/BICAN\|BICAN]] data access)

## Resources
- https://nemoarchive.org
- https://assets.nemoarchive.org (NeMO Analytics workspace)
- https://nemoarchive.org/data-access-request (controlled access request)
