---
{"dg-publish":true,"permalink":"/02-standards/obi/","dg-note-properties":{"name":"Ontology for Biomedical Investigations","aliases":["OBI"],"website":"https://obi-ontology.org","type":"terminology","scope":"international","domain":["clinical","multimodal"],"status":"active","founded":2007,"parent_org":"OBO Foundry"}}
---


# OBI — Ontology for Biomedical Investigations

## Overview
OBI is an OBO Foundry ontology covering the full lifecycle of biomedical
experiments: study design, protocols, instruments, assays, data collection,
and conclusions. It provides a machine-readable vocabulary for formally
describing *how* a scientific investigation was conducted — the experimental
design, what was measured with what instrument, how samples were collected,
and what statistical methods were applied. OBI is part of the OBO Foundry
ecosystem alongside [[02_Standards/HPO\|HPO]], [[02_Standards/UBERON\|UBERON]], and [[02_Standards/MONDO\|MONDO]], and integrates with
[[02_Standards/BIDS\|BIDS]] via its extensions for study-level metadata.

## Neuroscience Relevance
For [[00_Core/Paris Brain Institute\|Paris Brain Institute]], OBI is relevant for:
- **Formally describing MRI acquisition protocols** — scanner model, field strength,
  sequence parameters — in a machine-readable way for data sharing
- **Cognitive task descriptions** — linking to [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] terms via OBI
  assay concepts
- **Biomarker assay protocols** — CSF collection, immunoassay protocols for
  amyloid, tau, NfL measurements
- **FAIR data publication** — journals and repositories increasingly require
  structured protocol descriptions; OBI provides the vocabulary

## Key OBI Concepts
- `OBI:0000070` — assay (measurement process)
- `OBI:0000272` — protocol
- `OBI:0100026` — organism (subject in a study)
- `OBI:0000067` — data transformation
- `OBI:0000299` — datum (a piece of data)

## Connections
- Part of: OBO Foundry (with [[02_Standards/HPO\|HPO]], [[02_Standards/UBERON\|UBERON]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]])
- Integrates with: [[02_Standards/BIDS\|BIDS]] (protocol metadata extensions)
- Complements: [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] (cognitive tasks), [[02_Standards/UBERON\|UBERON]] (anatomy)
- Used in: biobank metadata ([[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]]), [[04_Governance/FAIR Principles\|FAIR Principles]] R1.3 compliance
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (study protocol description)

## Resources
- https://obi-ontology.org
- https://obofoundry.org/ontology/obi.html
- https://www.ebi.ac.uk/ols/ontologies/obi (EBI Ontology Lookup Service)
