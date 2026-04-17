---
{"dg-publish":true,"permalink":"/platforms/orcid/","tags":["icm/uses"],"dg-note-properties":{"name":"Open Researcher and Contributor ID","aliases":["ORCID"],"website":"https://orcid.org","type":"infrastructure","scope":"international","domain":["health","multimodal"],"status":"active","founded":2012,"parent_org":"Independent non-profit membership organisation","tags":["icm/uses"]}}
---


# ORCID — Open Researcher and Contributor ID

## Overview

ORCID is an international non-profit organisation that provides persistent digital identifiers for researchers and contributors to scholarly activity. An ORCID iD is a 16-digit identifier (formatted as a URL: https://orcid.org/0000-0000-0000-0000) that uniquely and persistently identifies a researcher across institutions, name changes and career stages. Launched in 2012, ORCID now has over 20 million registered researchers and is integrated into hundreds of publishing, funding, repository and research management systems worldwide.

The core problem ORCID solves is name ambiguity: common names, transliterations, middle name conventions and institutional affiliations change over time, making it unreliable to identify researchers by name string alone. The ORCID iD is researcher-controlled and researcher-asserted: the researcher owns their record and grants permissions to trusted organisations to read from or write to it.

## ORCID Record and API

An ORCID record holds biographical information, employment history, education, funding, peer review activity, and works (publications, datasets, software). The record is populated through a combination of self-assertion and trusted organisation assertions. The public API allows any system to read public ORCID data; the member API allows trusted organisations to push and pull data with researcher consent.

A key mechanism is the "push" workflow used by publishers, funders and repositories: when a researcher submits a manuscript, dataset or grant application using their ORCID iD, the system can automatically update their ORCID record with the output. This creates a persistent, machine-readable record of research contributions linked by a stable identifier rather than a name string.

## Integration in the Open Science Ecosystem

ORCID iDs are embedded throughout the infrastructure in this graph:

- **Repositories**: [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/Zenodo\|Zenodo]], [[Platforms/OSF\|OSF]], [[Platforms/EGA\|EGA]], [[Platforms/DANDI Archive\|DANDI Archive]], [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] all collect ORCID iDs at deposit and embed them in dataset metadata
- **Publications**: [[Platforms/Preprint Servers\|Preprint Servers]] (bioRxiv, medRxiv), [[Platforms/HAL\|HAL]] and all major journals collect ORCID at submission
- **Funding**: [[Governance/ANR Open Science Policy\|ANR Open Science Policy]] and [[Governance/EC Open Science Policy\|EC Open Science Policy]] require ORCID for grant applications through their respective systems; the EC uses ORCID in the Horizon Europe participant portal
- **Identifiers**: [[Platforms/DataCite\|DataCite]] metadata schema includes ORCID as the preferred creator identifier; [[Standards/DCAT\|DCAT]] profiles in [[Governance/EOSC\|EOSC]] and [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] recommend ORCID for contributor identification

## Relationship to ROR and Other Identifiers

ORCID is part of a broader persistent identifier ecosystem. ROR (Research Organization Registry) provides the institutional equivalent: a persistent identifier for research organisations. Together, ORCID (person) + ROR (institution) + [[Platforms/DataCite\|DataCite]] DOI (output) form the core identifier stack for FAIR scholarly communications. The [[Governance/FAIR Principles\|FAIR Principles]] explicitly require globally unique persistent identifiers; ORCID is the community answer for the researcher dimension.

## French Context

ORCID France is coordinated by INIST-CNRS (under [[Governance/CNRS Open Science\|CNRS Open Science]]) and Couperin. French mandates under [[Governance/Ouvrir la Science\|Ouvrir la Science]] and [[Governance/ANR Open Science Policy\|ANR Open Science Policy]] increasingly require ORCID for funded researchers. [[Platforms/HAL\|HAL]] integration allows French researchers to synchronise their HAL publication list with their ORCID record automatically.

## Connections

- Embedded in: [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/Zenodo\|Zenodo]], [[Platforms/OSF\|OSF]], [[Platforms/EGA\|EGA]], [[Platforms/DANDI Archive\|DANDI Archive]], [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Platforms/HAL\|HAL]], [[Platforms/Preprint Servers\|Preprint Servers]]
- Required by: [[Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[Governance/EC Open Science Policy\|EC Open Science Policy]]
- Metadata standard alignment: [[Platforms/DataCite\|DataCite]], [[Standards/DCAT\|DCAT]], [[Standards/Dublin Core\|Dublin Core]]
- Complements: ROR (institution identifiers), [[Platforms/DataCite\|DataCite]] DOI (output identifiers)
- French coordination: INIST-CNRS / Couperin (under [[Governance/CNRS Open Science\|CNRS Open Science]])
- Participates in: [[Governance/RDA\|RDA]], [[FORCE11\|FORCE11]], [[Governance/EOSC\|EOSC]]

## Resources

- https://orcid.org
- ORCID public API: https://pub.orcid.org
- ORCID France: https://www.orcid-france.fr
