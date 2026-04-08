---
{"dg-publish":true,"permalink":"/03-platforms/clean-web/","dg-note-properties":{"name":"CleanWEB","aliases":["CleanWeb","Telemedicine Technologies CleanWEB"],"website":"https://tentelemed.com/clinical-research/","type":"platform","scope":"french","domain":["clinical"],"status":"active","founded":1999,"parent_org":"Telemedicine Technologies (Boulogne-Billancourt, France)"}}
---


# CleanWEB

## Overview
CleanWEB is a French electronic clinical trial management platform developed by Telemedicine Technologies (Boulogne-Billancourt), the leading eClinical SaaS provider in France. It provides a modular, GDPR-compliant suite for the electronic management of clinical studies and patient registries. Since 2003, AP-HP (Assistance Publique — Hôpitaux de Paris) has contracted with Telemedicine Technologies for institutional use of CleanWEB as the standard eCRF platform for its clinical trials, making it the de facto standard for AP-HP-sponsored research. It is functionally comparable to [[03_Platforms/REDCap\|REDCap]] but oriented toward regulatory-grade Phase I–IV clinical trials.

## Key Modules
- **eCRF** — electronic Case Report Form; the core module; supports CDASH/CDISC compliance
- **CTMS** — Clinical Trial Management System; project monitoring portal
- **eTMF** — electronic Trial Master File
- **eConsent** — electronic informed consent
- **Medical Imaging** — DICOM and non-DICOM upload, anonymisation, viewer; integrates with eCRF
- **IWRS/RTSM** — Interactive Web/Voice Response System; randomisation and trial supply management
- **Vigilance** — pharmacovigilance and adverse event reporting
- **Managed Access Programmes (MAP)** — compassionate use tracking
- **CT-SCOUT** — AI-assisted patient pre-screening and trial matching module

## Standards and Interoperability
- Regulatory: CDISC (CDASH, SDTM) compliance; supports direct SAS export
- Data exchange: [[02_Standards/HL7 FHIR\|HL7 FHIR]] integration (in development)
- Security: HDS (Hébergement de Données de Santé) certified hosting option; GDPR-compliant
- Available as SaaS or on-premise deployment

## Connections
- Primary institutional user: [[04_Governance/AP-HP\|AP-HP]] (contracted since 2003; standard eCRF for AP-HP DRCD)
- Clinical research context: [[04_Governance/ECRIN\|ECRIN]] (European network uses compatible eCRF standards)
- Standards: [[02_Standards/CDISC\|CDISC]] (CDASH/SDTM), [[02_Standards/MedDRA\|MedDRA]] (adverse event coding)
- Comparable tools: [[03_Platforms/REDCap\|REDCap]] (research/academic), CleanWEB (regulatory-grade trials)
- French governance: [[04_Governance/Code de la Sante Publique\|Code de la Sante Publique]], CNIL, [[04_Governance/ANS\|ANS]]
- Relevant to [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]: used widely across AP-HP-sponsored clinical trials; context for understanding the French clinical research eCRF ecosystem alongside [[03_Platforms/REDCap\|REDCap]]

## Resources
- https://tentelemed.com/clinical-research/
- https://tentelemed.com/cleanweb/ (French)
