---
{"dg-publish":true,"permalink":"/standards/ror/","dg-note-properties":{"name":"Research Organization Registry","aliases":["ROR"],"website":"https://ror.org","type":"standard","scope":"international","domain":["multimodal"],"status":"active","founded":2019,"parent_org":"ROR Community (California Digital Library / Crossref / DataCite / ISNI)"}}
---


# ROR — Research Organization Registry

## Overview
ROR (Research Organization Registry) is a community-led registry that provides persistent, unique identifiers for research organisations — universities, research institutes, funders, hospitals, and government agencies. Launched in 2019 and maintained by a coalition of California Digital Library, Crossref, DataCite, and the ISNI International Agency, ROR fills the gap that [[Platforms/ORCID\|ORCID]] fills for individual researchers: a machine-readable, globally unique identifier for institutions that enables unambiguous affiliation metadata in publications, datasets, and grant records.

For the open science ecosystem this vault covers, ROR is the organisational identifier layer that complements [[Platforms/ORCID\|ORCID]] (people), [[Platforms/DataCite\|DataCite]] DOIs (research outputs), and [[Standards/RRID\|RRID]] (research resources). Every Actor node in this graph is a research organisation with a ROR ID.

## How ROR Works
- Each organisation receives a unique ROR ID in the format `https://ror.org/XXXXXXXXX`
- ROR records include: official name, aliases, country, organisation type, external identifiers (ISNI, GRID, Wikidata, Fundref), and relationships to parent/child organisations
- The full ROR dataset is openly available under CC0 — no licence required for reuse
- ROR IDs are resolved at `https://ror.org/<id>` and via a public API

## Adoption
ROR is rapidly becoming the standard for affiliation metadata in the scholarly communication infrastructure:
- **[[Platforms/DataCite\|DataCite]]** — uses ROR for funder and organisation metadata in DOI records
- **[[Platforms/ORCID\|ORCID]]** — integrates ROR for institutional affiliation in researcher profiles
- **[[Platforms/OpenAIRE\|OpenAIRE]]** — uses ROR for organisation disambiguation across EU publications
- **Crossref** — uses ROR for funder registry (replacing Fundref)
- **[[Platforms/Recherche Data Gouv\|Recherche Data Gouv]]** — uses ROR for depositing institution metadata
- **[[Governance/EOSC\|EOSC]]** — ROR adopted across EOSC services for organisation identification
- Hundreds of publishers, repositories, and CRIS systems now support ROR natively

## ICM ROR ID
- **Paris Brain Institute (ICM)**: `https://ror.org/050gn5214`

## Connections
- Complements: [[Platforms/ORCID\|ORCID]] (persistent identifiers for researchers)
- Used by: [[Platforms/DataCite\|DataCite]], [[Platforms/OpenAIRE\|OpenAIRE]], [[Platforms/ORCID\|ORCID]], [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Governance/EOSC\|EOSC]]
- Related: [[Standards/RRID\|RRID]] (persistent identifiers for research resources)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (ROR ID: https://ror.org/050gn5214; used in dataset and publication metadata)

## Resources
- https://ror.org
- https://ror.org/050gn5214 (Paris Brain Institute ROR record)
- https://ror.org/about (ROR overview and governance)
- https://github.com/ror-community (ROR community on GitHub)
