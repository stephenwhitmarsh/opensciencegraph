---
{"dg-publish":true,"permalink":"/platforms/snds/","tags":["icm/uses"],"dg-note-properties":{"name":"SNDS","aliases":["Système National des Données de Santé","National Health Data System","SNIIRAM"],"website":"https://www.health-data-hub.fr/page/acces-aux-donnees-du-snds","type":"repository","scope":"french","domain":["clinical","health"],"status":"active","founded":2017,"parent_org":"Health Data Hub / CNAM","tags":["icm/uses"]}}
---


# SNDS

## Overview
The Système National des Données de Santé (SNDS) is the French national health data system, covering virtually the entire French population (67+ million people). It consolidates claims data from health insurance (SNIIRAM), hospital discharge summaries (PMSI), causes of death (CépiDC), and disability data. It is the primary resource for large-scale epidemiological, pharmacological, and clinical research in France, and is governed and made accessible via the [[Governance/Health Data Hub\|Health Data Hub]].

## Scope and Coverage
- **Population**: ~99% of French residents; longitudinal follow-up possible since 2003
- **SNIIRAM** — health insurance reimbursement data: consultations, prescriptions, medical acts, devices; covers ambulatory care
- **PMSI** — Programme de Médicalisation des Systèmes d'Information; hospital stay records (diagnosis, procedures, DRGs) from all French hospitals
- **CépiDC** — cause-of-death data from INSERM's epidemiology centre
- **MDPH/CNSA** — disability compensation and care data (partial linkage)

## Data Access
- **Authorized research access** via the [[Governance/Health Data Hub\|Health Data Hub]] Datalab (secure processing environment; no data export)
- Access tiers: **Permanent access** (CNAM-approved standing committees, e.g. EPI-PHARE); **Project access** (requires CNIL authorisation + CESREES opinion for sensitive projects; INDS pathway); **Simplified access** for pre-approved uses (public health agencies, HAS)
- Data is pseudonymised (not anonymised); individual-level re-identification is prohibited

## Coding and Terminologies
- Diagnostic coding: [[Standards/ICD-10\|ICD-10]] / CIM-10 (PMSI and causes of death)
- Procedure coding: [[Standards/CCAM\|CCAM]] (PMSI) and NGAP (ambulatory acts)
- Drug coding: ATC (Anatomical Therapeutic Chemical) via CIS/CIP codes
- Laboratory: [[Standards/LOINC\|LOINC]] (in progress via ANS interoperability mandates)
- Rare diseases: [[Standards/ORDO\|ORDO]] codes used in rare disease PMSI module (PMSI-CMD)
- Standardisation pivot: [[Standards/OMOP CDM\|OMOP CDM]] (via [[Governance/Health Data Hub\|Health Data Hub]] Datalab transformation)

## Standards and Interoperability
- [[Standards/OMOP CDM\|OMOP CDM]] — HDH transforms SNDS extracts to OMOP for federated research
- [[Standards/HL7 FHIR\|HL7 FHIR]] — ANS-mandated interoperability profiles for future EHDS alignment
- [[Standards/DCAT\|DCAT]] / [[Standards/Dublin Core\|Dublin Core]] — dataset catalogue metadata for discoverability
- [[Governance/EHDS\|EHDS]] — SNDS is designated as the primary dataset for France's EHDS obligations; HDH is France's candidate HDAB (Health Data Access Body)

## Connections
- Hosted and governed by: [[Governance/Health Data Hub\|Health Data Hub]]
- Hospital data source: [[Governance/AP-HP\|AP-HP]] (PMSI contribution from Assistance Publique)
- Standards: [[Standards/ICD-10\|ICD-10]], [[Standards/CCAM\|CCAM]], [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/LOINC\|LOINC]], [[Standards/ORDO\|ORDO]]
- European context: [[Governance/EHDS\|EHDS]], [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/EOSC\|EOSC]]
- French governance: [[Governance/ANS\|ANS]], [[Governance/Ouvrir la Science\|Ouvrir la Science]], [[Governance/Code de la Sante Publique\|Code de la Sante Publique]]
- Relevant to [[Actors/Paris Brain Institute\|Paris Brain Institute]]: population-scale neurology and psychiatry cohorts, linkage with CENIR neuroimaging, AP-HP clinical data, pharmacoepidemiology

## Resources
- https://www.health-data-hub.fr/page/acces-aux-donnees-du-snds
- https://documentation-snds.health-data-hub.fr (community documentation portal)
- CNAM SNDS documentation: https://www.assurance-maladie.ameli.fr/etudes-et-statistiques/open-data
