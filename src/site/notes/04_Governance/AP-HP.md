---
{"dg-publish":true,"permalink":"/04-governance/ap-hp/","dg-note-properties":{"name":"Assistance Publique Hopitaux de Paris","aliases":["AP-HP"],"website":"https://www.aphp.fr","type":"infrastructure","scope":"french","domain":["clinical","health"],"status":"active","founded":1849,"parent_org":"French Ministry of Health"}}
---


# AP-HP - Assistance Publique Hopitaux de Paris

## Overview
AP-HP is the largest hospital system in Europe (39 hospitals, 100,000+ staff) and
a founding partner of [[00_Core/Paris Brain Institute\|Paris Brain Institute]] via Pitie-Salpetriere Hospital.
It operates the EDS AP-HP clinical data warehouse ([[02_Standards/OMOP CDM\|OMOP CDM]]) and is a major
contributor to [[04_Governance/Health Data Hub\|Health Data Hub]].

## Key Infrastructure
- EDS AP-HP - Entrepot de Donnees de Sante (OMOP CDM-based clinical data warehouse)
- CDW-AP-HP - [[04_Governance/i2b2\|i2b2]]-based clinical data warehouse
- Biological resource centres (biobanks)
- REDCap network for clinical trial data collection
- CIC Neurosciences (at [[00_Core/Paris Brain Institute\|Paris Brain Institute]])

## Standards Used
- [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/DICOM\|DICOM]], [[02_Standards/SNOMED CT\|SNOMED CT]], [[04_Governance/i2b2\|i2b2]], [[02_Standards/CDISC\|CDISC]]
- Diagnostic coding: [[02_Standards/ICD-10\|ICD-10]] / CIM-10 (PMSI billing, SNDS)
- Procedure coding: [[02_Standards/CCAM\|CCAM]] (PMSI billing)
- Lab results: [[02_Standards/LOINC\|LOINC]]
- Adverse events: [[02_Standards/MedDRA\|MedDRA]] (clinical trials)

## Connections
- French: [[04_Governance/Health Data Hub\|Health Data Hub]], [[00_Core/Paris Brain Institute\|Paris Brain Institute]], [[04_Governance/CATI\|CATI]],
  [[04_Governance/Inserm Open Science\|Inserm Open Science]], [[04_Governance/data.gouv.fr\|data.gouv.fr]]
- European: [[04_Governance/ECRIN\|ECRIN]], [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]]

## Resources
- https://www.aphp.fr
- https://eds.aphp.fr

