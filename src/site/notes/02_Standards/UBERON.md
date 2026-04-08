---
{"dg-publish":true,"permalink":"/02-standards/uberon/","tags":["icm/uses"],"dg-note-properties":{"name":"Uber Anatomy Ontology","aliases":["UBERON"],"website":"https://uberon.org","type":"terminology","scope":"international","domain":["neuroimaging","multimodal"],"status":"active","founded":2010,"parent_org":"OBO Foundry / Monarch Initiative","tags":["icm/uses"]}}
---


# UBERON — Uber Anatomy Ontology

## Overview
UBERON is a cross-species integrated anatomy ontology covering body parts, organs, tissues, and anatomical structures from multiple organisms. It is the standard for anatomical annotation in the OBO Foundry ecosystem and is deeply relevant to neuroscience because of its detailed **brain region coverage**: UBERON provides species-neutral terms that bridge mouse brain atlas regions (Allen Mouse Brain Atlas) with human neuroimaging parcellations, enabling cross-species comparisons. This is exactly the role it plays on [[03_Platforms/EBRAINS\|EBRAINS]] — annotating datasets from mouse electrophysiology and human MRI with a common anatomical vocabulary.

## Neuroscience Relevance
- **Cross-species brain region terms** — e.g. UBERON:0001384 (primary motor cortex) applies to both rodent and human data, enabling comparison
- **Bridges atlas systems** — links Allen Brain Atlas CCF regions, human MNI parcellations (AAL, Brodmann areas), and primate brain regions
- **NWB integration** — [[02_Standards/NWB\|NWB]] uses UBERON for brain region annotation in electrophysiology datasets
- **EBRAINS** — [[03_Platforms/EBRAINS\|EBRAINS]] openMINDS schemas use UBERON for brain region annotation in multimodal neuroscience datasets
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
- Used in: [[03_Platforms/EBRAINS\|EBRAINS]] (openMINDS schemas), [[02_Standards/NWB\|NWB]] (brain region annotation), [[01_Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]] (Atlas alignment)
- Complements: [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] (cognitive processes), [[02_Standards/HED\|HED]] (events)
- Part of: OBO Foundry (alongside [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]])
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], [[01_Actors/IBL\|IBL]], [[01_Actors/Human Connectome Project\|Human Connectome Project]]

## Resources
- https://uberon.org
- https://obofoundry.org/ontology/uberon.html
- https://www.ebi.ac.uk/ols/ontologies/uberon (EBI Ontology Lookup Service)
