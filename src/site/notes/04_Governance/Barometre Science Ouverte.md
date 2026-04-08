---
{"dg-publish":true,"permalink":"/04-governance/barometre-science-ouverte/","dg-note-properties":{"name":"Baromètre Français de la Science Ouverte","aliases":["French Open Science Monitor","BSO"],"website":"https://frenchopensciencemonitor.esr.gouv.fr","type":"platform","scope":"french","domain":["multimodal"],"status":"active","founded":2019,"parent_org":"Ministère de l'Enseignement Supérieur et de la Recherche (MESR)"}}
---


# Baromètre Français de la Science Ouverte

## Overview
The Baromètre Français de la Science Ouverte (BSO — French Open Science Monitor)
is an open-data dashboard developed by the French Ministry of Higher Education
and Research (MESR) to track the progress of open science practices across
French publicly funded research. Launched in 2019, it measures and publishes
annual statistics on open access to publications, open research data, and
open source software, providing the empirical evidence base for French open
science policy implementation under [[04_Governance/Ouvrir la Science\|Ouvrir la Science]].

The BSO is built entirely on open data and open-source methodology, with all
code available on GitHub, making it a model of open science applied to open
science monitoring itself.

## What It Measures

### Open Access to Publications
- Open access rate of French scientific publications by year, discipline,
  publisher type, and funding source
- Breakdown by access type: gold (publisher OA), green (repository deposit
  in [[04_Governance/HAL\|HAL]]), hybrid, bronze
- Compliance rates with [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]] mandates
- Institutional breakdown (by university, research organisation)

### Research Data
- Proportion of French publications with associated open data statements
- Data availability by discipline and funder
- Deposits in [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] and discipline-specific repositories

### Software
- Open source software publication rates
- Software Heritage deposits

## Technical Implementation
The BSO uses:
- **Unpaywall** and **OpenAlex** for publication open access status
- **[[04_Governance/HAL\|HAL]]** metadata for French repository deposits
- **DOI** resolution for publication identification
- **[[02_Standards/DCAT\|DCAT]]** / **[[02_Standards/Dublin Core\|Dublin Core]]** for dataset metadata
- All source code: https://github.com/MinistereSupRecherche/bso

## Institutional Adaptations
The BSO methodology has been adapted by individual institutions to create
local open science monitors:
- **BSO3** — institutional version deployed at universities and research
  organisations including Inserm, CNRS, and Sorbonne Université
- **Institut Pasteur Barometer** — Pasteur's local adaptation tracking its
  90%+ open access rate
- These local monitors feed into the national BSO aggregation

## Connections
- Produced by: MESR (French Ministry of Higher Education and Research)
- Measures: [[04_Governance/HAL\|HAL]] (publication deposits), [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] (data),
  [[04_Governance/Ouvrir la Science\|Ouvrir la Science]] (policy compliance)
- Implements: [[04_Governance/FAIR Principles\|FAIR Principles]] (methodology is open and reproducible)
- Policy context: [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/CoSO\|CoSO]]
- Related: [[04_Governance/OpenAIRE\|OpenAIRE]] (European equivalent monitoring — Open Science Monitor EU)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (ICM open access rate tracked;
  Sorbonne Université BSO3 covers ICM publications)

## Resources
- https://frenchopensciencemonitor.esr.gouv.fr
- https://github.com/MinistereSupRecherche/bso (source code)
