---
{"dg-publish":true,"permalink":"/platforms/data-cite/","tags":["icm/uses"],"dg-note-properties":{"name":"DataCite","aliases":["DataCite"],"website":"https://datacite.org","type":"infrastructure","scope":"international","domain":["health","multimodal"],"status":"active","founded":2009,"parent_org":"Independent non-profit membership organisation","tags":["icm/uses"]}}
---


# DataCite

## Overview

DataCite is an international non-profit organisation that provides persistent identifier infrastructure for research outputs, primarily through DOI (Digital Object Identifier) registration for research datasets, software, preprints, samples and other non-publication scholarly outputs. Founded in 2009 by a consortium of national research libraries and data centres, it now has over 50 member organisations worldwide and has registered hundreds of millions of DOIs for research objects.

DataCite is the primary DOI registration agency for research data in the open science ecosystem, occupying a distinct role from CrossRef, which handles journal articles and book chapters. The two agencies cooperate and their metadata is interoperable, allowing citation relationships between datasets and publications to be expressed and tracked.

## DataCite Metadata Schema

The DataCite Metadata Schema defines the required and recommended metadata fields for a DataCite DOI. The current version (4.x) includes mandatory fields (identifier, creator, title, publisher, publication year, resource type) and an extensive set of recommended fields covering funding, geolocation, related identifiers, subjects, contributors and rights. The schema is aligned with [[Standards/Dublin Core\|Dublin Core]] and [[Standards/DCAT\|DCAT]], and supports [[Platforms/ORCID\|ORCID]] identifiers for creators and contributors and ROR (Research Organization Registry) identifiers for institutions.

The related identifier field is particularly important for open science: it allows datasets to be linked to the associated publication, software, protocol or other dataset using typed relationships (IsSupplementTo, IsDerivedFrom, IsVersionOf, etc.), enabling machine-readable scholarly knowledge graphs.

## Role in the Repository Ecosystem

Virtually every open repository in this graph uses DataCite DOIs as persistent identifiers for deposited objects:

- [[Platforms/Zenodo\|Zenodo]] — all deposits receive a DataCite DOI; Zenodo is itself a DataCite member
- [[Platforms/DANDI Archive\|DANDI Archive]] — NWB datasets receive DataCite DOIs
- [[Platforms/OpenNeuro\|OpenNeuro]] — BIDS datasets receive DataCite DOIs
- [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] — DataCite DOIs for all deposited datasets; French node via INIST-CNRS
- [[Platforms/HAL\|HAL]] — DataCite DOIs for data linked from HAL records
- [[Platforms/OSF\|OSF]] — DataCite DOIs for registered projects and datasets

DataCite also operates Make Data Count, a project that tracks dataset views and downloads as equivalent metrics to article citations, relevant for incentivising open data sharing under [[Governance/Ouvrir la Science\|Ouvrir la Science]] and [[Governance/EC Open Science Policy\|EC Open Science Policy]] mandates.

## Relationship to EOSC and RDA

DataCite is a key infrastructure component of [[Governance/EOSC\|EOSC]], providing the persistent identifier layer that makes datasets findable and citable across the European open science cloud. DataCite participates actively in [[Governance/RDA\|RDA]] working groups, particularly those dealing with data citation, persistent identifiers and the FAIR data maturity model. DataCite's metadata is harvested by [[Platforms/OpenAIRE\|OpenAIRE]] and exposed through the EOSC catalogue.

## Connections

- Issues DOIs for: [[Platforms/Zenodo\|Zenodo]], [[Platforms/DANDI Archive\|DANDI Archive]], [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Platforms/OSF\|OSF]]
- Metadata schema aligns with: [[Standards/Dublin Core\|Dublin Core]], [[Standards/DCAT\|DCAT]]
- Supports: [[Platforms/ORCID\|ORCID]] (creator identifiers), ROR (institution identifiers)
- Integrated into: [[Governance/EOSC\|EOSC]], [[Platforms/OpenAIRE\|OpenAIRE]]
- Participates in: [[Governance/RDA\|RDA]], [[FORCE11\|FORCE11]]
- French node: INIST-CNRS (via [[Governance/CNRS Open Science\|CNRS Open Science]])

## Resources

- https://datacite.org
- DataCite Metadata Schema: https://schema.datacite.org
- Make Data Count: https://makedatacount.org
