---
{"dg-publish":true,"permalink":"/02-standards/snomed-ct/","tags":["icm/uses"],"dg-note-properties":{"name":"SNOMED International Clinical Terms","aliases":["SNOMED CT","SNOMED"],"website":"https://www.snomed.org","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":1999,"parent_org":"SNOMED International","tags":["icm/uses"],"icon":"https://www.snomed.org/favicon.ico"}}
---


# SNOMED CT — Systematized Nomenclature of Medicine Clinical Terms

## Overview
SNOMED CT is the world's most comprehensive and widely used clinical healthcare
terminology, maintained by SNOMED International (an international non-profit
organisation). It contains over 350,000 active concepts covering diseases,
clinical findings, procedures, body structures, substances, organisms, and
observable entities — all described with formal, machine-readable definitions
and organised in a polyhierarchical structure.

SNOMED CT is the core clinical terminology for [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]],
and [[02_Standards/openEHR\|openEHR]], making it the foundational vocabulary layer for health data
interoperability globally. France joined SNOMED International in 2023, enabling
French health organisations including [[04_Governance/AP-HP\|AP-HP]] to use SNOMED CT under the
international licence — directly relevant to the [[04_Governance/Health Data Hub\|Health Data Hub]] and [[04_Governance/EHDS\|EHDS]]
ecosystem.

## History
- **1965** — SNOMED precursor (SNOP) created by the College of American Pathologists
- **1999** — SNOMED CT created by merger of SNOMED RT (College of American Pathologists)
  and Clinical Terms Version 3 (NHS UK)
- **2007** — SNOMED International (then IHTSDO) established as international governing body
- **2010+** — Adopted as mandatory terminology in UK, US, Australia, Canada, Nordic countries
- **2023** — France joins SNOMED International; ANS coordinates French National Release Centre

## Concept Model
SNOMED CT uses a **description logic** model in which every concept is formally defined
by its relationships to other concepts:

- **Concepts** — uniquely identified by a SCTID (e.g. `73211009` = Diabetes mellitus)
- **Descriptions** — human-readable names for concepts (Fully Specified Name, Preferred Term,
  Synonyms)
- **Relationships** — typed semantic links between concepts (IS-A for hierarchy, attribute
  relationships for clinical meaning)

Key concept hierarchies relevant to neuroscience:
- **Clinical finding** (404684003) — diseases, symptoms, signs; includes all neurological disorders
- **Procedure** (71388002) — clinical procedures including neuroimaging, EEG, surgery
- **Body structure** (123037004) — anatomy including brain regions, cranial nerves
- **Substance** (105590001) — drugs, neurotransmitters, biomarkers
- **Observable entity** (363787002) — lab tests, measurements, cognitive assessments

## SNOMED CT in France
- **ANS (Agence du Numérique en Santé)** manages the French National Release Centre (NRC)
- French National Release provides French-language translations and France-specific extensions
- Mandated for use in French EHR systems under the ANS interoperability framework
- [[04_Governance/AP-HP\|AP-HP]] EDS (Entrepôt de Données de Santé) maps clinical data to SNOMED CT
- [[02_Standards/OMOP CDM\|OMOP CDM]] deployments at [[04_Governance/Health Data Hub\|Health Data Hub]] use SNOMED CT as the primary
  condition and procedure vocabulary (via Athena)

## Role in the Data Ecosystem

| System | SNOMED CT role |
|---|---|
| [[02_Standards/OMOP CDM\|OMOP CDM]] | Primary vocabulary for conditions, procedures, observations (domain: Condition, Procedure) |
| [[02_Standards/HL7 FHIR\|HL7 FHIR]] | Coded values in Condition, Procedure, Observation, AllergyIntolerance resources |
| [[02_Standards/openEHR\|openEHR]] | Archetype term bindings; preferred terminology for clinical concepts |
| [[04_Governance/Health Data Hub\|Health Data Hub]] | Core terminology for EDS semantic standardisation |
| [[04_Governance/EHDS\|EHDS]] | Mandated as primary clinical terminology for European health data spaces |

## Connections
- Integrated into: [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/openEHR\|openEHR]], [[04_Governance/Health Data Hub\|Health Data Hub]]
- Used by: [[04_Governance/AP-HP\|AP-HP]] (EDS), [[04_Governance/ECRIN\|ECRIN]] (clinical trials), [[04_Governance/EHDS\|EHDS]] member states
- Mandated by: [[04_Governance/EHDS\|EHDS]] (core clinical terminology for EHR content)
- Maps to: [[02_Standards/ICD-10\|ICD-10]] / [[02_Standards/ICD-11\|ICD-11]] (official WHO cross-maps maintained by SNOMED International)
- Maps to: [[02_Standards/LOINC\|LOINC]] (complementary — SNOMED for findings/procedures, LOINC for lab tests)
- Harmonised by: [[02_Standards/MONDO\|MONDO]] (SNOMED disease concepts integrated into unified ontology)
- Related: [[02_Standards/HPO\|HPO]] (phenotype layer — more granular for rare disease genomics)
- French coordination: ANS (Agence du Numérique en Santé) — NRC France
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (OMOP CDM clinical data standardisation,
  AP-HP EDS linkage, EHDS compliance)

## Resources
- https://www.snomed.org
- https://browser.ihtsdotools.org (SNOMED CT browser)
- https://www.snomed.org/snomed-ct/get-snomed (licensing and national releases)
- https://esante.gouv.fr/terminologies (ANS — French NRC)
