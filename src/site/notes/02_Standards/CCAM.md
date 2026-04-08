---
{"dg-publish":true,"permalink":"/02-standards/ccam/","tags":["icm/uses"],"dg-note-properties":{"name":"Classification Commune des Actes Médicaux","aliases":["CCAM"],"website":"https://www.atih.sante.fr/les-nomenclatures-de-facturation/ccam","type":"terminology","scope":"french","domain":["clinical","health"],"status":"active","founded":2005,"parent_org":"ATIH / Assurance Maladie (French Ministry of Health)","tags":["icm/uses"]}}
---


# CCAM — Classification Commune des Actes Médicaux

## Overview
CCAM is the French national classification of medical procedures, used for
billing all medical and surgical acts in French hospitals and outpatient settings.
It replaced the older NGAP classification and is maintained by the **ATIH**
(Agence Technique de l'Information sur l'Hospitalisation) together with the
Assurance Maladie. Every procedure performed at [[04_Governance/AP-HP\|AP-HP]] — including brain MRI,
EEG, lumbar puncture, neurosurgery — is coded in CCAM, making it a key
terminology for any study using French hospital procedure data from the
[[04_Governance/Health Data Hub\|Health Data Hub]] SNDS or the AP-HP data warehouse.

## Key Neurological Procedure Codes
| CCAM Code | Procedure |
|---|---|
| ADQP001 | Brain MRI (IRM cérébrale) |
| ACQP001 | Brain CT scan (Scanner cérébral) |
| ADQJ001 | EEG recording |
| ADLB001 | Lumbar puncture (ponction lombaire) |
| ADFA001 | Intracranial electroencephalography (stereo-EEG) |
| ADNB001 | Deep brain stimulation implantation |
| ADQP003 | Functional brain MRI |
| EALB001 | Nerve conduction study |

## French Health Data Context
- **PMSI** (Programme de Médicalisation des Systèmes d'Information) — all
  hospital billing uses CCAM codes alongside [[02_Standards/ICD-10\|ICD-10]] diagnoses
- **SNDS** at [[04_Governance/Health Data Hub\|Health Data Hub]] — CCAM codes are present in the DCIR
  (Données de Consommation Inter-Régimes) outpatient billing data
- **AP-HP EDS** — procedure data in the clinical data warehouse maps
  to CCAM codes

## Relationship to Other Standards
- **[[02_Standards/SNOMED CT\|SNOMED CT]]** — SNOMED provides more granular semantic procedure
  descriptions; CCAM is French billing classification
- **[[02_Standards/ICD-10\|ICD-10]]** — used alongside CCAM; diagnoses (ICD-10) + procedures (CCAM)
  together describe a hospital stay
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — CCAM maps to OMOP procedure concepts (via Athena vocabulary)
- **[[02_Standards/LOINC\|LOINC]]** — LOINC codes lab tests; CCAM codes the clinical procedure

## Connections
- Used in: [[04_Governance/Health Data Hub\|Health Data Hub]] (SNDS/DCIR), [[04_Governance/AP-HP\|AP-HP]] (PMSI billing)
- Maps to: [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/OMOP CDM\|OMOP CDM]] (via Athena CCAM vocabulary)
- Complements: [[02_Standards/ICD-10\|ICD-10]] (diagnoses), [[02_Standards/LOINC\|LOINC]] (lab results)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (any study using AP-HP procedure data)

## Resources
- https://www.atih.sante.fr/les-nomenclatures-de-facturation/ccam
- https://www.ameli.fr/accueil-de-la-ccam/index.php (Ameli CCAM browser)
- https://athena.ohdsi.org (OMOP CCAM vocabulary)
