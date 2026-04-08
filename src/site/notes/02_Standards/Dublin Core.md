---
{"dg-publish":true,"permalink":"/02-standards/dublin-core/","tags":["icm/uses"],"dg-note-properties":{"name":"Dublin Core Metadata Initiative","aliases":["Dublin Core","DCMI","DC"],"website":"https://dublincore.org","type":"standard","scope":"international","domain":["multimodal"],"status":"active","founded":1995,"parent_org":"Dublin Core Metadata Initiative","tags":["icm/uses"],"icon":"https://dublincore.org/favicon.ico"}}
---


# Dublin Core — Dublin Core Metadata Initiative

## Overview
Dublin Core is the simplest and most widely deployed metadata standard, providing
15 basic elements (title, creator, subject, description, publisher, contributor,
date, type, format, identifier, source, language, relation, coverage, rights)
for describing any resource. Originating from a 1995 workshop in Dublin, Ohio,
it became an ISO standard (ISO 15836) and is now ubiquitous as the base metadata
layer in virtually every research data repository, publication archive, and
digital library. For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], Dublin Core is the lowest
common denominator: any dataset deposited in [[03_Platforms/Zenodo\|Zenodo]], [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]],
or [[03_Platforms/OpenNeuro\|OpenNeuro]], and any publication deposited in HAL, will carry Dublin Core
metadata, often enriched with more specific standards on top.

## The 15 Dublin Core Elements
| Element | Description | Example |
|---|---|---|
| `dc:title` | Name of the resource | "MEMENTO cohort MRI data" |
| `dc:creator` | Author or PI | "Stéphanie Dupont" |
| `dc:subject` | Keywords or topic | "Alzheimer, neuroimaging, longitudinal" |
| `dc:description` | Abstract or summary | Free-text description |
| `dc:publisher` | Institution or repository | "Recherche Data Gouv" |
| `dc:date` | Publication date | "2024-03-15" |
| `dc:identifier` | DOI or persistent ID | "https://doi.org/10.57745/..." |
| `dc:format` | File format | "NIfTI, BIDS" |
| `dc:rights` | License | "CC BY 4.0" |

## Role in the Open Science Ecosystem
Dublin Core is the **lingua franca of metadata** — it is:
- The base layer beneath [[02_Standards/DCAT\|DCAT]], DataCite, and schema.org in all major repositories
- Used by [[03_Platforms/Zenodo\|Zenodo]], HAL, [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]], and institutional repositories
- Automatically generated when depositing data in any major repository
- Harvested by aggregators (OpenAIRE, [[04_Governance/EOSC\|EOSC]]) for cross-portal search

## Connections
- Used by: [[03_Platforms/Zenodo\|Zenodo]], [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[04_Governance/OpenAIRE\|OpenAIRE]], HAL
- Enriched by: [[02_Standards/DCAT\|DCAT]] (adds dataset-specific concepts), DataCite (adds citation metadata)
- Implements: [[04_Governance/FAIR Principles\|FAIR Principles]] F1, F2, F4 (at a basic level)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (all data deposits and publications)

## Resources
- https://dublincore.org
- https://www.dublincore.org/specifications/dublin-core/dcmi-terms/ (full terms)
- https://validator.dublincore.org (metadata validator)
