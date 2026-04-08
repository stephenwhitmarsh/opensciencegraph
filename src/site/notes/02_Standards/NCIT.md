---
{"dg-publish":true,"permalink":"/02-standards/ncit/","dg-note-properties":{"name":"NCI Thesaurus","aliases":["NCIT","NCIt","NCI Thesaurus"],"website":"https://ncithesaurus.nci.nih.gov","type":"terminology","scope":"international","domain":["clinical","genomics"],"status":"active","founded":2003,"parent_org":"National Cancer Institute (NCI) / US National Institutes of Health"}}
---


# NCIT — NCI Thesaurus

## Overview
The NCI Thesaurus (NCIt) is a reference terminology produced by the US National Cancer Institute covering the biomedical and clinical domains with particular depth in oncology, clinical trials, and biomedical research. With 170,000+ concepts and 370,000+ synonyms, it is one of the most comprehensive biomedical terminologies available, and is widely used in clinical trial data management, cancer registries, and regulatory submissions. NCIt is used in [[02_Standards/CDISC\|CDISC]] clinical trial standards, is mapped in [[02_Standards/OMOP CDM\|OMOP CDM]] vocabularies, and underpins the NCI Enterprise Vocabulary Services (EVS).

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], NCIt is relevant through clinical trial data management ([[02_Standards/CDISC\|CDISC]] SDTM uses NCIt as a controlled terminology source), neuro-oncology research, and its broad coverage of clinical research concepts that bridge oncology and neurology (brain tumours, neuroendocrine tumours, paraneoplastic syndromes).

## Key Concept Areas
- **Disease and conditions** — cancer diagnoses, benign tumours, syndromes; brain and CNS tumours covered in depth (WHO CNS tumour classification aligned)
- **Anatomy** — anatomical structures, organs, tumour sites
- **Drugs and agents** — chemotherapy agents, targeted therapies, biologics, radiopharmaceuticals; overlaps with [[02_Standards/ChEBI\|ChEBI]] and [[02_Standards/RxNorm\|RxNorm]]
- **Clinical trial concepts** — study design, endpoints, adverse event grades (CTCAE — Common Terminology Criteria for Adverse Events)
- **Genes and molecular targets** — gene names, biomarkers, molecular pathways
- **Procedures and interventions** — surgical procedures, imaging procedures

## Role in Clinical Data Standards
- **[[02_Standards/CDISC\|CDISC]]** — NCIt is the primary controlled terminology source for CDISC SDTM (Study Data Tabulation Model) and CDASH; clinical trial submissions to FDA/EMA use NCIt codes for intervention, indication, and adverse event coding
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — NCIt mapped in OMOP vocabulary for cancer and clinical research concepts; accessible via Athena (https://athena.ohdsi.org)
- **Cancer registries** — NCIt underpins the ICD-O (International Classification of Diseases for Oncology) mapping used in cancer surveillance
- **Regulatory** — FDA and EMA accept NCIt-coded controlled terminology in electronic clinical trial submissions

## Connections
- Produced by: NCI / NIH Enterprise Vocabulary Services (EVS)
- Used in: [[02_Standards/CDISC\|CDISC]] (SDTM controlled terminology), [[02_Standards/OMOP CDM\|OMOP CDM]] (vocabulary)
- Complements: [[02_Standards/SNOMED CT\|SNOMED CT]] (broader clinical), [[02_Standards/ICD-10\|ICD-10]] / [[02_Standards/ICD-11\|ICD-11]] (disease classification), [[02_Standards/MedDRA\|MedDRA]] (adverse events), [[02_Standards/ChEBI\|ChEBI]] / [[02_Standards/RxNorm\|RxNorm]] (drugs)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (clinical trials, neuro-oncology, CDISC submissions via [[04_Governance/ECRIN\|ECRIN]])

## Resources
- https://ncithesaurus.nci.nih.gov
- https://evs.nci.nih.gov (NCI Enterprise Vocabulary Services)
- https://obofoundry.org/ontology/ncit.html (OBO Foundry entry)
- https://athena.ohdsi.org (OMOP vocabulary including NCIt)
