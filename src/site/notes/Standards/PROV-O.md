---
{"dg-publish":true,"permalink":"/standards/prov-o/","dg-note-properties":{"name":"W3C PROV Ontology","aliases":["PROV-O","PROV","W3C Provenance Ontology"],"website":"https://www.w3.org/TR/prov-o/","type":"standard","scope":"international","domain":["multimodal"],"status":"active","founded":2013,"parent_org":"W3C (World Wide Web Consortium)","icon":"https://www.w3.org/favicon.ico"}}
---


# PROV-O — W3C Provenance Ontology

## Overview
PROV-O is the W3C standard ontology for representing **provenance** — the documented history of how a piece of data was created, by whom, using what process, and from which inputs. Published as a W3C Recommendation in 2013, it provides a minimal but powerful vocabulary for recording data lineage in a machine-readable, interoperable way. PROV-O is the foundation on which [[Standards/NIDM\|NIDM]] (Neuroimaging Data Model) is built: NIDM extends PROV-O with neuroscience-specific terms to track the full computational history of a neuroimaging analysis. DataLad, the distributed data management system used by [[Platforms/OpenNeuro\|OpenNeuro]] and [[Actors/ReproNim\|ReproNim]], also generates PROV-O compatible provenance.

## Core Model
Three fundamental classes:

| Class | Description | Example |
|---|---|---|
| `prov:Entity` | A piece of data or a thing | An fMRI dataset, a statistical map |
| `prov:Activity` | A process that used or generated entities | An fMRI preprocessing pipeline |
| `prov:Agent` | A person, software, or organisation responsible | A researcher, FSL software |

Key relationships: `wasGeneratedBy`, `used`, `wasAttributedTo`, `wasDerivedFrom`, `wasAssociatedWith`

## Neuroscience Use Cases
- **[[Standards/NIDM\|NIDM]]** — extends PROV-O to describe neuroimaging experiments, results, and workflows with neuroscience-specific semantics
- **[[Actors/ReproNim\|ReproNim]]** — uses PROV-O via NIDM for reproducibility tracking in neuroimaging pipelines
- **DataLad** (used by [[Platforms/OpenNeuro\|OpenNeuro]], [[Actors/CONP\|CONP]]) — generates PROV-O compatible records for dataset version history and pipeline execution
- **[[Governance/EOSC\|EOSC]]** — EOSC data catalogues use PROV-O for provenance metadata

## Connections
- Foundation for: [[Standards/NIDM\|NIDM]] (extends PROV-O for neuroimaging)
- Used by: [[Actors/ReproNim\|ReproNim]], DataLad, [[Platforms/OpenNeuro\|OpenNeuro]], [[Governance/EOSC\|EOSC]]
- Complements: [[Standards/DCAT\|DCAT]] (dataset description), [[Standards/Dublin Core\|Dublin Core]] (basic metadata)
- Part of: W3C Semantic Web standards stack (alongside RDF, OWL, SPARQL)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (reproducible neuroimaging pipelines)

## Resources
- https://www.w3.org/TR/prov-o/
- https://www.w3.org/TR/prov-primer/ (accessible introduction)
- http://nidm.nidash.org (NIDM, built on PROV-O)
