---
{"dg-publish":true,"permalink":"/02-standards/nidm/","dg-note-properties":{"name":"Neuroimaging Data Model","aliases":["NIDM","NIDM-Experiment","NIDM-Results"],"website":"http://nidm.nidash.org","type":"standard","scope":"international","domain":["neuroimaging"],"status":"active","founded":2013,"parent_org":"ReproNim / INCF"}}
---


# NIDM — Neuroimaging Data Model

## Overview
NIDM (Neuroimaging Data Model) is a W3C PROV-based semantic data model for representing neuroimaging experiments, statistical results, and analysis provenance. Developed within the [[01_Actors/ReproNim\|ReproNim]] ecosystem and the NIDASH working group under [[01_Actors/INCF\|INCF]], NIDM provides a machine-readable, graph-based representation of the full neuroimaging research workflow — from subject characteristics and acquisition parameters through to analysis pipelines and final statistical maps. Its goal is to enable automated result discovery, cross-study comparison, and reproducibility verification across neuroimaging datasets.

NIDM extends [[02_Standards/BIDS\|BIDS]] at the semantic layer: while BIDS organises the file structure of a dataset, NIDM describes the *meaning* of that data and the provenance of how results were derived from it, using the W3C [[02_Standards/PROV-O\|PROV-O]] ontology as its formal foundation.

## Three Components

### NIDM-Experiment
Describes the experimental design and dataset metadata in a machine-readable graph:
- Subject demographics (age, sex, diagnosis — using [[02_Standards/SNOMED CT\|SNOMED CT]] / [[02_Standards/HPO\|HPO]] terms)
- Acquisition parameters (MRI scanner, sequence — linking to [[02_Standards/DICOM\|DICOM]] metadata)
- Study design (tasks, stimuli — linking to [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] terms)
- Links to [[02_Standards/BIDS\|BIDS]] dataset files via persistent identifiers

NIDM-Experiment files are typically stored as `.ttl` (Turtle RDF) alongside a BIDS dataset and enable federated queries across multiple studies — the foundation for tools like the NIDM Query Tool used in multi-site neuroimaging meta-analyses.

### NIDM-Results
Packages neuroimaging statistical analysis results with complete provenance:
- Statistical maps (z-scores, t-scores, p-values) as [[02_Standards/NIfTI\|NIfTI]] files with metadata
- Complete description of the analysis pipeline (software, parameters, contrasts)
- Provenance chain from raw data to results using [[02_Standards/PROV-O\|PROV-O]] Activity/Entity/Agent model
- Export format supported by FSL, SPM, and AFNI — the three major neuroimaging analysis packages

NIDM-Results files are accepted by [[03_Platforms/NeuroVault\|NeuroVault]] for open sharing of statistical maps with full methodological context, directly enabling reproducibility and meta-analysis.

### NIDM-Workflow (emerging)
Captures complete analysis pipeline provenance using workflow description standards, linking to containerised pipeline definitions (Boutiques, BIDS Apps) to enable full re-execution.

## Tools and Ecosystem
- **PyNIDM** — Python library for creating, querying, and manipulating NIDM documents
- **NIDM-Terms** — shared vocabulary for common neuroimaging data elements (demographics, acquisition parameters) maintained by [[01_Actors/ReproNim\|ReproNim]]
- **ReproIn** — [[02_Standards/BIDS\|BIDS]]-compatible MRI acquisition naming convention that feeds into automated NIDM-Experiment generation
- **NIDM Query Tool** — SPARQL-based federated query tool for searching across NIDM-annotated datasets from multiple sites

## Current Adoption Status
NIDM-Results is production-ready and actively used: [[03_Platforms/NeuroVault\|NeuroVault]] accepts NIDM-Results packages for statistical map deposit; FSL, SPM, AFNI all export NIDM-Results natively or via plugins; used in [[01_Actors/ReproNim\|ReproNim]] / [[01_Actors/INCF\|INCF]] training programmes. NIDM-Experiment is in active development: used in [[01_Actors/CONP\|CONP]] (Canadian Open Neuroscience Platform) for dataset annotation; integrated into [[03_Platforms/OpenNeuro\|OpenNeuro]] metadata pipeline (partial); basis for federated cohort discovery alongside [[03_Platforms/Neurobagel\|Neurobagel]].

## Connections
- Extends: [[02_Standards/BIDS\|BIDS]] (semantic layer on top of BIDS file organisation)
- Built on: [[02_Standards/PROV-O\|PROV-O]] (W3C Provenance Ontology — NIDM extends PROV-O for neuroimaging)
- Endorsed by: [[01_Actors/INCF\|INCF]] (via NIDASH working group)
- Used in: [[01_Actors/ReproNim\|ReproNim]], [[03_Platforms/NeuroVault\|NeuroVault]] (NIDM-Results), [[01_Actors/CONP\|CONP]] (NIDM-Experiment)
- Vocabularies: [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] (task terms), [[02_Standards/SNOMED CT\|SNOMED CT]] / [[02_Standards/HPO\|HPO]] (subject terms), [[02_Standards/UBERON\|UBERON]] (anatomy), [[02_Standards/DICOM\|DICOM]] (acquisition metadata)
- Tools: PyNIDM, ReproIn, NIDM Query Tool
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (reproducibility, statistical result sharing via [[03_Platforms/NeuroVault\|NeuroVault]], multi-site cohort annotation)

## Resources
- http://nidm.nidash.org
- https://github.com/incf-nidash/PyNIDM (PyNIDM library)
- https://github.com/NIDM-Experiment (NIDM-Experiment specification)
- https://www.repronim.org/reproschema.html (ReproNim schema tools)
