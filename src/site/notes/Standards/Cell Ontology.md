---
{"dg-publish":true,"permalink":"/standards/cell-ontology/","dg-note-properties":{"name":"Cell Ontology","aliases":["CL","Cell Ontology CL"],"website":"https://cell-ontology.github.io","type":"terminology","scope":"international","domain":["genomics","multimodal"],"status":"active","founded":2004,"parent_org":"OBO Foundry"}}
---


# Cell Ontology (CL)

## Overview
The Cell Ontology (CL) is the OBO Foundry standard ontology for describing cell types across all organisms. It provides a controlled, hierarchically organised vocabulary of ~2,500 cell type terms covering the full range of cell types found in multicellular organisms — from broad categories (neuron, glial cell, immune cell) to highly specific subtypes (parvalbumin-positive interneuron, dopaminergic neuron of the substantia nigra pars compacta).

With the explosion of single-cell RNA-sequencing ([[Actors/iGENSEQ\|iGENSEQ]]), spatial transcriptomics, and brain cell atlas projects ([[Actors/BICAN\|BICAN]], [[Actors/Human Brain Project\|Human Brain Project]]), CL has become critically important for annotating cell type identities in single-cell datasets — providing the controlled vocabulary that enables cross-study comparison, meta-analysis, and machine-readable cell type annotations.

## Neuroscience-Relevant Cell Types
CL contains a rich hierarchy of neural and glial cell types:
- **Neurons** — excitatory, inhibitory, dopaminergic, serotonergic, cholinergic, glutamatergic, GABAergic
- **Interneurons** — parvalbumin+, somatostatin+, VIP+, chandelier cells
- **Astrocytes** — fibrous, protoplasmic; reactive subtypes
- **Oligodendrocytes** — mature myelinating, oligodendrocyte precursor cells (OPCs)
- **Microglia** — homeostatic, activated, disease-associated (DAM)
- **Ependymal cells**, **radial glia**, **neural stem cells**
- **Vascular cells** — endothelial cells, pericytes, smooth muscle cells

## Integration with Single-Cell Workflows
CL is the standard vocabulary for cell type annotation in single-cell data:
- **AnnData** / h5ad files — CL terms stored in `.obs` metadata for cell type labels
- **CELLxGENE** (CZI) — requires CL terms for all cell type annotations in the CELLxGENE Data Portal (largest single-cell human data collection)
- **[[Actors/BICAN\|BICAN]]** cell atlas — uses CL for all annotated cell types in the mammalian brain atlas
- **[[Actors/Human Brain Project\|Human Brain Project]]** — brain cell types in EBRAINS data linked to CL
- **Allen Brain Cell Atlas** — cell types mapped to CL identifiers

## OBO Foundry Integration
CL is part of the OBO Foundry and integrates with other OBO ontologies:
- **[[Standards/UBERON\|UBERON]]** — anatomical location of cell types (e.g. neuron OF the cerebral cortex)
- **[[Standards/GO\|GO]]** — biological processes carried out by cell types
- **[[Standards/HPO\|HPO]]** — cell type changes as phenotypic features (e.g. loss of dopaminergic neurons)
- **[[Standards/MONDO\|MONDO]]** — cell type involvement in diseases

## Connections
- Part of: OBO Foundry (with [[Standards/HPO\|HPO]], [[Standards/UBERON\|UBERON]], [[Standards/MONDO\|MONDO]], [[Standards/GO\|GO]])
- Used by: [[Actors/BICAN\|BICAN]] (brain cell atlas), CELLxGENE (CZI data portal)
- Integrates with: [[Standards/UBERON\|UBERON]] (anatomy), [[Standards/GO\|GO]] (function), [[Standards/HPO\|HPO]] (phenotypes)
- Format: OWL and OBO; terms identified as `CL:XXXXXXX`
- Used in: AnnData/h5ad single-cell data, EBRAINS data deposits
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (single-cell RNA-seq annotation at [[Actors/iGENSEQ\|iGENSEQ]]; neurological disease cell type characterisation)

## Resources
- https://cell-ontology.github.io
- https://obofoundry.org/ontology/cl.html (OBO Foundry CL page)
- https://www.ebi.ac.uk/ols/ontologies/cl (EBI Ontology Lookup Service)
- https://cellxgene.cziscience.com (CELLxGENE — requires CL annotations)
