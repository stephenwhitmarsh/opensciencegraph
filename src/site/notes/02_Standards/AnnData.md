---
{"dg-publish":true,"permalink":"/02-standards/ann-data/","dg-note-properties":{"name":"AnnData","aliases":["h5ad","AnnData format","Annotated Data"],"website":"https://anndata.readthedocs.io","type":"standard","scope":"international","domain":["genomics","multimodal"],"status":"active","founded":2017,"parent_org":"Theislab / Helmholtz Munich / Broad Institute"}}
---


# AnnData — Annotated Data (h5ad format)

## Overview
AnnData (Annotated Data) is the de facto standard data format and Python object
for single-cell genomics data, developed by the Theislab at Helmholtz Munich
(Fabian Theis group) and now co-maintained with the Broad Institute. The `.h5ad`
file format (HDF5-based) is the serialisation of AnnData objects, and has become
the universal exchange format for single-cell RNA-seq, single-cell ATAC-seq,
spatial transcriptomics, and multi-omics data.

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], AnnData/h5ad is the primary output format of
[[01_Actors/iGENSEQ\|iGENSEQ]]'s single-cell RNA-seq workflows (10x Genomics, Visium spatial
transcriptomics) and is directly relevant to neurological disease cell atlas
studies using [[01_Actors/BICAN\|BICAN]] reference data.

## Data Structure
An AnnData object stores a **count matrix** alongside all associated metadata:

```
AnnData object
  .X         — n_obs × n_vars matrix (cells × genes; sparse or dense)
  .obs        — cell/observation metadata DataFrame (cell type, cluster, patient ID…)
  .var        — gene/variable metadata DataFrame (gene names, IDs, highly variable…)
  .uns        — unstructured metadata dictionary (UMAP params, colour schemes…)
  .obsm       — multi-dimensional cell embeddings (UMAP, PCA, spatial coordinates)
  .varm       — multi-dimensional gene embeddings
  .obsp       — cell-cell connectivity matrices (neighbours graph)
  .layers     — additional data matrices (raw counts, normalised, log-normalised)
```

## Ecosystem: Scanpy and Scverse
AnnData is the core data structure of **Scanpy** and the broader **scverse** ecosystem:
- **Scanpy** — single-cell analysis toolkit (equivalent of Seurat for Python)
- **scverse** — umbrella organisation for interoperable single-cell Python tools:
  Scanpy, scvi-tools (deep learning), squidpy (spatial), muon (multi-omics),
  scirpy (TCR/BCR), cellrank (trajectory analysis)

## Spatial Transcriptomics
AnnData is also used for spatial transcriptomics data (10x Visium, Slide-seq,
MERFISH, Xenium):
- Spatial coordinates stored in `.obsm["spatial"]`
- High-resolution tissue image stored in `.uns["spatial"]`
- [[02_Standards/BIDS\|BIDS]] Microscopy extension (BEP031) is developing alignment with AnnData
  for BIDS-compatible spatial transcriptomics datasets

## CELLxGENE and [[01_Actors/BICAN\|BICAN]] Alignment
- **CELLxGENE Data Portal** (https://cellxgene.cziscience.com) — the largest
  public single-cell dataset collection; all datasets in h5ad format with
  standardised [[02_Standards/Cell Ontology\|Cell Ontology]] (CL) and [[02_Standards/UBERON\|UBERON]] annotations
- **[[01_Actors/BICAN\|BICAN]]** — BRAIN Initiative cell atlas data distributed in h5ad via
  NeMO Archive and AWS Open Data
- **Human Cell Atlas** — primary data exchange format is h5ad

## Connections
- Developed by: Theislab / Helmholtz Munich, Broad Institute
- Part of: scverse ecosystem (Scanpy, scvi-tools, squidpy, muon)
- Used by: [[01_Actors/BICAN\|BICAN]], CELLxGENE, Human Cell Atlas, [[01_Actors/iGENSEQ\|iGENSEQ]] workflows
- Annotations use: [[02_Standards/Cell Ontology\|Cell Ontology]] (cell types), [[02_Standards/UBERON\|UBERON]] (anatomy),
  [[02_Standards/HPO\|HPO]] / [[02_Standards/MONDO\|MONDO]] (disease context)
- Related format: [[02_Standards/NWB\|NWB]] (analogous role for electrophysiology)
- Spatial integration: [[02_Standards/BIDS\|BIDS]] Microscopy BEP031 (emerging alignment)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (scRNA-seq and spatial transcriptomics
  outputs from [[01_Actors/iGENSEQ\|iGENSEQ]]; [[01_Actors/BICAN\|BICAN]] reference data access)

## Resources
- https://anndata.readthedocs.io
- https://github.com/scverse/anndata (AnnData GitHub)
- https://scverse.org (scverse ecosystem)
- https://cellxgene.cziscience.com (CELLxGENE — largest h5ad dataset portal)
- https://scanpy.readthedocs.io (Scanpy — primary single-cell analysis toolkit)
