---
{"dg-publish":true,"permalink":"/03-platforms/recherche-data-gouv/","tags":["icm/uses"],"dg-note-properties":{"name":"Recherche Data Gouv","aliases":["Entrepot national de donnees de recherche","RDG"],"website":"https://recherche.data.gouv.fr","type":"repository","scope":"french","domain":["multimodal"],"status":"active","founded":2021,"parent_org":"Ministere de l'Enseignement Superieur et de la Recherche (MESR)","tags":["icm/uses"],"icon":"https://www.recherche.data.gouv.fr/favicon.ico"}}
---


# Recherche Data Gouv

## Overview
Recherche Data Gouv is the French national multidisciplinary research data repository, launched in 2021 by the Ministry of Higher Education and Research (MESR) within the [[04_Governance/data.gouv.fr\|data.gouv.fr]] ecosystem. It is the **primary recommended deposit destination** for research data from French publicly funded projects, fulfilling the data deposit mandates of [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/CNRS Open Science\|CNRS Open Science]], [[04_Governance/Inserm Open Science\|Inserm Open Science]], and [[04_Governance/Ouvrir la Science\|Ouvrir la Science]].

Recherche Data Gouv fills a gap in the French research data landscape: distinct from [[04_Governance/data.gouv.fr\|data.gouv.fr]] (which targets government open data, not research); distinct from [[04_Governance/Health Data Hub\|Health Data Hub]] (which targets clinical/health data under the [[04_Governance/Code de la Sante Publique\|Code de la Sante Publique]] framework); distinct from [[04_Governance/HAL\|HAL]] (which archives publications, not datasets); and the French counterpart to [[03_Platforms/Zenodo\|Zenodo]] (CERN/EU general-purpose repository) for discipline-agnostic research data with French-specific policy compliance.

## What Recherche Data Gouv Provides

### Repository Features
- **DOI assignment** — every deposited dataset receives a persistent DOI
- **FAIR-compliant metadata** — structured metadata schema based on [[02_Standards/DCAT\|DCAT]] / DCAT-AP (EU profile) and [[02_Standards/Dublin Core\|Dublin Core]] (base layer)
- **Version management** — datasets can be updated with new versions while preserving access to previous versions
- **Embargo** — datasets can be deposited with an embargo period (data accessible only after a specified date)
- **Restricted access** — datasets can require access request approval (relevant for sensitive but non-health research data)
- **Large file support** — up to several TB per dataset
- **Open licences** — CC0, CC-BY, Etalab Licence Ouverte

### Disciplinary Nodes
Recherche Data Gouv operates through **disciplinary data nodes** (entrepôts disciplinaires) that provide domain-specific metadata schemas and workflows for specific scientific communities: **Progedo** (social sciences and humanities data); **Nakala** ([[04_Governance/Huma-Num\|Huma-Num]] — humanities and cultural heritage collections); **SEANOE** (ocean sciences data, Ifremer); **Didomena** (education sciences); **Life sciences node** — coordinated by [[04_Governance/IFB\|IFB]] (ELIXIR-FR); provides bioinformatics-specific guidance and FAIR-Checker integration. The disciplinary nodes are aggregated into the Recherche Data Gouv catalogue for unified discoverability and EOSC harvesting.

### OPIDoR Integration
Recherche Data Gouv is tightly integrated with [[04_Governance/OPIDoR\|OPIDoR]]: **DMP OPIDoR** links directly to Recherche Data Gouv as the recommended deposit destination for French research data; **Cat OPIDoR** catalogues Recherche Data Gouv among French RDM services; **JurisDoR** provides legal guidance for deposits under GDPR and French law.

### European Discoverability
- Metadata is harvested by [[04_Governance/EOSC\|EOSC]] via DCAT-AP, making French research datasets discoverable across European research infrastructure
- [[04_Governance/OpenAIRE\|OpenAIRE]] harvests Recherche Data Gouv metadata for EU open science monitoring
- Deposits with DOIs are indexed in DataCite, enabling citation tracking

## Depositing from Paris Brain Institute
For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] researchers, Recherche Data Gouv is the appropriate repository for non-sensitive research data not covered by domain-specific repositories (e.g. behavioural data, quantitative microscopy, electrophysiology where [[03_Platforms/DANDI Archive\|DANDI Archive]] or [[03_Platforms/OpenNeuro\|OpenNeuro]] are not appropriate), software and analysis code (alongside or instead of [[04_Governance/Software Heritage\|Software Heritage]]), supplementary data associated with publications in [[04_Governance/HAL\|HAL]], and data that must satisfy ANR or Horizon Europe deposit mandates but lacks a domain-specific FAIR repository.

Neuroimaging data should prefer [[03_Platforms/OpenNeuro\|OpenNeuro]] ([[02_Standards/BIDS\|BIDS]]-organised); genomics data should prefer [[03_Platforms/NCBI GEO\|NCBI GEO]] (open) or [[03_Platforms/EGA\|EGA]] (controlled access); electrophysiology data should prefer [[03_Platforms/DANDI Archive\|DANDI Archive]] ([[02_Standards/NWB\|NWB]]-formatted).

## Connections
- Part of: [[04_Governance/data.gouv.fr\|data.gouv.fr]] ecosystem, [[04_Governance/Ouvrir la Science\|Ouvrir la Science]]
- Mandated by: [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/CNRS Open Science\|CNRS Open Science]], [[04_Governance/Inserm Open Science\|Inserm Open Science]]
- Life sciences node: [[04_Governance/IFB\|IFB]] (ELIXIR-FR Disciplinary Competence Centre)
- DMP integration: [[04_Governance/OPIDoR\|OPIDoR]] (DMP OPIDoR → Recherche Data Gouv pipeline)
- Legal guidance: [[04_Governance/OPIDoR\|OPIDoR]] JurisDoR
- Metadata standards: [[02_Standards/DCAT\|DCAT]] / DCAT-AP (EU profile), [[02_Standards/Dublin Core\|Dublin Core]] (base)
- European discoverability: [[04_Governance/EOSC\|EOSC]], [[04_Governance/OpenAIRE\|OpenAIRE]] (DCAT-AP harvesting)
- Domain alternatives: [[03_Platforms/OpenNeuro\|OpenNeuro]] (neuroimaging), [[03_Platforms/DANDI Archive\|DANDI Archive]] (neurophysiology), [[03_Platforms/NCBI GEO\|NCBI GEO]] / [[03_Platforms/EGA\|EGA]] (genomics)
- Related general-purpose: [[03_Platforms/Zenodo\|Zenodo]] (CERN/EU counterpart)
- Implements: [[04_Governance/FAIR Principles\|FAIR Principles]]

## Resources
- https://recherche.data.gouv.fr
- https://recherche.data.gouv.fr/en/depositing-data (deposit guide)
- https://recherche.data.gouv.fr/en/repositories (disciplinary nodes catalogue)
- https://cat.opidor.fr (Cat OPIDoR — discover French RDM services)
