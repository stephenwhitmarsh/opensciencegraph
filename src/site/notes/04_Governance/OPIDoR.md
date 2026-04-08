---
{"dg-publish":true,"permalink":"/04-governance/opi-do-r/","tags":["icm/uses"],"dg-note-properties":{"name":"OPIDoR","aliases":["DMP OPIDoR","Cat OPIDoR","PID OPIDoR","DORANum"],"website":"https://opidor.fr","type":"platform","scope":"french","domain":["multimodal"],"status":"active","founded":2016,"parent_org":"INIST-CNRS / Ministère de l'Enseignement Supérieur et de la Recherche","tags":["icm/uses"],"icon":"https://opidor.fr/favicon.ico"}}
---


# OPIDoR

## Overview
OPIDoR (Optimiser le PIlotage des Données de la Recherche) is the suite of
research data management tools and services operated by **INIST-CNRS** on behalf
of the French Ministry of Higher Education and Research. It is the primary DMP
infrastructure for French publicly funded research, directly implementing the
[[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]] and [[04_Governance/Ouvrir la Science\|Ouvrir la Science]] mandates for Data
Management Plans. For [[00_Core/Paris Brain Institute\|Paris Brain Institute]], OPIDoR's DMP OPIDoR tool
is the recommended platform for meeting ANR DMP requirements on funded projects.

## Components

### DMP OPIDoR (https://dmp.opidor.fr)
The national online DMP tool, based on the DMPRoadmap open-source platform,
hosted and operated entirely by INIST-CNRS. Provides structured questionnaires,
DMP templates for major funders (ANR, Horizon Europe), and a repository of
public DMPs. ANR, CNRS, and Institut Pasteur have all adopted DMP OPIDoR as
their official DMP template platform. It is the primary DMP tool for the
broad French research community regardless of discipline.

Note: [[04_Governance/IFB\|IFB]] (ELIXIR-FR) operates a **separate** DMP tool — **DSW@IFB**
(Data Stewardship Wizard, https://dsw.france-bioinformatique.fr) — specifically
for life sciences infrastructure DMP template development. IFB recommends
both DMP OPIDoR and DSW@IFB to its users, and interoperability between the
two tools is under development. IFB does not host or operate DMP OPIDoR.

### Cat OPIDoR (https://cat.opidor.fr)
A national catalogue of research data management services, tools, and
repositories available to French researchers. Helps researchers identify
appropriate deposit destinations, DMP support services, and PID providers.
Complements [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] as a discovery layer.

### PID OPIDoR
Guidance and tooling for Persistent Identifier (PID) management — DOIs, ORCIDs,
ROR identifiers — supporting FAIR data requirements across French institutions.

### DORANum (https://doranum.fr)
The national training portal for research data management best practices, run
by INIST. Provides open educational resources on FAIR principles, DMPs, data
sharing, and open science for French researchers and data stewards.

### JurisDoR (https://recherche.data.gouv.fr/en/actuality/jurisdor)
A legal resources centre for research data management operated within the
[[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] ecosystem. Covers GDPR compliance for research data,
intellectual property, consent frameworks, and data sharing agreements —
directly relevant to neuroimaging and genomics research at
[[00_Core/Paris Brain Institute\|Paris Brain Institute]] given sensitivity of health data under [[04_Governance/EHDS\|EHDS]].

## Connections
- Operated exclusively by: INIST-CNRS (not hosted or operated by IFB)
- Parallel life sciences DMP tool: [[04_Governance/IFB\|IFB]] DSW@IFB (https://dsw.france-bioinformatique.fr)
  — a separate Data Stewardship Wizard instance for life sciences; interoperability
  with DMP OPIDoR is under development but they are independent tools
- Part of: [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] ecosystem, [[04_Governance/data.gouv.fr\|data.gouv.fr]]
- Implements: [[04_Governance/Ouvrir la Science\|Ouvrir la Science]], [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]] mandates
- FAIR tooling: DMP OPIDoR enforces [[04_Governance/FAIR Principles\|FAIR Principles]] R1.3 (domain standards)
  and F1 (persistent identifiers) through PID OPIDoR
- European alignment: [[04_Governance/EOSC\|EOSC]] (DMPs linked to EOSC infrastructure),
  [[04_Governance/OpenAIRE\|OpenAIRE]] (DMP interoperability)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (ANR DMP compliance),
  [[04_Governance/CNRS Open Science\|CNRS Open Science]], [[04_Governance/Inserm Open Science\|Inserm Open Science]]

## Resources
- https://opidor.fr
- https://dmp.opidor.fr
- https://cat.opidor.fr
- https://doranum.fr
