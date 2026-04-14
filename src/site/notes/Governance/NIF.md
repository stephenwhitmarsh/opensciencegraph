---
{"dg-publish":true,"permalink":"/governance/nif/","dg-note-properties":{"name":"Neuroscience Information Framework","aliases":["NIF"],"website":"https://neuinfo.org","type":"platform","scope":"international","domain":["neuroimaging","multimodal"],"status":"active","founded":2008,"parent_org":"UCSD / NIH Blueprint for Neuroscience Research"}}
---


# NIF — Neuroscience Information Framework

## Overview
The Neuroscience Information Framework (NIF) is a US NIH-funded resource for discovering and accessing neuroscience data, tools, and materials. Developed at UCSD (University of California San Diego) under the NIH Blueprint for Neuroscience Research, NIF provides a comprehensive registry of neuroscience resources — databases, software tools, data repositories, model organisms, antibodies, and more — with unique identifiers (RRID — Research Resource Identifiers) that enable unambiguous citation of research resources in scientific publications.

NIF's most widely used product is the **RRID** (Research Resource Identifier) system, which is now mandated by hundreds of journals for citing antibodies, mcell lines, model organisms, software tools, and databases in Methods sections.

## Key Products

### RRID — Research Resource Identifiers
RRIDs provide unique, persistent identifiers for research resources:
- **Antibodies** — RRID:AB_xxxxxxx (from Antibody Registry)
- **Cell lines** — RRID:CVCL_xxxx (from Cellosaurus)
- **Model organisms** — RRID:IMSR_JAX:xxxxxx (mouse strains from JAX, etc.)
- **Software tools** — RRID:SCR_xxxxxx (from SciCrunch Registry)
- **Databases** — RRID:SCR_xxxxxx

RRIDs are increasingly required in Methods sections by journals including Nature, Science, Cell, eLife, and most neuroscience journals. They resolve to resource records in the SciCrunch Registry (https://scicrunch.org).

### NIF Data Federation / SPARC Portal Integration
NIF originally operated as a federated neuroscience data search engine, and its registry infrastructure now underpins the **SPARC Portal** (https://sparc.science) used by [[Standards/SPARC SDS\|SPARC SDS]] datasets and the NIH BRAIN Initiative resource catalogue.

### Suggested Data Repositories
NIF maintains a curated list of recommended data repositories for neuroscience (https://neuinfo.org/rin/suggested-data-repositories), organised by data type — a key reference for researchers choosing deposit venues for neuroimaging, electrophysiology, genomics, and clinical neuroscience data.

## Connections
- Funded by: NIH Blueprint for Neuroscience Research
- Produces: [[Standards/RRID\|RRID]] system (widely adopted by journals)
- Maintains: neuroscience resource registry (SciCrunch)
- Integrates with: [[Standards/SPARC SDS\|SPARC SDS]] (SPARC Portal uses NIF resource registry)
- Data repository guide: https://neuinfo.org/rin/suggested-data-repositories
- Related: [[Actors/INCF\|INCF]] (complementary international neuroinformatics body)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (RRID use in publications for antibodies, cell lines, and software tools; repository selection guidance)

## Resources
- https://neuinfo.org
- https://scicrunch.org (SciCrunch resource registry — RRID resolver)
- https://neuinfo.org/rin/suggested-data-repositories (recommended repositories)
- https://www.rrids.org (RRID initiative)
