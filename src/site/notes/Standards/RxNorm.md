---
{"dg-publish":true,"permalink":"/standards/rx-norm/","dg-note-properties":{"name":"RxNorm","aliases":["RxNorm","NLM Drug Terminology"],"website":"https://www.nlm.nih.gov/research/umls/rxnorm/","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":2001,"parent_org":"US National Library of Medicine (NLM)"}}
---


# RxNorm — NLM Drug Terminology

## Overview
RxNorm is a normalised naming system for clinical drugs produced and maintained by the US National Library of Medicine (NLM). It provides standard names and identifiers for medications at the clinical level — drug ingredients, strengths, dose forms, and branded/generic names — and links them to many drug vocabularies commonly used in pharmacy management and drug interaction software. RxNorm is the primary drug terminology used in [[Standards/OMOP CDM\|OMOP CDM]] medication records, making it directly relevant to any institution using OMOP for clinical data standardisation, including [[Governance/AP-HP\|AP-HP]] and [[Platforms/Health Data Hub\|Health Data Hub]] in France.

## Concept Hierarchy
RxNorm organises drug concepts into a hierarchy from most general to most specific:

- **Ingredient** — active moiety (e.g. levodopa, carbidopa)
- **Clinical Drug Component** — ingredient + strength (e.g. levodopa 100 mg)
- **Clinical Drug Form** — ingredient + dose form (e.g. levodopa oral tablet)
- **Clinical Drug** — ingredient + strength + dose form (e.g. levodopa 100 mg oral tablet)
- **Branded Drug** — trade name versions (e.g. Sinemet)
- **Clinical Pack / Branded Pack** — multi-drug combination products

## Role in Clinical Data Standards
- **[[Standards/OMOP CDM\|OMOP CDM]]** — RxNorm is the standard drug vocabulary in OMOP; all medication records are mapped to RxNorm concept IDs via the OMOP Vocabulary (browsable at https://athena.ohdsi.org). The ATC (Anatomical Therapeutic Chemical) classification is used alongside RxNorm for drug class grouping.
- **[[Standards/HL7 FHIR\|HL7 FHIR]]** — RxNorm codes used in Medication and MedicationRequest resources as the standard US drug terminology; in European contexts SNOMED CT drug concepts or national terminologies are used alongside RxNorm
- **[[Platforms/Health Data Hub\|Health Data Hub]]** — French SNDS uses the UCD (Unité Commune de Dispensation) code system for drug dispensation data; mapping to RxNorm is performed via OMOP vocabulary for international interoperability
- **Clinical NLP** — RxNorm is a standard target for medication extraction from clinical notes (e.g. via cTAKES, MedSpaCy)

## French Context
France uses its own drug coding systems in administrative health data: **UCD** (Unité Commune de Dispensation — hospital drug dispensation), **CIS** (Code Identifiant de Spécialité — drug product identifier, ANSM), and **ATC** (WHO Anatomical Therapeutic Chemical classification). These are mapped to RxNorm within [[Standards/OMOP CDM\|OMOP CDM]] deployments at [[Governance/AP-HP\|AP-HP]] and [[Platforms/Health Data Hub\|Health Data Hub]] to enable international federated analyses.

## Connections
- Produced by: US National Library of Medicine (NLM) / UMLS
- Used in: [[Standards/OMOP CDM\|OMOP CDM]] (primary drug vocabulary), [[Standards/HL7 FHIR\|HL7 FHIR]] (medication resources)
- Complements: [[Standards/ChEBI\|ChEBI]] (chemical layer), [[Standards/SNOMED CT\|SNOMED CT]] (clinical findings), [[Standards/LOINC\|LOINC]] (lab tests), ATC (drug class grouping)
- French mapping: UCD/CIS → RxNorm via OMOP vocabulary
- Relevant to: [[Governance/AP-HP\|AP-HP]], [[Platforms/Health Data Hub\|Health Data Hub]], [[Actors/Paris Brain Institute\|Paris Brain Institute]] (clinical trial drug coding, OMOP CDM medication records)

## Resources
- https://www.nlm.nih.gov/research/umls/rxnorm/
- https://mor.nlm.nih.gov/RxNav/ (RxNav browser)
- https://athena.ohdsi.org (OMOP Vocabulary including RxNorm)
