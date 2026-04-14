---
{"dg-publish":true,"permalink":"/governance/ap-hp/","dg-note-properties":{"name":"Assistance Publique Hopitaux de Paris","aliases":["AP-HP"],"website":"https://www.aphp.fr","type":"infrastructure","scope":"french","domain":["clinical","health"],"status":"active","founded":1849,"parent_org":"French Ministry of Health"}}
---


# AP-HP - Assistance Publique Hopitaux de Paris

## Overview
AP-HP is the largest hospital system in Europe (39 hospitals, 100,000+ staff) and a founding partner of [[Actors/Paris Brain Institute\|Paris Brain Institute]] via Pitié-Salpêtrière Hospital. It operates the EDS AP-HP clinical data warehouse ([[Standards/OMOP CDM\|OMOP CDM]]) and is a major contributor to [[Governance/Health Data Hub\|Health Data Hub]].

## Key Infrastructure
- EDS AP-HP — Entrepôt de Données de Santé (OMOP CDM-based clinical data warehouse)
- CDW-AP-HP — [[Platforms/i2b2\|i2b2]]-based clinical data warehouse
- Biological resource centres (biobanks)
- REDCap network for clinical trial data collection
- CIC Neurosciences (at [[Actors/Paris Brain Institute\|Paris Brain Institute]]) — see [[Governance/CIC Neurosciences\|CIC Neurosciences]]

## Standards Used
- [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/DICOM\|DICOM]], [[Standards/SNOMED CT\|SNOMED CT]], [[Platforms/i2b2\|i2b2]], [[Standards/CDISC\|CDISC]]
- Diagnostic coding: [[Standards/ICD-10\|ICD-10]] / CIM-10 (PMSI billing, SNDS)
- Procedure coding: [[Standards/CCAM\|CCAM]] (PMSI billing)
- Lab results: [[Standards/LOINC\|LOINC]]
- Adverse events: [[Standards/MedDRA\|MedDRA]] (clinical trials)

## Connections
- French: [[Governance/Health Data Hub\|Health Data Hub]], [[Actors/Paris Brain Institute\|Paris Brain Institute]], [[Governance/CATI\|CATI]], [[Governance/Inserm Open Science\|Inserm Open Science]], [[Governance/data.gouv.fr\|data.gouv.fr]]
- European: [[Governance/ECRIN\|ECRIN]], [[Governance/BBMRI-ERIC\|BBMRI-ERIC]]

## Resources
- https://www.aphp.fr
- https://eds.aphp.fr
