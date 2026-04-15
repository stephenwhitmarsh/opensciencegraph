---
{"dg-publish":true,"permalink":"/governance/ifb/","tags":["icm/uses"],"dg-note-properties":{"name":"Institut Français de Bioinformatique","aliases":["IFB","ELIXIR-FR","French Bioinformatics Institute"],"website":"https://www.france-bioinformatique.fr","type":"infrastructure","scope":"french","domain":["genomics","multimodal"],"status":"active","founded":2012,"parent_org":"Investissements d'Avenir PIA / ANR","tags":["icm/uses"]}}
---


# IFB - Institut Français de Bioinformatique (ELIXIR-FR)

## Overview
The Institut Français de Bioinformatique is the French national bioinformatics infrastructure and the French node of [[Governance/ELIXIR\|ELIXIR]] (ELIXIR-FR). Founded in 2012 under the Investissements d'Avenir programme, IFB federates 20+ bioinformatics platforms across France, providing computing resources, data management tools, training, and FAIR data support to the life sciences research community. For [[Actors/Paris Brain Institute\|Paris Brain Institute]], IFB is the primary French infrastructure for genomics and bioinformatics pipelines, DMP tools, and FAIR compliance support  particularly relevant for neurogenomics research, multi-omics integration, and compliance with [[Governance/ANR Open Science Policy\|ANR Open Science Policy]] and [[Governance/EHDS\|EHDS]] data mandates. [[Actors/DAC\|DAC]] is member platform (https://www.ifb-elixir.fr/ifb-elixir-fr/nos-plateformes/dac/)

## Key Services and Tools

### Data Management and FAIR
- **DSW@IFB** (https://dsw.france-bioinformatique.fr) — IFB's own Data Stewardship Wizard instance, an ELIXIR Recommended Interoperability Resource. IFB uses DSW primarily for **collaborative development of thematic DMP templates** for French life sciences infrastructures (France BioImaging, France Génomique, ProFI, MetaboHUB, etc.) and to build machine-actionable DMPs for infrastructure platforms. Free for academic users. Distinct from DMP OPIDoR (see below).
- **DMP OPIDoR** — IFB **recommends** DMP OPIDoR (https://dmp.opidor.fr), which is hosted and operated by INIST-CNRS (not by IFB), as the primary DMP tool for French researchers writing project DMPs for ANR and other funders. IFB's maDMP4LS project has developed programmatic integration between DSW@IFB and DMP OPIDoR so that DMP data can flow between the two systems.
- **FAIR-Checker** (https://fair-checker.france-bioinformatique.fr) — automated FAIR assessment tool for digital resources; developed by IFB, contributing to [[Governance/ELIXIR\|ELIXIR]] FAIR services
- **Cat OPIDoR** — IFB's services are listed in Cat OPIDoR (the national RDM service catalogue operated by INIST-CNRS via [[Governance/OPIDoR\|OPIDoR]])

### Computing Infrastructure
- **National Network of Computing Resources (NNCR)** — distributed HPC infrastructure: IFB-core cloud (Lyon) and cluster (Orsay) plus 9 regional HPC platforms; open to French and international life sciences research
- **usegalaxy.fr** — French instance of the Galaxy open analysis platform, providing FAIR, reproducible bioinformatics workflows
- **MADBOT** — web dashboard for research data and metadata management

### Training
- Active training programme in bioinformatics, RDM, and FAIR principles;
  IFB is the primary organiser of French bioinformatics training events and
  contributes to [[Governance/ELIXIR\|ELIXIR]] TeSS (Training e-Support System)

## Position in the French Ecosystem
IFB is the operational life sciences bioinformatics node sitting between the policy layer ([[Governance/Ouvrir la Science\|Ouvrir la Science]], [[Governance/ANR Open Science Policy\|ANR Open Science Policy]]) and individual researchers. It translates FAIR and open science policy into concrete tools and compute infrastructure. It is a Disciplinary Competence Center within the [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] ecosystem for life sciences.

## Connections
- European node: [[Governance/ELIXIR\|ELIXIR]] (ELIXIR-FR)
- Disciplinary node: [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] (life sciences competence centre)
- DMP tools: DSW@IFB (IFB's own Data Stewardship Wizard instance for life sciences DMP template development); recommends [[Governance/OPIDoR\|OPIDoR]] DMP OPIDoR (operated by INIST-CNRS) for general project DMPs; interoperability between the two in development
- Policy alignment: [[Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[Governance/Ouvrir la Science\|Ouvrir la Science]], [[Governance/CNRS Open Science\|CNRS Open Science]]
- Umbrella: [[Governance/INBS\|INBS]] (French national biology/health infrastructure network)
- Partners: [[Governance/France BioImaging\|France BioImaging]], [[Governance/France Life Imaging\|France Life Imaging]], [[Actors/GA4GH\|GA4GH]] (genomics standards adoption)
- Develops FAIR tools: FAIR-Checker (automated [[Governance/FAIR Principles\|FAIR Principles]] assessment), [[Governance/OPIDoR\|OPIDoR]] DMP tooling, usegalaxy.fr reproducible workflows
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (bioinformatics, genomics, DMP support, FAIR compliance)


## Resources
- https://www.france-bioinformatique.fr
- https://fair-checker.france-bioinformatique.fr
- https://usegalaxy.fr
- https://rdmkit.elixir-europe.org/ifb_assembly (RDMkit IFB tool assembly)
