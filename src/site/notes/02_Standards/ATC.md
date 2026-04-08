---
{"dg-publish":true,"permalink":"/02-standards/atc/","dg-note-properties":{"name":"ATC","aliases":["Anatomical Therapeutic Chemical Classification","ATC/DDD","Defined Daily Dose"],"website":"https://www.who.int/tools/atc-ddd-toolkit/atc-classification","type":"terminology","scope":"international","domain":["clinical","health"],"status":"active","founded":1976,"parent_org":"WHO Collaborating Centre for Drug Statistics Methodology (Norwegian Institute of Public Health)"}}
---


# ATC

## Overview
The Anatomical Therapeutic Chemical (ATC) Classification System is the WHO-endorsed
international standard for classifying drug substances by the organ or system they
act on, and by their therapeutic, pharmacological, and chemical properties. Developed
in Norway in the 1970s, it was formalised by the WHO Collaborating Centre for Drug
Statistics Methodology (established 1982, hosted at the Norwegian Institute of Public
Health in Oslo) and recommended for global use by WHO in 1996. ATC is paired with
the Defined Daily Dose (DDD) — a unit of measurement representing the assumed average
adult maintenance dose per day — to form the ATC/DDD methodology, the international
standard for drug utilisation research and pharmacoepidemiology.

## Structure
ATC codes have a five-level hierarchy:

| Level | Type | Example |
|---|---|---|
| 1st | Anatomical main group (letter) | `N` — Nervous System |
| 2nd | Therapeutic subgroup (2 digits) | `N05` — Psycholeptics |
| 3rd | Therapeutic/pharmacological subgroup (letter) | `N05A` — Antipsychotics |
| 4th | Chemical/pharmacological subgroup (letter) | `N05AH` — Diazepines, oxazepines… |
| 5th | Chemical substance (2 digits) | `N05AH03` — Olanzapine |

There are 14 anatomical main groups (A–V). The index is updated annually each
January 1st. A substance can have multiple ATC codes for different routes of
administration or indications.

## ATC and DDD in OMOP CDM
ATC is a standardised vocabulary in the [[02_Standards/OMOP CDM\|OMOP CDM]] Athena vocabulary browser, where
it supplements [[02_Standards/RxNorm\|RxNorm]] as a drug classification hierarchy. ATC codes are used for:
- Drug utilisation studies and pharmacoepidemiology
- Imputing drug exposure duration (via DDD-based calculations)
- Mapping across different national drug coding systems
- SNDS and AP-HP EDS drug coding (France uses ATC for population-level pharmacovigilance)

## Connections
- Maintained by: WHO Collaborating Centre for Drug Statistics Methodology (WHOCC, Oslo)
- Used in: [[02_Standards/OMOP CDM\|OMOP CDM]] (Athena vocabulary), [[03_Platforms/SNDS\|SNDS]] (French national health data),
  [[04_Governance/Health Data Hub\|Health Data Hub]], [[04_Governance/AP-HP\|AP-HP]] EDS, [[02_Standards/OSIRIS\|OSIRIS]] (oncology drug coding)
- Complementary terminologies: [[02_Standards/RxNorm\|RxNorm]] (US clinical drug names), [[02_Standards/ChEBI\|ChEBI]]
  (chemical entities), [[02_Standards/MedDRA\|MedDRA]] (adverse events)
- Relevant to [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]: drug coding in SNDS-based pharmacoepidemiology
  studies; required for OMOP CDM drug_exposure table analysis; used in neurological
  drug utilisation research (antiepileptics, antiparkinson agents — ATC N03/N04)

## Resources
- ATC classification: https://www.who.int/tools/atc-ddd-toolkit/atc-classification
- ATC/DDD index (searchable): https://atcddd.fhi.no/atc_ddd_index/
- ATC/DDD methodology: https://www.who.int/tools/atc-ddd-toolkit/methodology
- Athena OMOP vocabularies: https://athena.ohdsi.org
