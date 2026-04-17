---
{"dg-publish":true,"permalink":"/platforms/neurobagel/","dg-note-properties":{"name":"Neurobagel","aliases":["Nipoppy"],"website":"https://neurobagel.org","type":"platform","scope":"international","domain":["neuroimaging","clinical","multimodal"],"status":"active","founded":2021,"parent_org":"McGill University / CONP / ReproNim"}}
---


# Neurobagel

## Overview
Neurobagel is an open-source ecosystem of tools for federated neuroscience cohort discovery across decentralised BIDS datasets. Developed at McGill University in collaboration with [[Actors/CONP\|CONP]] and [[Actors/ReproNim\|ReproNim]], it enables participant-level cohort search across multiple institutions simultaneously — without centralising data or requiring data transfer. Each participating institution deploys a local Neurobagel node; the federation API aggregates query results across all nodes while data files remain under local custody and governance.

Neurobagel complements [[Platforms/OpenNeuro\|OpenNeuro]] (which centralises open datasets) by providing federated search across both open and restricted datasets, including controlled-access clinical cohorts that cannot be centralised. It is particularly relevant for multi-site clinical neuroimaging studies like those coordinated by [[Actors/CATI\|CATI]].

## Architecture
Neurobagel uses a **hub-and-spoke federated model**: each institution deploys a **Neurobagel node** (containerised, self-hosted) containing a knowledge graph of harmonised participant-level metadata; the **federation API** (federate.neurobagel.org) aggregates queries across all public nodes simultaneously; the **query tool** (query.neurobagel.org) provides a web interface for defining cohort criteria and retrieving matching participant lists.

## Data Model and Standards
- Phenotypic data annotated using [[Standards/BIDS\|BIDS]] conventions and [[Standards/NIDM\|NIDM]] terms
- Controlled vocabularies: [[Standards/SNOMED CT\|SNOMED CT]] (diagnosis), age/sex standardisation, imaging modality from BIDS
- Linked data / semantic web representation (JSON-LD, knowledge graphs)
- DataLad backend for imaging data download from participating nodes

## Public Nodes (as of 2025)
- **OpenNeuro** — growing subset of OpenNeuro datasets annotated by community
- **INDI** — International Neuroimaging Data-sharing Initiative datasets
- **Quebec Parkinson Network** — federated access (discovery only, no download)
- **ENIGMA-Parkinson's WG** — pilot deployment across 4 Dutch sites (2025)

## Companion Tool: Nipoppy
Nipoppy is a Python package that extends [[Standards/BIDS\|BIDS]] for managing neuroimaging pipeline tracking and curation. It standardises the management and monitoring of neuroimaging data processing workflows, producing Neurobagel-ready metadata as output. The Neurobagel+Nipoppy stack provides a complete pipeline from raw data curation to federated discovery.

## Connections
- Built on: [[Standards/BIDS\|BIDS]], [[Standards/NIDM\|NIDM]], DataLad
- Vocabularies: [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/HPO\|HPO]] (diagnosis annotation)
- Complements: [[Platforms/OpenNeuro\|OpenNeuro]] (centralised open data), [[Platforms/LORIS\|LORIS]] (site-level data management)
- Developed by: McGill / [[Actors/CONP\|CONP]] / [[Actors/ReproNim\|ReproNim]]
- Deployed at: [[Actors/ENIGMA Consortium\|ENIGMA Consortium]] Parkinson's WG, Ontario Brain Institute, others
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (multi-site BIDS cohort discovery, CATI-managed datasets)

## Resources
- https://neurobagel.org
- https://query.neurobagel.org (public query tool)
- https://github.com/neurobagel (source code)
- https://neurobagel.org/nipoppy/overview/ (Nipoppy documentation)
