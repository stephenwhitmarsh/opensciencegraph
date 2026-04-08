---
{"dg-publish":true,"permalink":"/02-standards/sparc-sds/","dg-note-properties":{"name":"SPARC Data Structure","aliases":["SPARC","SDS","MIS"],"website":"https://docs.sparc.science/docs/sparc-data-structure","type":"standard","scope":"international","domain":["electrophysiology","behavior","multimodal"],"status":"active","founded":2019,"parent_org":"NIH SPARC Program / SPARC Consortium"}}
---


# SPARC / SDS — SPARC Data Structure

## Overview
The SPARC Data Structure (SDS) is the data organisation standard developed by
the NIH SPARC (Stimulating Peripheral Activity to Relieve Conditions) programme
for sharing data about the peripheral nervous system, autonomic nervous system,
and organ-nerve interactions. Conceptually analogous to [[02_Standards/BIDS\|BIDS]] for neuroimaging,
SDS provides a standardised folder hierarchy and metadata schema for organising
experimental data from SPARC-funded studies — covering electrophysiology,
anatomy, connectivity mapping, imaging, and behavioural data related to
peripheral nervous system function.

SDS-formatted datasets are deposited in the **SPARC Portal** (sparc.science),
which serves as the primary open data repository for peripheral nervous system
research, analogous to [[03_Platforms/OpenNeuro\|OpenNeuro]] for central nervous system neuroimaging.

## Structure
SDS organises a dataset into a standardised hierarchy:
```
dataset/
├── dataset_description.json   ← dataset-level metadata
├── subjects.xlsx              ← subject-level metadata
├── samples.xlsx               ← sample-level metadata
├── code/                      ← analysis code
├── docs/                      ← documentation
├── primary/                   ← raw data (organised by subject/sample)
└── derivative/                ← processed data
```
Metadata is captured in standardised xlsx templates and a JSON descriptor,
with controlled vocabularies drawn from community ontologies.

## Relationship to BIDS
SDS and [[02_Standards/BIDS\|BIDS]] are complementary standards addressing different nervous system
domains:

| Feature | BIDS | SDS |
|---|---|---|
| Primary domain | Central nervous system | Peripheral nervous system |
| Key modalities | MRI, EEG, MEG, iEEG, PET | Ephys, anatomy, connectivity, imaging |
| Repository | [[03_Platforms/OpenNeuro\|OpenNeuro]] | SPARC Portal |
| Governance | [[01_Actors/INCF\|INCF]] / [[04_Governance/BIDS Steering Group\|BIDS Steering Group]] | NIH SPARC / SPARC Consortium |

Convergence efforts are underway to harmonise BIDS and SDS metadata schemas
for studies that span central and peripheral nervous systems.

## Relevance to Paris Brain Institute
SDS/SPARC is relevant to [[00_Core/Paris Brain Institute\|Paris Brain Institute]] through:
- Peripheral nervous system research programmes (autonomic neurology,
  enteric nervous system)
- Electrophysiology data from ePHYS platform that includes peripheral nerve recordings
- Cross-domain studies combining CNS ([[02_Standards/BIDS\|BIDS]]) and PNS (SDS) data

## Connections
- Analogous to: [[02_Standards/BIDS\|BIDS]] (CNS equivalent)
- Repository: SPARC Portal (https://sparc.science)
- Funded by: NIH SPARC Programme (Office of Strategic Coordination)
- Governance: SPARC Consortium / MIS (Map Core)
- Standards used within SDS: [[02_Standards/NWB\|NWB]] (electrophysiology data files),
  community anatomy ontologies
- Harmonisation effort: BIDS-SPARC convergence working group
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (peripheral neuroscience, ePHYS platform)

## Resources
- https://sparc.science (SPARC Portal — dataset repository)
- https://docs.sparc.science/docs/sparc-data-structure (SDS specification)
- https://github.com/SciCrunch/sparc-curation (SDS tooling)
