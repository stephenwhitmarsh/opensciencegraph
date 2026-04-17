---
{"dg-publish":true,"permalink":"/standards/rrid/","dg-note-properties":{"name":"Research Resource Identifiers","aliases":["RRID"],"website":"https://www.rrids.org","type":"standard","scope":"international","domain":["multimodal"],"status":"active","founded":2014,"parent_org":"NIF / SciCrunch (UCSD)"}}
---


# RRID — Research Resource Identifiers

## Overview
RRIDs (Research Resource Identifiers) are persistent, unique identifiers for the reagents, tools, model organisms, software, and core facilities used in biomedical research. Developed by the **[[Governance/NIF\|NIF]]** (Neuroscience Information Framework) at UCSD and now coordinated through the SciCrunch Registry, RRIDs provide unambiguous citation of research resources in Methods sections — addressing the reproducibility crisis caused by ambiguous reagent descriptions in publications.

RRIDs are mandated by hundreds of journals including Nature, Science, Cell, eLife, and the major neuroscience journals. They resolve to curated records in the SciCrunch Registry (https://scicrunch.org).

## RRID Categories
Each resource type is managed by a dedicated authority database:

| Category | Prefix | Authority |
|---|---|---|
| Antibodies | `RRID:AB_` | Antibody Registry |
| Cell lines | `RRID:CVCL_` | Cellosaurus (SIB/ExPASy) |
| Model organisms | `RRID:IMSR_`, `RRID:MGI_`, etc. | JAX, MGI, ZFIN, FlyBase, etc. |
| Software / tools / databases | `RRID:SCR_` | SciCrunch Registry |
| Core facilities | `RRID:SCR_` | SciCrunch Registry / CoreMarketplace |

## RRIDs for ICM Core Facilities
All ICM platforms are registered in the SciCrunch Registry and should be cited using their RRID in publications that use their services:

| Platform | RRID | SciCrunch record |
|---|---|---|
| Paris Brain Institute (institution) | `RRID:SCR_026379` | https://scicrunch.org/resolver/SCR_026379 |
| DAC — Data Analysis Core | `RRID:SCR_026138` | https://scicrunch.org/resolver/SCR_026138 |
| ICM Quant — Quantitative Imaging | `RRID:SCR_026393` | https://scicrunch.org/resolver/SCR_026393 |
| ePHYS — Electrophysiology | `RRID:SCR_026412` | https://scicrunch.org/resolver/SCR_026412 |
| PRISME — Behavioural Phenotyping | `RRID:SCR_026394` | https://scicrunch.org/resolver/SCR_026394 |
| HISTOMICS — Histology and Neuropathology | `RRID:SCR_028275` | https://scicrunch.org/resolver/SCR_028275 |
| ICV — Cellular Engineering and Vectorology | `RRID:SCR_028048` | https://scicrunch.org/resolver/SCR_028048 |

## How to Cite
The standard citation format is the resource name followed by the RRID in parentheses, e.g.:
> *"Data analysis was performed by the Paris Brain Institute Data Analysis Core Facility (RRID:SCR_026138)."*

## Connections
- Produced by: [[Governance/NIF\|NIF]] (Neuroscience Information Framework / SciCrunch)
- Resolves via: SciCrunch Registry (https://scicrunch.org)
- Complements: [[Governance/ORCID\|ORCID]] (researcher IDs), [[Standards/ROR\|ROR]] (organisation IDs), [[Governance/DataCite\|DataCite]] (output DOIs)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Actors/DAC\|DAC]], [[Actors/CENIR\|CENIR]], [[Actors/iGENSEQ\|iGENSEQ]] (antibody/reagent citations in publications)

## Resources
- https://www.rrids.org (RRID initiative)
- https://scicrunch.org (SciCrunch Registry — RRID resolver)
- https://coremarketplace.org (CoreMarketplace — core facility RRIDs)