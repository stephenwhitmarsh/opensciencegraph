---
{"dg-publish":true,"permalink":"/platforms/eds-ap-hp/","dg-note-properties":{"name":"Entrepôt de Données de Santé AP-HP","aliases":["EDS AP-HP","AP-HP Clinical Data Warehouse","Clinical Data Warehouse of Greater Paris University Hospitals"],"website":"https://eds.aphp.fr","type":"platform","scope":"french","domain":["clinical","health"],"status":"active","founded":2017,"parent_org":"AP-HP / Direction des Services Numériques"}}
---


# EDS AP-HP — Entrepôt de Données de Santé

## Overview
The EDS AP-HP (Entrepôt de Données de Santé de l'Assistance Publique – Hôpitaux de Paris) is one of the largest hospital clinical data warehouses in Europe, integrating administrative and medical data from the 38 establishments of [[Governance/AP-HP\|AP-HP]]. Authorised by [[Governance/CNIL\|CNIL]] since January 2017, it provides a unified, standardised research infrastructure for observational studies, cohort building, algorithm development, and AI applications in clinical medicine.

For [[Actors/Paris Brain Institute\|Paris Brain Institute]], the EDS AP-HP is a primary resource for neurological disease epidemiology and real-world data studies, leveraging the full Pitié-Salpêtrière patient population linked to ICM research cohorts.

## Scale (current figure)
- **19 million patients**
- **190 million medical reports**
- **1,372 million biology results**
- **42 million imaging exams**
- **83 million diagnoses**
- **93 million acts**
[Source](https://eds.aphp.fr/a-propos-eds/)
## Data Content
The EDS integrates structured and unstructured data from across AP-HP's hospital information systems:
- **Administrative data** — hospitalisations, consultations, diagnoses (PMSI), procedures ([[Standards/CCAM\|CCAM]]), billing
- **Biological data** — laboratory results ([[Standards/LOINC\|LOINC]]-coded)
- **Prescriptions and dispensing** — drug data ([[Standards/ATC\|ATC]] classification)
- **Clinical notes** — free-text medical reports (NLP-processed)
- **Imaging metadata** — links to [[Standards/DICOM\|DICOM]] imaging data
- **Diagnostic coding** — [[Standards/ICD-10\|ICD-10]] / CIM-10 (PMSI), [[Standards/SNOMED CT\|SNOMED CT]]

## Standards and Interoperability
Data is standardised to international standards: [[Standards/OMOP CDM\|OMOP CDM]] as the primary common data model, [[Standards/HL7 FHIR\|HL7 FHIR]] for API access, and medical terminologies including [[Standards/LOINC\|LOINC]], CIM-10 ([[Standards/ICD-10\|ICD-10]]), and [[Standards/ATC\|ATC]]. This standardisation enabled AP-HP to join the international 4CE consortium (Consortium for Clinical Characterization of COVID-19 by EHR) for federated international analyses during the pandemic.

## Tools and Access

### Cohort360
**Cohort360** (https://github.com/aphp/Cohort360) is the primary web interface for the EDS, allowing AP-HP clinicians and researchers to build patient cohorts using inclusion/exclusion criteria. It is open source, built on a [[Standards/HL7 FHIR\|HL7 FHIR]] API over the [[Standards/OMOP CDM\|OMOP CDM]] backend, and is in active production use.

### i2b2
The EDS also exposes data through an **[[Platforms/i2b2\|i2b2]]** interface, enabling federated queries compatible with the broader i2b2/SHRINE network, including the Cancéropôle Île-de-France network (AP-HP, [[Actors/Institut Curie\|Institut Curie]], [[Actors/Institut Pasteur\|Institut Pasteur]], Gustave Roussy).

### Datalab
The **Datalab** is a secure private workspace for data analysis, providing up to 5 CPU, 16 GB RAM, and 100 GB storage per project. It includes Jupyter notebooks, GitLab, Slurm, and HDFS/Hive, and is accessible remotely from anywhere via double authentication. Additional AI tools are available including EDS-NLP and EDS-Scikit for medical text and tabular data analysis. Described at https://eds.aphp.fr/nos-produits/.

## Governance and Access
- **Comité de pilotage stratégique** — defines the EDS strategy and roadmap; meets bimonthly; includes medical, paramedical, scientific, executive and patient representatives
- **CSE** (Comité Scientifique et Éthique) — reviews and approves all research projects; external partner access decisions within 2 months of complete dossier submission
- **CNIL authorisation** — research reuse authorised since January 2017
- **Patient opposition** — patients can opt out of research reuse at any time (https://eds.aphp.fr/formulaire-dopposition/)
- **External access** — requires AP-HP medical sponsor, URC feasibility review, CSE approval, and contractualisation before data access

## Connections
- Operated by: [[Governance/AP-HP\|AP-HP]] Direction des Services Numériques
- Regulatory authorisation: [[Governance/CNIL\|CNIL]] (since January 2017)
- Data model: [[Standards/OMOP CDM\|OMOP CDM]] (primary), [[Standards/HL7 FHIR\|HL7 FHIR]] (API layer)
- Query tools: Cohort360 (open source), [[Platforms/i2b2\|i2b2]]
- Terminologies: [[Standards/ICD-10\|ICD-10]], [[Standards/LOINC\|LOINC]], [[Standards/ATC\|ATC]], [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/CCAM\|CCAM]]
- Part of: [[Platforms/Health Data Hub\|Health Data Hub]] ecosystem (SNDS linkage for national health data access)
- National standardisation: EDS France 2030 common data model initiative ([[Standards/OMOP CDM\|OMOP CDM]], coordinated by [[Platforms/Health Data Hub\|Health Data Hub]])
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (neurological disease real-world data; Pitié-Salpêtrière patient population; linkage with [[Actors/Paris Brain Institute\|ICM]] research cohorts via [[Actors/iCRIN\|iCRIN]] and [[Actors/CIC Neurosciences\|CIC Neurosciences]])

## Resources
- https://eds.aphp.fr
- https://eds.aphp.fr/a-propos-eds/ (key figures and governance)
- https://panorama.eds.aphp.fr (data availability panorama)
- https://eds.aphp.fr/nos-produits/ (Cohort360, Datalab, tools)
- https://github.com/aphp/Cohort360 (Cohort360 — open source cohort builder)
- https://eds.aphp.fr/recherche-et-innovation-partenaires/ (external partner access guide)
- https://eds.aphp.fr/portail-de-transparence/ (transparency portal — all approved studies)
- https://eds.aphp.fr/calendrier-du-cse/ (CSE calendar)
