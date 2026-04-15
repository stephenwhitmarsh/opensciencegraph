---
{"dg-publish":true,"permalink":"/standards/open-minds/","dg-note-properties":{"name":"Open Metadata Initiative for Neuroscience Data Structures","aliases":["openMINDS"],"website":"https://openminds.ebrains.eu","type":"framework","scope":"european","domain":["neuroimaging","multimodal"],"status":"active","founded":2020,"parent_org":"EBRAINS / Human Brain Project","tags":null,"icon":"https://openminds.ebrains.eu/favicon.ico"}}
---


# openMINDS — Open Metadata Initiative for Neuroscience Data Structures

## Overview
openMINDS is the metadata framework developed by [[Platforms/EBRAINS\|EBRAINS]] for describing neuroscience research products — datasets, models, software, and workflows — with rich, FAIR-compliant, machine-readable schemas. It is the metadata infrastructure that powers EBRAINS Data and Knowledge: every dataset, model, and software tool shared on the EBRAINS platform is described using openMINDS schemas. Institutions depositing data on EBRAINS use openMINDS schemas as part of the curation process.

## Schema Collections
openMINDS is organised into domain-specific schema collections:

- **core** — fundamental research product metadata: datasets, persons, organisations, licenses, protocols, subjects, specimens, digital identifiers
- **SANDS** (Spatial Anchoring in Neuroscience Data Structures) — spatial anchoring of data to brain atlases; uses [[Standards/UBERON\|UBERON]] for cross-species region terms and maps to specific atlas versions (Allen CCF, BigBrain, MNI)
- **computation** — computational models, simulations, workflows; relevant for EBRAINS neuromorphic computing and modelling datasets
- **controlled terms** — the controlled vocabulary library for openMINDS, covering brain regions, species, techniques, licenses, etc.

## FAIR Integration
openMINDS schemas are designed to fulfil the FAIR principles:
- **F** — every dataset gets a persistent identifier via EBRAINS Knowledge Graph
- **A** — metadata retrievable via EBRAINS Knowledge Graph API
- **I** — uses [[Standards/UBERON\|UBERON]], [[Standards/BIDS\|BIDS]] conventions, and linked data (JSON-LD)
- **R** — rich provenance including protocols, subjects, techniques, licenses

## Connections
- Required for: [[Platforms/EBRAINS\|EBRAINS]] data and model sharing
- Uses: [[Standards/UBERON\|UBERON]] (brain region annotation), [[Standards/BIDS\|BIDS]] (dataset organisation), [[Standards/NWB\|NWB]] (electrophysiology data format)
- Complements: [[Standards/REMBI\|REMBI]] (microscopy metadata), [[Standards/BIDS\|BIDS]] (neuroimaging organisation)
- Relevant to: [[Platforms/EBRAINS\|EBRAINS]] member institutions, [[Actors/Donders Institute\|Donders Institute]], [[Governance/Human Brain Project\|Human Brain Project]]

## Resources
- https://openminds.ebrains.eu
- https://github.com/HumanBrainProject/openMINDS (GitHub repository)
- https://kg.ebrains.eu (EBRAINS Knowledge Graph, powered by openMINDS)
