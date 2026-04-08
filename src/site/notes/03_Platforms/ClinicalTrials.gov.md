---
{"dg-publish":true,"permalink":"/03-platforms/clinical-trials-gov/","tags":["icm/uses"],"dg-note-properties":{"name":"ClinicalTrials.gov","aliases":["CTG"],"website":"https://clinicaltrials.gov","type":"repository","scope":"international","domain":["clinical"],"status":"active","founded":2000,"parent_org":"National Library of Medicine (NLM) / NIH","tags":["icm/uses"]}}
---


# ClinicalTrials.gov

## Overview
ClinicalTrials.gov is the world's largest registry and results database for
clinical trials, operated by the US National Library of Medicine (NLM) / NIH
since 2000. It provides public access to information on privately and publicly
funded clinical studies conducted around the world. Registration is mandated
by the FDA Amendments Act (FDAAA 2007) for US-regulated trials, and is required
by the International Committee of Medical Journal Editors (ICMJE) as a condition
of publication in most major medical journals worldwide.

For [[01_Actors/Paris Brain Institute\|Paris Brain Institute]], ClinicalTrials.gov registration is mandatory for
all interventional clinical trials involving ICM researchers or [[04_Governance/AP-HP\|AP-HP]] as
sponsor, and is the primary registry for trials conducted through [[04_Governance/NeurATRIS\|NeurATRIS]]
and [[01_Actors/Institut de Myologie\|Institut de Myologie]] clinical platforms.

## What ClinicalTrials.gov Provides

### Registry
- Study design, eligibility criteria, interventions, primary and secondary endpoints
- Sponsor and investigator contact information
- Recruitment status and study locations (including French sites)
- Protocol documents (optional upload)
- NCT number — the universal trial identifier used in publications

### Results Database
Since 2017, FDAAA requires results submission within 12 months of primary
completion for applicable clinical trials:
- Participant flow and baseline characteristics
- Outcome measure results with statistical analyses
- Adverse events
- Point-of-care result summaries

## European Context
ClinicalTrials.gov is complementary to the **EU Clinical Trials Register** (EU CTR,
https://www.clinicaltrialsregister.eu) which covers Eudra-CT registered trials.
Under EU Clinical Trials Regulation (EU 536/2014), the **CTIS** (Clinical Trials
Information System) is replacing EudraCT for EU trials from 2023. Both registries
are accepted by ICMJE. French trials are typically registered in both
ClinicalTrials.gov and EudraCT/CTIS.

## Data Standards
ClinicalTrials.gov data is accessible via a structured API and uses controlled
vocabularies for:
- Conditions: [[02_Standards/MeSH\|MeSH]] terms (Medical Subject Headings), [[02_Standards/ICD-10\|ICD-10]]
- Interventions: drug names mapped to [[02_Standards/RxNorm\|RxNorm]] and [[02_Standards/ChEBI\|ChEBI]]
- Outcomes: outcome measure terms aligned with [[02_Standards/LOINC\|LOINC]] and [[02_Standards/CDISC\|CDISC]]

## Connections
- Operated by: NLM / NIH
- Complements: EU CTR / CTIS (European registry), WHO ICTRP (global registry)
- Standards: [[02_Standards/CDISC\|CDISC]] (trial data structure), [[02_Standards/MedDRA\|MedDRA]] (adverse events),
  [[02_Standards/ICD-10\|ICD-10]] (condition coding), [[02_Standards/RxNorm\|RxNorm]] / [[02_Standards/ChEBI\|ChEBI]] (drug coding)
- French trials: registered here + EudraCT/CTIS; sponsored by [[04_Governance/AP-HP\|AP-HP]],
  [[04_Governance/ECRIN\|ECRIN]] for multinational trials
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (trial registration requirement;
  [[04_Governance/NeurATRIS\|NeurATRIS]] and [[01_Actors/Institut de Myologie\|Institut de Myologie]] clinical programmes)

## Resources
- https://clinicaltrials.gov
- https://clinicaltrials.gov/data-api/api (REST API)
- https://www.clinicaltrialsregister.eu (EU CTR — European registry)
