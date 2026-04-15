---
{"dg-publish":true,"permalink":"/standards/osiris/","dg-note-properties":{"name":"OSIRIS","aliases":["Interoperability and data sharing of clinical and biological data in Oncology"],"website":"https://ig-osiris.cancer.fr/ig/osiris/","type":"standard","scope":"french","domain":["clinical","genomics"],"status":"active","founded":2015,"parent_org":"INCa (Institut National du Cancer)","tags":null}}
---


# OSIRIS

## Overview
OSIRIS (Interoperability and data sharing of clinical and biological data in Oncology) is a French national minimum data set and Common Data Model for clinical and genomic data sharing in oncology, developed through a bottom-up national consensus process launched in 2015. Funded by INCa (the French National Cancer Institute), it was built by a task force of Integrated Cancer Research Sites (SIRICs), comprehensive cancer centres (Unicancer network), and university hospitals. The resulting model specifies 67 clinical items and 65 omics items in an event-based data model that captures longitudinal disease course, treatment, and genomic findings in precision medicine trials. OSIRIS is aligned with [[Standards/HL7 FHIR\|HL7 FHIR]] (a full FHIR R4 Implementation Guide exists), approved by a National Plan Strategic Committee, and freely released.

## Scope and Model
The OSIRIS event-based data model organises data around Treatment Plan Episodes (TPEs) — clinical moments anchored to treatment decisions — and captures:
- **Patient characteristics** — demographics, family history, clinical trial participation
- **Disease characteristics** — ICD-O-3 tumour histology, ICD-10 diagnosis coding
- **Treatment** — drug administration, surgical procedures, radiotherapy, adverse events
- **Genomics** — sequencing analysis, SNVs, copy number variants, fusions, annotations
- **Response evaluation** — RECIST, biomarker measurements
- **Imaging** — radiomics, imaging study metadata

## Terminologies Used
OSIRIS relies on international standards throughout:
- Diagnosis: [[Standards/ICD-10\|ICD-10]] (CIM-10), ICD-O-3
- Drugs: [[Standards/RxNorm\|RxNorm]], [[Standards/ATC\|ATC]] (Anatomical Therapeutic Chemical)
- Adverse events: [[Standards/MedDRA\|MedDRA]]
- Clinical data exchange: [[Standards/HL7 FHIR\|HL7 FHIR]] R4
- Genomics: [[Standards/VCF\|VCF]], [[Standards/OMOP CDM\|OMOP CDM]] (ETL mapping underway)
- Interoperability: [[Platforms/i2b2\|i2b2]] CDM (ETL demonstrated in proof-of-concept)

## Key Features
- Modular and extensible — core oncology model can be extended to specific cancer types
- Supports retrospective and prospective data from EHRs, eCRFs, data warehouses, and cancer registries
- FHIR Implementation Guide v1.1.0 published at ig-osiris.cancer.fr
- GDPR-compliant by design; reviewed by CNIL
- Proof-of-concept demonstrated on 300-patient cohort across multiple French cancer centres

## Connections
- Funded by: INCa (Institut National du Cancer)
- Core contributors: [[Actors/Institut Curie\|Institut Curie]], Institut Bergonié, Centre Léon Bérard; AP-HP HEGP
- French governance: [[Governance/Code de la Sante Publique\|Code de la Sante Publique]], CNIL, [[Governance/ANS\|ANS]]
- Standards: [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/ICD-10\|ICD-10]], [[Standards/MedDRA\|MedDRA]], [[Standards/RxNorm\|RxNorm]], [[Standards/ATC\|ATC]], [[Standards/OMOP CDM\|OMOP CDM]], [[Platforms/i2b2\|i2b2]]
- Related French oncology infrastructure: SIRICs, Unicancer, [[Governance/Health Data Hub\|Health Data Hub]]
- Relevant to [[Actors/Paris Brain Institute\|Paris Brain Institute]]: neuro-oncology data sharing context; OSIRIS is the French standard for multi-centre cancer genomics trials

## Resources
- FHIR IG: https://ig-osiris.cancer.fr/ig/osiris/
- Publication: https://pmc.ncbi.nlm.nih.gov/articles/PMC8140800/
- INCa: https://www.e-cancer.fr
