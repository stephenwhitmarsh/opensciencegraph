---
{"dg-publish":true,"permalink":"/platforms/ebrains/","tags":["icm/participates"],"dg-note-properties":{"name":"EBRAINS","aliases":["EBRAINS Research Infrastructure"],"website":"https://ebrains.eu","type":"infrastructure","scope":"european","domain":["neuroimaging","multimodal"],"status":"active","founded":2020,"parent_org":"Human Brain Project / EU Horizon","tags":["icm/participates"],"icon":"https://ebrains.eu/favicon.ico"}}
---


# EBRAINS

## Overview
EBRAINS is the open neuroscience research infrastructure created by the [[Governance/Human Brain Project\|Human Brain Project]] (HBP) and launched as an independent infrastructure in 2020. It is the central European hub for brain data sharing, brain atlas services, simulation, and HPC for neuroscience, integrated into [[Governance/EOSC\|EOSC]] as a key service provider. [[Actors/Paris Brain Institute\|Paris Brain Institute]] is a participating institution, contributing data and using EBRAINS services for data sharing and computational neuroscience.

EBRAINS is currently on the path to becoming an **ERIC** (European Research Infrastructure Consortium), which will give it permanent legal and funding status comparable to [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/ELIXIR\|ELIXIR]], and [[Governance/EATRIS\|EATRIS]].

## Key Services

### EBRAINS Data and Knowledge
- **Dataset sharing** — FAIR dataset deposit using [[Standards/openMINDS\|openMINDS]] metadata framework; datasets receive DOIs and are discoverable via the EBRAINS Knowledge Graph
- **openMINDS** ([[Standards/openMINDS\|openMINDS]]) — the required metadata framework for EBRAINS data; describes experimental metadata, data provenance, file formats, and linked entities
- Supports [[Standards/BIDS\|BIDS]] (neuroimaging) and [[Standards/NWB\|NWB]] (neurophysiology) datasets alongside custom modalities
- **EBRAINS Knowledge Graph** — semantic graph database linking datasets, models, software, publications, and researchers; queryable via API

### Brain Atlases
- **Human Brain Atlas** — multi-scale probabilistic atlas of the human brain; includes the Julich Brain Atlas (cytoarchitectonic maps of 200+ brain areas)
- **Mouse Brain Atlas** — Allen Common Coordinate Framework integration
- **Multi-species atlases** — rat, macaque, and other species
- Brain region annotations use [[Standards/UBERON\|UBERON]] for cross-species interoperability
- **Interactive Atlas Viewer** — web-based 3D brain atlas viewer

### Simulation and HPC
- **Neuromorphic Computing** — SpiNNaker (Manchester) and BrainScaleS (Heidelberg) neuromorphic hardware platforms for energy-efficient neural simulation
- **HPC access** — FENIX Research Infrastructure connects EBRAINS to European Tier-0/Tier-1 supercomputing centres (CSCS, JSC, CINECA)
- **NEST, NEURON, TVB** — simulation engines available via EBRAINS Lab

### Live Papers
**Live Papers** — interactive, reproducible scientific publications that embed data, code, and simulations directly in the paper; readers can re-execute analyses; built on EBRAINS infrastructure.

## EBRAINS and EOSC
EBRAINS is one of the flagship neuroscience services within [[Governance/EOSC\|EOSC]]: EBRAINS datasets and services are discoverable via the EOSC Portal; openMINDS metadata is harvested by [[Governance/OpenAIRE\|OpenAIRE]] for EU open science monitoring; EBRAINS is a model for domain-specific EOSC service integration.

## Connections
- Created by: [[Governance/Human Brain Project\|Human Brain Project]]
- Part of: [[Governance/EOSC\|EOSC]] (key service provider)
- Standards: [[Standards/BIDS\|BIDS]], [[Standards/NWB\|NWB]], [[Standards/openMINDS\|openMINDS]] (required metadata), [[Standards/UBERON\|UBERON]]
- Partners: [[Actors/INCF\|INCF]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/ECRIN\|ECRIN]], [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Actors/Donders Institute\|Donders Institute]], [[Actors/GA4GH\|GA4GH]]
- Atlases: Julich Brain Atlas, Allen CCF ([[Standards/UBERON\|UBERON]] annotation)
- Simulation: SpiNNaker, BrainScaleS, NEST, NEURON
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (ICM participates; data sharing; atlas-linked research; [[Standards/openMINDS\|openMINDS]] metadata for BIDS/NWB datasets)

## Resources
- https://ebrains.eu
- https://openminds.ebrains.eu ([[Standards/openMINDS\|openMINDS]] metadata framework)
- https://ebrains.eu/services/data-and-knowledge (data sharing services)
- https://interactive-viewer.apps.ebrains.eu (Interactive Atlas Viewer)
- https://ebrains.eu/services/live-papers (Live Papers)
