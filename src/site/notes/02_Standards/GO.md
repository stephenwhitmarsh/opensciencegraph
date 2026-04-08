---
{"dg-publish":true,"permalink":"/02-standards/go/","dg-note-properties":{"name":"Gene Ontology","aliases":["GO","Gene Ontology Consortium"],"website":"https://geneontology.org","type":"terminology","scope":"international","domain":["genomics","multimodal"],"status":"active","founded":1998,"parent_org":"Gene Ontology Consortium"}}
---


# GO — Gene Ontology

## Overview
The Gene Ontology is the world's largest source of information on the functions of genes and gene products. Developed by the Gene Ontology Consortium since 1998, GO provides a structured, precisely defined, common controlled vocabulary for describing gene product attributes across all organisms. It is organised into three independent ontologies: **Biological Process** (BP), **Molecular Function** (MF), and **Cellular Component** (CC). GO terms are used to annotate gene products in databases worldwide, enabling systematic, cross-species functional analysis of genomic and transcriptomic data.

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], GO is directly relevant to neurogenomics and transcriptomics analyses — RNA-seq and single-cell RNA-seq pipelines at [[01_Actors/iGENSEQ\|iGENSEQ]] produce gene expression data that is interpreted using GO term enrichment analysis.

## Three Ontology Domains

### Biological Process (BP)
The larger processes accomplished by multiple molecular activities. Examples: synaptic transmission, myelination, DNA repair, axon guidance, apoptosis.

### Molecular Function (MF)
The biochemical activities of gene products. Examples: kinase activity, ion channel activity, RNA binding, receptor signalling.

### Cellular Component (CC)
The locations where a gene product is active. Examples: synapse, mitochondrion, nucleus, plasma membrane, extracellular space.

## Usage in Neuroscience
- **Transcriptomics** — GO enrichment analysis (GSEA, ORA) identifies biological processes dysregulated in neurological disease conditions
- **Single-cell RNA-seq** — cell type annotation and cluster functional characterisation using GO terms
- **Comparative genomics** — cross-species functional comparison using GO annotations from model organisms (mouse, zebrafish, Drosophila)
- **Drug target identification** — GO MF terms identify molecular pathways for therapeutic intervention

## Integration with Other Standards
- [[02_Standards/OMOP CDM\|OMOP CDM]] — GO terms used in pharmacogenomics and biomarker modules
- [[02_Standards/Phenopackets\|Phenopackets]] / [[02_Standards/HPO\|HPO]] — GO (gene function) complements HPO (phenotype) in rare disease genomics workflows
- [[02_Standards/VCF\|VCF]] — variant functional annotation pipelines (e.g. Ensembl VEP) map variants to GO terms via affected genes

## Connections
- Produced by: Gene Ontology Consortium (founding members include EBI, ZFIN, MGI, FlyBase, SGD, WormBase)
- Hosted at: EBI (QuickGO browser), Gene Ontology Consortium (AmiGO browser)
- Used by: [[04_Governance/IFB\|IFB]] (bioinformatics pipelines), [[01_Actors/iGENSEQ\|iGENSEQ]] (RNA-seq analysis)
- Complements: [[02_Standards/HPO\|HPO]] (phenotype), [[02_Standards/MONDO\|MONDO]] (disease), [[02_Standards/ChEBI\|ChEBI]] (chemical entities)
- Part of: OBO Foundry (https://obofoundry.org)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (neurogenomics, transcriptomics)

## Resources
- https://geneontology.org
- https://amigo.geneontology.org (AmiGO browser)
- https://www.ebi.ac.uk/QuickGO (QuickGO browser, EBI)
- https://obofoundry.org/ontology/go.html (OBO Foundry entry)
