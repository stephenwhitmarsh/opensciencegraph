---
{"dg-publish":true,"permalink":"/standards/uberon/","tags":["icm/uses"],"dg-note-properties":{"name":"Uber Anatomy Ontology","aliases":["UBERON"],"website":"https://uberon.org","type":"terminology","scope":"international","domain":["neuroimaging","multimodal"],"status":"active","founded":2010,"parent_org":"OBO Foundry / Monarch Initiative","tags":["icm/uses"]}}
---


# UBERON — Uber Anatomy Ontology

## Overview
UBERON is a cross-species integrated anatomy ontology covering body parts, organs, tissues, and anatomical structures from multiple organisms. It is the standard for anatomical annotation in the OBO Foundry ecosystem and is deeply relevant to neuroscience because of its detailed **brain region coverage**: UBERON provides species-neutral terms that bridge mouse brain atlas regions (Allen Mouse Brain Atlas) with human neuroimaging parcellations, enabling cross-species comparisons. This is exactly the role it plays on [[Platforms/EBRAINS\|EBRAINS]] — annotating datasets from mouse electrophysiology and human MRI with a common anatomical vocabulary.

## Neuroscience Relevance
- **Cross-species brain region terms** — e.g. UBERON:0001384 (primary motor cortex) applies to both rodent and human data, enabling comparison
- **Bridges atlas systems** — links Allen Brain Atlas CCF regions, human MNI parcellations (AAL, Brodmann areas), and primate brain regions
- **NWB integration** — [[Standards/NWB\|NWB]] uses UBERON for brain region annotation in electrophysiology datasets
- **EBRAINS** — [[Platforms/EBRAINS\|EBRAINS]] openMINDS schemas use UBERON for brain region annotation in multimodal neuroscience datasets
- **IBL** — the Brain Wide Map uses UBERON-aligned region definitions

## Key Brain Structure Examples
| UBERON ID | Structure |
|---|---|
| UBERON:0001384 | Primary motor cortex |
| UBERON:0002298 | Brodmann area (generic) |
| UBERON:0001876 | Amygdala |
| UBERON:0002421 | Hippocampal formation |
| UBERON:0000955 | Brain |
| UBERON:0001133 | Cerebral cortex |

## Connections
- Used in: [[Platforms/EBRAINS\|EBRAINS]] (openMINDS schemas), [[Standards/NWB\|NWB]] (brain region annotation), [[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]] (Atlas alignment)
- Complements: [[Standards/Cognitive Atlas\|Cognitive Atlas]] (cognitive processes), [[Standards/HED\|HED]] (events)
- Part of: OBO Foundry (alongside [[Standards/HPO\|HPO]], [[Standards/MONDO\|MONDO]], [[Standards/ORDO\|ORDO]])
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Actors/IBL\|IBL]], [[Actors/Human Connectome Project\|Human Connectome Project]]

## Resources
- https://uberon.org
- https://obofoundry.org/ontology/uberon.html
- https://www.ebi.ac.uk/ols/ontologies/uberon (EBI Ontology Lookup Service)
