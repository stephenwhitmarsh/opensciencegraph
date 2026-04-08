---
{"dg-publish":true,"permalink":"/04-governance/ans/","dg-note-properties":{"name":"Agence du Numerique en Sante","aliases":["ANS","Agence du Numérique en Santé"],"website":"https://esante.gouv.fr","type":"infrastructure","scope":"french","domain":["clinical","health"],"status":"active","founded":2019,"parent_org":"French Ministry of Health (Direction Générale de l'Offre de Soins)"}}
---


# ANS — Agence du Numérique en Santé

## Overview
The Agence du Numérique en Santé (ANS) is the French national agency responsible for developing and coordinating digital health standards, interoperability frameworks, and health information systems in France. Created in 2019 from the merger of the former ASIP Santé and the digital health mission of the DGOS (Direction Générale de l'Offre de Soins), ANS operates under the French Ministry of Health and is the French national competent body for health IT standardisation.

ANS is directly relevant to [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] and the broader French neuroscience research community because it manages the French national release of [[02_Standards/SNOMED CT\|SNOMED CT]], publishes French national [[02_Standards/HL7 FHIR\|HL7 FHIR]] Implementation Guides (IGs) and profiles, operates the **interoperability framework** (CI-SIS) that defines how French health information systems must exchange data, and is the national HDAB candidate for [[04_Governance/EHDS\|EHDS]] implementation in France.

## Key Responsibilities

### French SNOMED CT National Release Centre
ANS is France's **SNOMED International National Release Centre (NRC)**: it maintains the French-language translation of [[02_Standards/SNOMED CT\|SNOMED CT]] concepts, publishes the French National Release of SNOMED CT (fr-FR), provides French clinical terms and preferred synonyms for all SNOMED CT concepts, and coordinates SNOMED CT adoption in French EHR systems and clinical coding.

### HL7 FHIR National Implementation Guides
ANS publishes French national [[02_Standards/HL7 FHIR\|HL7 FHIR]] profiles and Implementation Guides (IGs): **CI-SIS FHIR** — the French interoperability framework FHIR profiles; profiles for specific French use cases including hospitalisation summary, medication reconciliation, biological results, and vaccination records. ANS FHIR IGs are available at https://interop.esante.gouv.fr. France primarily uses **FHIR R4**; ANS manages the transition timeline.

### CI-SIS — Cadre d'Interopérabilité des Systèmes d'Information de Santé
The **CI-SIS** is France's master interoperability framework for health information systems, specifying which standards are mandatory for French health IT systems ([[02_Standards/HL7 FHIR\|HL7 FHIR]] R4, [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/DICOM\|DICOM]], HL7 v2, CDA), French national profiles and extensions on international standards, and implementation guidance for specific clinical use cases.

### Espace Numérique de Santé (ENS) / Mon Espace Santé
ANS operates France's national patient health portal (**Mon Espace Santé**) and coordinates the **Espace Numérique de Santé** — the French national personal health record system, which stores patient documents in [[02_Standards/HL7 FHIR\|HL7 FHIR]] format and is accessible to all French citizens.

### EHDS National HDAB
ANS is the designated national health data access body (**HDAB**) candidate for France under [[04_Governance/EHDS\|EHDS]] (European Health Data Space), responsible for managing secondary use access to French health data in the EHDS framework — working alongside [[04_Governance/Health Data Hub\|Health Data Hub]] which currently handles the operational SNDS access.

## Connections
- Manages: French [[02_Standards/SNOMED CT\|SNOMED CT]] NRC (National Release Centre)
- Publishes: French [[02_Standards/HL7 FHIR\|HL7 FHIR]] IGs (CI-SIS FHIR profiles)
- Operates: Mon Espace Santé (French national health portal, FHIR-based)
- Framework: CI-SIS (French health IT interoperability framework)
- Partners: [[04_Governance/Health Data Hub\|Health Data Hub]] (SNDS data access), [[04_Governance/AP-HP\|AP-HP]] (largest French hospital)
- European: [[04_Governance/EHDS\|EHDS]] national HDAB candidate; European eHealth Network
- Standards managed: [[02_Standards/SNOMED CT\|SNOMED CT]] (French NRC), [[02_Standards/HL7 FHIR\|HL7 FHIR]] (French profiles), [[02_Standards/LOINC\|LOINC]], [[02_Standards/ICD-10\|ICD-10]] (CIM-10 French version)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (French FHIR profiles for clinical data; SNOMED CT French terms for AP-HP EDS; EHDS secondary use framework)

## Resources
- https://esante.gouv.fr
- https://interop.esante.gouv.fr (ANS FHIR IGs and CI-SIS)
- https://www.monespacesante.fr (Mon Espace Santé — French national health portal)
- https://esante.gouv.fr/produits-services/espace-numerique-de-sante (ENS programme)
