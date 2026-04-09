---
{"dg-publish":true,"permalink":"/standards/hl-7-fhir/","tags":["icm/uses"],"dg-note-properties":{"name":"Fast Healthcare Interoperability Resources","aliases":["HL7 FHIR","FHIR","FHIR R4","FHIR R5"],"website":"https://hl7.org/fhir/","type":"standard","scope":"international","domain":["clinical","health"],"status":"active","founded":2011,"parent_org":"HL7 International","tags":["icm/uses"],"icon":"https://hl7.org/favicon.ico"}}
---


# HL7 FHIR — Fast Healthcare Interoperability Resources

## Overview
HL7 FHIR (Fast Healthcare Interoperability Resources) is the modern standard for electronic health data exchange, developed by HL7 International and first published in 2011. FHIR uses RESTful APIs, JSON/XML/Turtle serialisation, and a modular **resource** model to enable systems to exchange health data in a standardised, machine-readable way. It is now the dominant health interoperability standard globally and is mandated by the [[Governance/EHDS\|EHDS]] for European health data spaces, by the US ONC 21st Century Cures Act, and by national health IT agencies in France (ANS), the UK (NHS England), and Australia (ADHA).

## Resource Model
FHIR organises all health information into **Resources** — discrete units of clinical information, each with a defined structure, mandatory/optional fields, and a REST API endpoint. There are 150+ resources covering all clinical domains. Key resources relevant to neuroscience research:

- **Patient** — demographic and administrative information
- **Condition** — diagnoses and clinical problems (coded with [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/ICD-10\|ICD-10]])
- **Observation** — lab results, vitals, cognitive assessments (coded with [[Standards/LOINC\|LOINC]])
- **Procedure** — clinical procedures (coded with [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/CCAM\|CCAM]])
- **MedicationRequest** / **MedicationAdministration** — drug prescriptions and administration
- **ImagingStudy** — link to [[Standards/DICOM\|DICOM]] imaging studies; references WADO-RS endpoints
- **DiagnosticReport** — structured clinical report (radiology, pathology)
- **ResearchStudy** / **ResearchSubject** — clinical trial metadata (alignment with [[Standards/CDISC\|CDISC]])
- **Consent** — patient consent records (important for [[Governance/EHDS\|EHDS]] secondary use)
- **DocumentReference** — links to unstructured documents (discharge summaries, etc.)

## Versioning
FHIR has gone through several major versions:
- **DSTU2 / STU3** — widely deployed legacy versions
- **R4 (2019)** — current stable version; international baseline; used by [[Governance/EHDS\|EHDS]], NHS, ANS
- **R4B (2022)** — minor update; adds medication knowledge and clinical reasoning resources
- **R5 (2023)** — latest; improved data modelling, subscriptions, cross-version mapping

Most production deployments in France ([[Governance/AP-HP\|AP-HP]], [[Governance/Health Data Hub\|Health Data Hub]]) use **R4**.

## SMART on FHIR
**SMART on FHIR** (Substitutable Medical Applications, Reusable Technologies) is the OAuth2/OpenID Connect-based authorisation framework built on top of FHIR, enabling third-party applications to securely access patient data from FHIR servers with patient/clinician consent. It is the standard for EHR app ecosystems (Epic, Cerner, Oracle Health) and is used in clinical research portal applications.

## FHIR in France
- **ANS** (Agence du Numérique en Santé) publishes French national FHIR Implementation Guides (IGs) — profiles that constrain FHIR resources to French healthcare context
- **AP-HP EDS** exposes some data via FHIR R4 endpoints; the Hôpital Numérique programme requires FHIR compliance
- **[[Governance/Health Data Hub\|Health Data Hub]]** uses FHIR as part of its interoperability framework alongside [[Standards/OMOP CDM\|OMOP CDM]] for secondary data use

## FHIR and OMOP
FHIR and [[Standards/OMOP CDM\|OMOP CDM]] serve complementary roles:
- **FHIR** — operational/clinical data exchange standard; real-time API access
- **OMOP CDM** — analytical standard for retrospective research; batch ETL from EHR
- ETL pipelines convert FHIR resources to OMOP tables (OHDSI provides FHIR-to-OMOP mapping tools); [[Governance/EHDS\|EHDS]] mandates both standards for primary and secondary use respectively

## Connections
- Maps to: [[Standards/OMOP CDM\|OMOP CDM]] (ETL pathway), [[Standards/openEHR\|openEHR]] (bidirectional mapping), [[Standards/DICOM\|DICOM]] (ImagingStudy resource), [[Standards/CDISC\|CDISC]] (ResearchStudy / clinical trial data)
- Coded values use: [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/LOINC\|LOINC]], [[Standards/ICD-10\|ICD-10]], [[Standards/ICD-11\|ICD-11]], [[Standards/MedDRA\|MedDRA]]
- Adopted by: [[Governance/Health Data Hub\|Health Data Hub]], [[Governance/AP-HP\|AP-HP]], [[Governance/ECRIN\|ECRIN]], [[Platforms/i2b2\|i2b2]]
- Mandated by: [[Governance/EHDS\|EHDS]] (primary EHR interoperability standard across EU)
- French coordination: ANS (national FHIR IGs and profiles)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (AP-HP EDS FHIR access, EHDS compliance, clinical trial data integration)

## Resources
- https://hl7.org/fhir/ (FHIR R4 specification)
- https://hl7.org/fhir/R5/ (FHIR R5 specification)
- https://smarthealthit.org (SMART on FHIR)
- https://esante.gouv.fr/ans-nationale/convergences-fhir (ANS French FHIR IGs)
- https://github.com/OHDSI/ETL-CDMBuilder (FHIR to OMOP ETL)
