---
{"dg-publish":true,"permalink":"/standards/nidm/","dg-note-properties":{"name":"Neuroimaging Data Model","aliases":["NIDM","NIDM-Experiment","NIDM-Results"],"website":"http://nidm.nidash.org","type":"standard","scope":"international","domain":["neuroimaging"],"status":"active","founded":2013,"parent_org":"ReproNim / INCF"}}
---


# NIDM — Neuroimaging Data Model

## Overview
NIDM (Neuroimaging Data Model) is a W3C PROV-based semantic data model for
representing neuroimaging experiments, statistical results, and analysis provenance.
Developed within the [[Actors/ReproNim\|ReproNim]] ecosystem and the NIDASH working group under
[[Actors/INCF\|INCF]], NIDM provides a machine-readable, graph-based representation of the
full neuroimaging research workflow — from subject characteristics and acquisition
parameters through to analysis pipelines and final statistical maps. Its goal is
to enable automated result discovery, cross-study comparison, and reproducibility
verification across neuroimaging datasets.

NIDM extends [[Standards/BIDS\|BIDS]] at the semantic layer: while BIDS organises the file structure
of a dataset, NIDM describes the *meaning* of that data and the provenance of how
results were derived from it, using the W3C [[Standards/PROV-O\|PROV-O]] ontology as its formal
foundation.

## Three Components

### NIDM-Experiment
Describes the experimental design and dataset metadata in a machine-readable graph:
- Subject demographics (age, sex, diagnosis — using [[Standards/SNOMED CT\|SNOMED CT]] / [[Standards/HPO\|HPO]] terms)
- Acquisition parameters (MRI scanner, sequence — linking to [[Standards/DICOM\|DICOM]] metadata)
- Study design (tasks, stimuli — linking to [[Standards/Cognitive Atlas\|Cognitive Atlas]] terms)
- Links to [[Standards/BIDS\|BIDS]] dataset files via persistent identifiers

NIDM-Experiment files are typically stored as `.ttl` (Turtle RDF) alongside a
BIDS dataset and enable federated queries across multiple studies — the foundation
for tools like the NIDM Query Tool used in multi-site neuroimaging meta-analyses.

### NIDM-Results
Packages neuroimaging statistical analysis results with complete provenance:
- Statistical maps (z-scores, t-scores, p-values) as [[Standards/NIfTI\|NIfTI]] files with metadata
- Complete description of the analysis pipeline (software, parameters, contrasts)
- Provenance chain from raw data to results using [[Standards/PROV-O\|PROV-O]] Activity/Entity/Agent model
- Export format supported by FSL, SPM, and AFNI — the three major neuroimaging
  analysis packages

NIDM-Results files are accepted by [[Platforms/NeuroVault\|NeuroVault]] for open sharing of statistical
maps with full methodological context, directly enabling reproducibility and
meta-analysis.

### NIDM-Workflow (emerging)
Captures complete analysis pipeline provenance using workflow description standards,
linking to containerised pipeline definitions (Boutiques, BIDS Apps) to enable
full re-execution.

## Tools and Ecosystem
- **PyNIDM** — Python library for creating, querying, and manipulating NIDM documents
- **NIDM-Terms** — shared vocabulary for common neuroimaging data elements
  (demographics, acquisition parameters) maintained by [[Actors/ReproNim\|ReproNim]]
- **ReproIn** — [[Standards/BIDS\|BIDS]]-compatible MRI acquisition naming convention that feeds
  into automated NIDM-Experiment generation
- **NIDM Query Tool** — SPARQL-based federated query tool for searching across
  NIDM-annotated datasets from multiple sites

## Current Adoption Status
NIDM-Results is production-ready and actively used:
- [[Platforms/NeuroVault\|NeuroVault]] accepts NIDM-Results packages for statistical map deposit
- FSL, SPM, AFNI all export NIDM-Results natively or via plugins
- Used in [[Actors/ReproNim\|ReproNim]] / [[Actors/INCF\|INCF]] training programmes

NIDM-Experiment is in active development and community adoption:
- Used in [[Actors/CONP\|CONP]] (Canadian Open Neuroscience Platform) for dataset annotation
- Integrated into [[Platforms/OpenNeuro\|OpenNeuro]] metadata pipeline (partial)
- Basis for federated cohort discovery alongside [[Platforms/Neurobagel\|Neurobagel]]

## Connections
- Extends: [[Standards/BIDS\|BIDS]] (semantic layer on top of BIDS file organisation)
- Built on: [[Standards/PROV-O\|PROV-O]] (W3C Provenance Ontology — NIDM extends PROV-O for neuroimaging)
- Endorsed by: [[Actors/INCF\|INCF]] (via NIDASH working group)
- Used in: [[Actors/ReproNim\|ReproNim]], [[Platforms/NeuroVault\|NeuroVault]] (NIDM-Results), [[Actors/CONP\|CONP]] (NIDM-Experiment)
- Vocabularies: [[Standards/Cognitive Atlas\|Cognitive Atlas]] (task terms), [[Standards/SNOMED CT\|SNOMED CT]] / [[Standards/HPO\|HPO]] (subject terms),
  [[Standards/UBERON\|UBERON]] (anatomy), [[Standards/DICOM\|DICOM]] (acquisition metadata)
- Tools: PyNIDM, ReproIn, NIDM Query Tool
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (reproducibility, statistical result sharing
  via [[Platforms/NeuroVault\|NeuroVault]], multi-site cohort annotation)

## Resources
- http://nidm.nidash.org
- https://github.com/incf-nidash/PyNIDM (PyNIDM library)
- https://github.com/NIDM-Experiment (NIDM-Experiment specification)
- https://www.repronim.org/reproschema.html (ReproNim schema tools)
