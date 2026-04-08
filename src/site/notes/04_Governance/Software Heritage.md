---
{"dg-publish":true,"permalink":"/04-governance/software-heritage/","dg-note-properties":{"name":"Software Heritage","aliases":["Software Heritage Archive"],"website":"https://www.softwareheritage.org","type":"repository","scope":"international","domain":["multimodal"],"status":"active","founded":2016,"parent_org":"Inria / UNESCO"}}
---


# Software Heritage

## Overview
Software Heritage is a non-profit initiative launched by Inria (France) in 2016
under UNESCO auspices, with the mission to collect, preserve, and share all
publicly available software source code. It is the world's largest archive of
software source code, containing 16+ billion unique source files from 250+ million
software projects crawled from GitHub, GitLab, PyPI, npm, CRAN, and dozens of
other forges and package registries.

For research software, Software Heritage provides **long-term archival and
persistent identifiers** (SWHIDs) for software code — directly addressing the
reproducibility crisis where cited software disappears when repositories are
deleted or renamed. Under [[04_Governance/Ouvrir la Science\|Ouvrir la Science]] and the Second PNSO ([[04_Governance/Ouvrir la Science\|Ouvrir la Science]]),
French publicly funded researchers are encouraged to deposit their research
software in Software Heritage as part of open science compliance.

## SWHID — Software Hash Identifiers
The **SWHID** (Software Heritage persistent Identifier) is a content-addressed,
intrinsic identifier for software objects:
- `swh:1:snp:...` — snapshot of a repository at a point in time
- `swh:1:rev:...` — a specific commit/revision
- `swh:1:dir:...` — a directory tree
- `swh:1:cnt:...` — a single source file

SWHIDs are computed from the content itself (like a cryptographic hash), meaning
they are **independent of the hosting location** — the identifier stays valid even
if the original repository is moved, deleted, or renamed. They can be cited in
publications to permanently identify the exact version of software used.

## HAL-Software Heritage Integration
Software Heritage is deeply integrated with [[04_Governance/HAL\|HAL]], France's national open access
archive:
- HAL automatically archives source code referenced in software deposits
- Researchers can deposit software via HAL and receive a HAL identifier +
  a SWHID for the archived code
- This integration implements the **software citation** pillar of [[04_Governance/Ouvrir la Science\|Ouvrir la Science]]

## Research Software Citation
Software Heritage enables the **FORCE11 Software Citation Principles** and
**CITATION.cff** format:
- `CITATION.cff` — a machine-readable citation file in YAML placed at the root
  of a repository, specifying how to cite the software
- CodeMeta — a JSON-LD metadata format for research software, supported by
  Software Heritage and [[03_Platforms/Zenodo\|Zenodo]]

## Connections
- Founded by: Inria + UNESCO
- Integrated with: [[04_Governance/HAL\|HAL]] (French national software archive pathway)
- Related deposit option: [[03_Platforms/Zenodo\|Zenodo]] (also accepts software with DOIs, but not
  as comprehensive in crawling as Software Heritage)
- Implements: [[04_Governance/Ouvrir la Science\|Ouvrir la Science]] software pillar, FORCE11 Software Citation Principles
- Standards: SWHID (persistent identifier), CITATION.cff, CodeMeta (metadata)
- Referenced by: [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/CNRS Open Science\|CNRS Open Science]], [[04_Governance/Inserm Open Science\|Inserm Open Science]]
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (archiving [[01_Actors/DAC\|DAC]] analysis pipelines,
  [[04_Governance/CATI\|CATI]] software, ICM research code under open science mandates)

## Resources
- https://www.softwareheritage.org
- https://archive.softwareheritage.org (Software Heritage Archive — search and browse)
- https://www.softwareheritage.org/save (Save Code Now — deposit a repository)
- https://hal.science (HAL — French integrated deposit pathway)
- https://citation-file-format.github.io (CITATION.cff format)
