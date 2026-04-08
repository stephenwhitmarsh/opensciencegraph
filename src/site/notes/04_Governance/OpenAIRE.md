---
{"dg-publish":true,"permalink":"/04-governance/open-aire/","dg-note-properties":{"name":"OpenAIRE","aliases":["OpenAIRE AMKE","OpenAIRE Nexus"],"website":"https://www.openaire.eu","type":"infrastructure","scope":"european","domain":["multimodal"],"status":"active","founded":2009,"parent_org":"EU / OpenAIRE consortium (50+ organisations)"}}
---


# OpenAIRE

## Overview
OpenAIRE (Open Access Infrastructure for Research in Europe) is the EU's primary
open science and open access infrastructure, operating since 2009 through successive
EU-funded projects and now as the **OpenAIRE AMKE** (Association Membre sans but
Lucratif) — a legal entity consortium of 50+ research organisations, funders, and
infrastructure providers across Europe. OpenAIRE manages the European scholarly
communication ecosystem: it aggregates open access publications, research data,
and software from repositories worldwide, operates [[03_Platforms/Zenodo\|Zenodo]] as the flagship open
research repository, monitors Horizon Europe open access compliance, and provides
the technical services that connect research outputs to ORCID identifiers, funding
information, and persistent identifiers.

## Key Services

### OpenAIRE Graph
The **OpenAIRE Research Graph** is a massive open knowledge graph connecting:
- 160+ million publications, datasets, and software objects
- Linked to funding information (grants from EC, ANR, ERC, Wellcome, etc.)
- Linked to ORCID researcher identifiers
- Linked to organisations and projects
- Fully open and downloadable (CC0 licence)

The Graph powers literature search (explore.openaire.eu), open access monitoring,
and impact tracking. It harvests metadata from [[04_Governance/HAL\|HAL]], [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]],
[[03_Platforms/EGA\|EGA]], [[03_Platforms/OpenNeuro\|OpenNeuro]], and hundreds of other repositories via OAI-PMH, SWORD,
and REST APIs.

### Zenodo
[[03_Platforms/Zenodo\|Zenodo]] (https://zenodo.org) is operated by OpenAIRE and CERN as the
general-purpose open research repository. It accepts any research output (datasets,
code, publications, presentations), assigns DOIs, and is the recommended deposit
destination for EU-funded projects that lack a domain-specific repository.

### Monitor (Open Science Observatory)
The **OpenAIRE Monitor** (https://monitor.openaire.eu) provides open science
monitoring dashboards for:
- Institutional open access rates (analogous to [[04_Governance/Barometre Science Ouverte\|Barometre Science Ouverte]] but European-wide)
- Funder compliance dashboards (Horizon Europe OA compliance)
- Country and repository-level statistics

### Amnesia
**Amnesia** (https://amnesia.openaire.eu) is OpenAIRE's anonymisation tool for
research datasets, designed to help researchers share sensitive data by applying
k-anonymisation and other privacy-preserving transformations — directly relevant
to health and genomics data sharing under [[04_Governance/EHDS\|EHDS]] and GDPR.

### Scholix
OpenAIRE co-developed **Scholix** (Scholarly Link Exchange) — the framework for
linking publications to their underlying datasets, enabling research data citation
and tracking across publishers and repositories.

## Horizon Europe Compliance
All Horizon Europe projects are required to:
- Make publications open access immediately (via HAL, institutional repository,
  or journal OA)
- Deposit datasets in an [[04_Governance/EOSC\|EOSC]]-compatible repository
- OpenAIRE's monitoring infrastructure verifies compliance and feeds into the
  European Commission's open access reporting

## Connections
- Operates: [[03_Platforms/Zenodo\|Zenodo]] (general-purpose repository)
- Part of: [[04_Governance/EOSC\|EOSC]] (key service provider and governance member)
- Harvests: [[04_Governance/HAL\|HAL]], [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[03_Platforms/EGA\|EGA]], [[03_Platforms/OpenNeuro\|OpenNeuro]], 900+ repositories
- Partners: [[04_Governance/RDA\|RDA]], [[04_Governance/GO FAIR\|GO FAIR]], [[04_Governance/ELIXIR\|ELIXIR]]
- Monitors: Horizon Europe OA compliance, French OA rates (via [[04_Governance/HAL\|HAL]] metadata)
- Standards: [[02_Standards/DCAT\|DCAT]] (dataset metadata), [[02_Standards/Dublin Core\|Dublin Core]] (base metadata),
  [[04_Governance/FAIR Principles\|FAIR Principles]] (R1.1 licence, F1 PID)
- French alignment: [[04_Governance/Ouvrir la Science\|Ouvrir la Science]], [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/HAL\|HAL]]
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (Horizon Europe compliance, Zenodo deposit,
  ORCID linking, publication open access monitoring)

## Resources
- https://www.openaire.eu
- https://explore.openaire.eu (OpenAIRE Explore — literature and dataset search)
- https://zenodo.org (Zenodo — general-purpose repository)
- https://monitor.openaire.eu (OpenAIRE Monitor — OA monitoring)
- https://amnesia.openaire.eu (Amnesia — anonymisation tool)
- https://graph.openaire.eu (OpenAIRE Research Graph — open knowledge graph)
