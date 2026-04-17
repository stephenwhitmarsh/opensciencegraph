---
{"dg-publish":true,"permalink":"/standards/dcat/","dg-note-properties":{"name":"Data Catalog Vocabulary","aliases":["DCAT","W3C DCAT"],"website":"https://www.w3.org/TR/vocab-dcat/","type":"standard","scope":"international","domain":["multimodal"],"status":"active","founded":2014,"parent_org":"W3C (World Wide Web Consortium)","icon":"https://www.w3.org/favicon.ico"}}
---


# DCAT — Data Catalog Vocabulary

## Overview
DCAT is the W3C standard for describing datasets and data catalogues in RDF (Resource Description Framework), enabling federated data discovery across distributed repositories. Published as a W3C Recommendation (DCAT v1: 2014, DCAT v2: 2020, DCAT v3: 2024), it is the vocabulary that makes data catalogues interoperable: a dataset described with DCAT in [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] can be harvested and found through the [[Governance/EOSC\|EOSC]] portal, [[Platforms/data.gouv.fr\|data.gouv.fr]], and other DCAT-compliant catalogues without any manual re-entry. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], DCAT is the "invisible" standard that powers discoverability of ICM datasets in the French and European open science ecosystem.

## Core Classes
| Class | Description |
|---|---|
| `dcat:Dataset` | A logical collection of data (e.g. a neuroimaging cohort) |
| `dcat:Distribution` | A specific form/download of a dataset (e.g. a ZIP file, an API endpoint) |
| `dcat:Catalog` | A curated collection of dataset metadata (e.g. Recherche Data Gouv catalogue) |
| `dcat:DataService` | An API or endpoint providing access to data |

## Where DCAT is Used in the ICM Ecosystem
- **[[Platforms/Recherche Data Gouv\|Recherche Data Gouv]]** — uses DCAT as the underlying metadata model; all deposited datasets are described in DCAT-AP (the EU profile of DCAT)
- **[[Governance/EOSC\|EOSC]]** — uses DCAT-AP for cross-portal data discovery across European repositories; ICM datasets on Recherche Data Gouv are automatically harvested into the EOSC catalogue
- **[[Platforms/data.gouv.fr\|data.gouv.fr]]** — uses DCAT for all government open data catalogue entries
- **[[Platforms/Health Data Hub\|Health Data Hub]]** — catalogue of health datasets uses DCAT-AP

## DCAT-AP
DCAT-AP is the European Application Profile of DCAT — a specification that adds requirements and recommendations specific to European public sector data. It is the standard for data portals in the EU Open Data Portal and for EOSC.

## Connections
- Implements: [[Governance/FAIR Principles\|FAIR Principles]] F4 (data registered in a searchable resource)
- Used by: [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Governance/EOSC\|EOSC]], [[Platforms/data.gouv.fr\|data.gouv.fr]], [[Platforms/Health Data Hub\|Health Data Hub]]
- Complements: Dublin Core (simpler metadata), [[Standards/PROV-O\|PROV-O]] (provenance)
- Related: [[Platforms/OPIDoR\|OPIDoR]] (DMP tools produce DCAT-compatible metadata)

## Resources
- https://www.w3.org/TR/vocab-dcat/ (W3C DCAT specification)
- https://joinup.ec.europa.eu/collection/semantic-interoperability-community-semic/solution/dcat-application-profile-data-portals-europe (DCAT-AP)
