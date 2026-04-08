---
{"dg-publish":true,"permalink":"/platforms/ne-mo-archive/","dg-note-properties":{"name":"NeMO Archive","aliases":["Neuroscience Multi-Omic Archive"],"website":"https://nemoarchive.org","type":"repository","scope":"international","domain":["genomics","multimodal"],"status":"active","founded":2017,"parent_org":"University of Maryland / NIH BRAIN Initiative"}}
---


# NeMO Archive — Neuroscience Multi-Omic Archive

## Overview
The NeMO Archive (Neuroscience Multi-Omic Archive) is the primary data repository for multi-omic single-cell data from the **[[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]]** and specifically the primary archive for [[Actors/BICAN\|BICAN]] (BRAIN Initiative Cell Atlas Network) datasets. Hosted at the University of Maryland Institute for Genome Sciences, NeMO stores and distributes single-cell and single-nucleus sequencing data — scRNA-seq, snRNA-seq, scATAC-seq, spatial transcriptomics, multi-omics — from human, non-human primate, and mouse brain studies.

## What NeMO Stores
- **scRNA-seq / snRNA-seq** — single-cell and single-nucleus transcriptomics of brain tissue; the primary data type; stored as [[Standards/AnnData\|AnnData]]/h5ad files
- **scATAC-seq** — chromatin accessibility at single-cell resolution
- **Spatial transcriptomics** — MERFISH, Slide-seq, Visium brain tissue maps
- **Multi-omics** — joint transcriptome + chromatin accessibility (SHARE-seq, SNARE-seq)
- **Epigenomics** — DNA methylation (snmC-seq, bisulfite sequencing)
- **Processed data** — cell type annotations, dimensionality reductions, clustering results alongside raw counts

## Access Model
NeMO operates a **tiered access model**: **open access** — processed data (cell type annotations, metadata, summary files) freely downloadable without registration; **controlled access** — raw data from human subjects requires data access request (similar to [[Platforms/dbGaP\|dbGaP]]); managed through NeMO Access portal; **NeMO Analytics** — cloud-based analysis workspace for controlled-access data (analogous to [[Platforms/VIVLI\|VIVLI]] Enclave or [[Governance/Health Data Hub\|Health Data Hub]] Datalab).

## BICAN Datasets
NeMO is the primary repository for [[Actors/BICAN\|BICAN]] data: **Human Brain Cell Atlas** — comprehensive human brain single-cell taxonomy; millions of cells across all major brain regions; **Non-human primate atlases** — macaque and marmoset brain cell atlases; **Mouse brain atlas** — continuation and expansion of BICCN mouse data; **Spatial transcriptomics** — MERFISH brain maps with cell type spatial distributions. These datasets provide the reference cell type framework for neurological disease research at [[Actors/Paris Brain Institute\|Paris Brain Institute]].

## Data Standards
- Primary format: [[Standards/AnnData\|AnnData]] / h5ad (processed data)
- Raw reads: FASTQ → deposited in [[Platforms/NCBI GEO\|NCBI GEO]] / SRA (cross-linked)
- Cell type annotations: [[Standards/Cell Ontology\|Cell Ontology]] (CL) terms
- Anatomy: [[Standards/UBERON\|UBERON]] brain region terms
- Access: REST API and AWS S3 for large-scale data transfer

## Connections
- Funded by: [[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]]
- Primary archive for: [[Actors/BICAN\|BICAN]] (BRAIN Initiative Cell Atlas)
- Formats: [[Standards/AnnData\|AnnData]] / h5ad, FASTQ (raw reads → [[Platforms/NCBI GEO\|NCBI GEO]])
- Annotations use: [[Standards/Cell Ontology\|Cell Ontology]], [[Standards/UBERON\|UBERON]]
- Related: [[Platforms/DANDI Archive\|DANDI Archive]] (electrophysiology), Brain Image Library (microscopy), [[Platforms/dbGaP\|dbGaP]] (controlled-access human genomics)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (reference cell atlas data for neurological disease single-cell studies; [[Actors/BICAN\|BICAN]] data access)

## Resources
- https://nemoarchive.org
- https://assets.nemoarchive.org (NeMO Analytics workspace)
- https://nemoarchive.org/data-access-request (controlled access request)
