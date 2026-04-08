---
{"dg-publish":true,"permalink":"/03-platforms/snds/","tags":["icm/uses"],"dg-note-properties":{"name":"SNDS","aliases":["Système National des Données de Santé","National Health Data System","SNIIRAM"],"website":"https://www.health-data-hub.fr/page/acces-aux-donnees-du-snds","type":"repository","scope":"french","domain":["clinical","health"],"status":"active","founded":2017,"parent_org":"Health Data Hub / CNAM","tags":["icm/uses"]}}
---


# SNDS

## Overview
The Système National des Données de Santé (SNDS) is the French national health data
system, covering virtually the entire French population (67+ million people). It
consolidates claims data from health insurance (SNIIRAM), hospital discharge summaries
(PMSI), causes of death (CépiDC), and disability data. It is the primary resource for
large-scale epidemiological, pharmacological, and clinical research in France, and is
governed and made accessible via the [[04_Governance/Health Data Hub\|Health Data Hub]].

## Scope and Coverage
- **Population**: ~99% of French residents; longitudinal follow-up possible since 2003
- **SNIIRAM** — health insurance reimbursement data: consultations, prescriptions,
  medical acts, devices; covers ambulatory care
- **PMSI** — Programme de Médicalisation des Systèmes d'Information; hospital stay
  records (diagnosis, procedures, DRGs) from all French hospitals
- **CépiDC** — cause-of-death data from INSERM's epidemiology centre
- **MDPH/CNSA** — disability compensation and care data (partial linkage)

## Data Access
- **Authorized research access** via the [[04_Governance/Health Data Hub\|Health Data Hub]] Datalab (secure processing
  environment; no data export)
- Access tiers:
  - **Permanent access** (CNAM-approved standing committees): e.g. EPI-PHARE
  - **Project access**: requires CNIL authorisation + CESREES opinion for sensitive
    projects; INDS pathway
  - **Simplified access** for pre-approved uses (public health agencies, HAS)
- Data is pseudonymised (not anonymised); individual-level re-identification is prohibited

## Coding and Terminologies
- Diagnostic coding: [[02_Standards/ICD-10\|ICD-10]] / CIM-10 (PMSI and causes of death)
- Procedure coding: [[02_Standards/CCAM\|CCAM]] (PMSI) and NGAP (ambulatory acts)
- Drug coding: ATC (Anatomical Therapeutic Chemical) via CIS/CIP codes
- Laboratory: [[02_Standards/LOINC\|LOINC]] (in progress via ANS interoperability mandates)
- Rare diseases: [[02_Standards/ORDO\|ORDO]] codes used in rare disease PMSI module (PMSI-CMD)
- Standardisation pivot: [[02_Standards/OMOP CDM\|OMOP CDM]] (via [[04_Governance/Health Data Hub\|Health Data Hub]] Datalab transformation)

## Standards and Interoperability
- [[02_Standards/OMOP CDM\|OMOP CDM]] — HDH transforms SNDS extracts to OMOP for federated research
- [[02_Standards/HL7 FHIR\|HL7 FHIR]] — ANS-mandated interoperability profiles for future EHDS alignment
- [[02_Standards/DCAT\|DCAT]] / [[02_Standards/Dublin Core\|Dublin Core]] — dataset catalogue metadata for discoverability
- [[04_Governance/EHDS\|EHDS]] — SNDS is designated as the primary dataset for France's EHDS obligations;
  HDH is France's candidate HDAB (Health Data Access Body)

## Connections
- Hosted and governed by: [[04_Governance/Health Data Hub\|Health Data Hub]]
- Hospital data source: [[04_Governance/AP-HP\|AP-HP]] (PMSI contribution from Assistance Publique)
- Standards: [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/ORDO\|ORDO]]
- European context: [[04_Governance/EHDS\|EHDS]], [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[04_Governance/EOSC\|EOSC]]
- French governance: [[04_Governance/ANS\|ANS]], [[04_Governance/Ouvrir la Science\|Ouvrir la Science]], [[04_Governance/Code de la Sante Publique\|Code de la Sante Publique]]
- Relevant to [[00_Core/Paris Brain Institute\|Paris Brain Institute]]: population-scale neurology and psychiatry
  cohorts, linkage with CENIR neuroimaging, AP-HP clinical data, pharmacoepidemiology

## Resources
- https://www.health-data-hub.fr/page/acces-aux-donnees-du-snds
- https://documentation-snds.health-data-hub.fr (community documentation portal)
- CNAM SNDS documentation: https://www.assurance-maladie.ameli.fr/etudes-et-statistiques/open-data
