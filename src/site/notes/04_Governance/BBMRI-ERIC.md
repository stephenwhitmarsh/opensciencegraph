---
{"dg-publish":true,"permalink":"/04-governance/bbmri-eric/","tags":["icm/participates"],"dg-note-properties":{"name":"Biobanking and Biomolecular Resources Research Infrastructure","aliases":["BBMRI-ERIC","BBMRI"],"website":"https://www.bbmri-eric.eu","type":"infrastructure","scope":"european","domain":["clinical","genomics"],"status":"active","founded":2013,"parent_org":"ESFRI / EU Member States","tags":["icm/participates"]}}
---


# BBMRI-ERIC — Biobanking and Biomolecular Resources Research Infrastructure

## Overview
BBMRI-ERIC (Biobanking and Biomolecular Resources Research Infrastructure — European Research Infrastructure Consortium) is the European research infrastructure for biobanking, connecting national biobank networks across 20+ member countries to enable standardised biological sample and data sharing for biomedical research. Established as an ERIC in 2013 under ESFRI coordination, BBMRI-ERIC provides the governance, standards, and IT infrastructure that allow researchers to discover, access, and use biological samples and associated data from biobanks across Europe.

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], BBMRI-ERIC is directly relevant through the [[01_Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] — ICM's biobank which operates within the French BIOBANQUES node of BBMRI-ERIC — and through [[01_Actors/Institut de Myologie\|Institut de Myologie]]'s Myobank-AFM, which also participates in the BBMRI-ERIC network.

## Structure

### National Nodes
BBMRI-ERIC operates through national nodes in each member country: **BBMRI-ERIC.fr (BIOBANQUES)** — French national node; federates French biobanks including AP-HP biological resource centres and research biobanks; **BBMRI-ERIC.nl** — Netherlands; includes population biobanks (Lifelines, Netherlands Twin Register); **BBMRI-ERIC.de** — Germany; German Biobank Alliance; **BBMRI-ERIC.uk** — UK; includes UK Biobank; **BBMRI-ERIC.se** — Sweden (coordinating country and HQ in Graz, Austria).

### Key Services and Tools
- **BBMRI-ERIC Directory** — federated catalogue of European biobanks and collections; searchable via https://directory.bbmri-eric.eu; enables researchers to find samples matching their inclusion criteria
- **BBMRI-ERIC Negotiator** — access negotiation platform connecting researchers with biobank data access committees; implements [[01_Actors/GA4GH\|GA4GH]] DUO for consent terms
- **GBA (Generic Biobank Application)** — open-source biobank LIMS (Laboratory Information Management System) for sample tracking and management

## Data and Metadata Standards
BBMRI-ERIC promotes standardised metadata and data models across its network: **MIABIS (Minimum Information About BIobank data Sharing)** — the BBMRI-ERIC metadata standard for describing biobanks, sample collections, and study designs; **[[02_Standards/OMOP CDM\|OMOP CDM]]** — recommended common data model for clinical/phenotypic data associated with biobank samples; **[[02_Standards/HL7 FHIR\|HL7 FHIR]]** — used for clinical data exchange between biobanks and EHR systems; **[[02_Standards/VCF\|VCF]]** — for genomic variant data; **[[02_Standards/Phenopackets\|Phenopackets]]** (GA4GH) — for structured phenotype-genotype descriptions.

## ESFRI Cluster
BBMRI-ERIC is part of the ESFRI Health and Food Research Infrastructure cluster together with [[04_Governance/ELIXIR\|ELIXIR]], [[04_Governance/EATRIS\|EATRIS]], [[04_Governance/ECRIN\|ECRIN]], and [[04_Governance/Euro-BioImaging\|Euro-BioImaging]]. These five ERICs collaborate on integrated life science research infrastructure for translational medicine.

## Connections
- French node: BIOBANQUES (federates French biobanks including [[01_Actors/Banque ADN et Cellules\|Banque ADN et Cellules]])
- ICM connection: [[01_Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] (neurology biobank), [[01_Actors/Institut de Myologie\|Institut de Myologie]] (Myobank-AFM — neuromuscular biobank)
- ESFRI cluster: [[04_Governance/ELIXIR\|ELIXIR]], [[04_Governance/EATRIS\|EATRIS]], [[04_Governance/ECRIN\|ECRIN]], [[04_Governance/Euro-BioImaging\|Euro-BioImaging]]
- Standards: [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/VCF\|VCF]], [[02_Standards/Phenopackets\|Phenopackets]], MIABIS
- Access governance: [[01_Actors/GA4GH\|GA4GH]] DUO (Data Use Ontology) for consent term machine-reading
- Partners: [[04_Governance/Health Data Hub\|Health Data Hub]], [[01_Actors/UK Biobank\|UK Biobank]], [[04_Governance/EOSC\|EOSC]], [[01_Actors/GA4GH\|GA4GH]]
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (Banque ADN et Cellules BBMRI integration; sample discovery for neurological disease research)

## Resources
- https://www.bbmri-eric.eu
- https://directory.bbmri-eric.eu (BBMRI-ERIC Directory — biobank catalogue)
- https://negotiator.bbmri-eric.eu (Negotiator — access request platform)
- https://www.miabis.net (MIABIS metadata standard)
