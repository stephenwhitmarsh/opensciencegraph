---
{"dg-publish":true,"permalink":"/03-platforms/red-cap/","tags":["icm/uses"],"dg-note-properties":{"name":"REDCap","aliases":["Research Electronic Data Capture","REDCap+"],"website":"https://www.project-redcap.org","type":"platform","scope":"international","domain":["clinical"],"status":"active","founded":2004,"parent_org":"Vanderbilt University","tags":["icm/uses"]}}
---


# REDCap — Research Electronic Data Capture

## Overview
REDCap (Research Electronic Data Capture) is a secure, web-based software platform
for building and managing online surveys and databases for research and clinical
data collection. Developed at Vanderbilt University in 2004 and now supported by
a global consortium of 6,000+ institutional partners, REDCap is the de facto
standard electronic data capture (EDC) tool for academic clinical research and
clinical trials worldwide. It is used for eCRF (electronic Case Report Form) design,
longitudinal study management, survey distribution, and clinical data warehousing.

At [[00_Core/Paris Brain Institute\|Paris Brain Institute]], REDCap is used for clinical data management and is
supported by the [[01_Actors/DAC\|DAC]] (Data Analysis Core), which provides REDCap training and
helpdesk support to ICM researchers and clinicians.

## Key Features

### Data Collection
- **eCRF design** — drag-and-drop form builder with 18+ field types
  (text, numbers, dates, dropdowns, calculated fields, file uploads)
- **Branching logic** — conditional field display based on responses
- **Validation** — built-in range checks, date formats, regex patterns
- **Surveys** — public-facing survey mode for participant self-report
- **Repeating instruments** — longitudinal data collection with multiple visits

### Data Management
- **Audit trail** — complete change history for regulatory compliance
- **Data access groups** — role-based access control for multi-site studies
- **Field-level permissions** — granular read/edit rights per user
- **Data locking** — record locking for completed CRFs
- **e-Consent** — electronic informed consent module

### Import / Export
- Export to CSV, Excel, SPSS, SAS, Stata, R, CDISC ODM XML
- Import from Excel/CSV templates
- REDCap API — REST API for programmatic data access and integration
- FHIR endpoint (REDCap on FHIR) for [[02_Standards/HL7 FHIR\|HL7 FHIR]] interoperability

### Clinical Research Tools
- **Randomisation** — built-in randomisation module for clinical trials
- **Scheduling** — appointment tracking and visit management
- **Clinical Data Interoperability Services (CDIS)** — pulls data from
  EHR systems via HL7 FHIR
- **External modules** — community-developed extensions (500+)

## REDCap Consortium and Deployment
REDCap is free to non-profit institutions that join the REDCap consortium
(https://www.project-redcap.org). Each institution hosts its own REDCap server;
the consortium provides software updates, documentation, and community support.

In France:
- [[04_Governance/AP-HP\|AP-HP]] operates REDCap instances for clinical data collection across its hospitals
- [[04_Governance/ECRIN\|ECRIN]] operates a GDPR-compliant REDCap instance available to
  ECRIN-supported multinational clinical studies
- [[00_Core/Paris Brain Institute\|Paris Brain Institute]] / [[01_Actors/DAC\|DAC]] runs an institutional REDCap instance
  supporting ICM research teams

## Standards Alignment
- **[[02_Standards/CDISC\|CDISC]]** — REDCap exports to CDISC ODM (Operational Data Model) XML;
  complements SDTM/ADaM pipelines
- **[[02_Standards/HL7 FHIR\|HL7 FHIR]]** — REDCap on FHIR enables bidirectional EHR data exchange
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — REDCap data can be mapped to OMOP CDM via ETL pipelines

## Connections
- Support at ICM: [[01_Actors/DAC\|DAC]] (REDCap training, helpdesk, instance management)
- Deployed at: [[04_Governance/AP-HP\|AP-HP]], [[04_Governance/ECRIN\|ECRIN]] (multinational trials instance)
- Standards: [[02_Standards/CDISC\|CDISC]] (ODM XML export), [[02_Standards/HL7 FHIR\|HL7 FHIR]] (CDIS module)
- Complements: [[02_Standards/OMOP CDM\|OMOP CDM]] (downstream ETL from REDCap to OMOP)
- Related platforms: [[03_Platforms/LORIS\|LORIS]] (neuroimaging-specific equivalent),
  [[03_Platforms/XNAT\|XNAT]] (imaging data management)
- Used in training: [[01_Actors/DAC\|DAC]] training programme (REDCap sessions Jan–Mar 2026)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (clinical study data collection,
  eCRF management, longitudinal cohort tracking)

## Resources
- https://www.project-redcap.org (REDCap consortium — software and documentation)
- https://redcap.vanderbilt.edu (Vanderbilt REDCap home)
- https://projectredcap.org/resources/videos/ (training videos)
