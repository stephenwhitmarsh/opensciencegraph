---
{"dg-publish":true,"permalink":"/03-platforms/vivli/","dg-note-properties":{"name":"VIVLI","aliases":["Center for Global Clinical Research Data"],"website":"https://vivli.org","type":"platform","scope":"international","domain":["clinical"],"status":"active","founded":2016}}
---


# VIVLI — Center for Global Clinical Research Data

## Overview
VIVLI is an independent non-profit platform (founded 2016, Boston) that enables responsible sharing and reuse of individual patient-level data (IPD) from clinical trials globally. It serves as a neutral, trusted intermediary repository between pharmaceutical companies, academic sponsors, and researchers seeking access to trial data for secondary analysis, meta-analysis, and replication studies.

VIVLI's model addresses the gap between two extremes: fully open publication of trial data (which risks privacy) and complete data lock-up (which wastes research value). Instead, VIVLI implements a **controlled-access model** where researchers submit proposals, and data contributors decide on a case-by-case basis whether to grant access through a standardised request and review process.

## How VIVLI Works

### For Data Contributors
Pharmaceutical companies, academic institutions, and foundations deposit anonymised individual patient datasets from completed trials. Contributors retain control: they set access conditions and review requests. Major contributors include Johnson & Johnson, Novartis, Pfizer, Roche, GSK, Sanofi, and multiple academic research programmes.

### For Researchers
Researchers submit a research proposal describing the planned analysis. VIVLI reviews for completeness; contributors review for scientific validity. Approved researchers access data via a secure **Enclave** (cloud-based remote desktop) — data cannot be downloaded, only analysed in-place. Results and code can be exported after review.

## Data Standards
- **[[02_Standards/CDISC\|CDISC]]** — VIVLI encourages SDTM/ADaM-formatted submissions; provides metadata harmonisation support for non-CDISC datasets
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — VIVLI is exploring OMOP harmonisation for federated queries across deposited datasets
- Metadata uses controlled terminology ([[02_Standards/MeSH\|MeSH]] for conditions, [[02_Standards/RxNorm\|RxNorm]] for drugs)

## Neurological Disease Datasets
VIVLI hosts datasets relevant to neurological disease research including Alzheimer's disease trials (cholinesterase inhibitors, amyloid-targeting agents), Parkinson's disease trials, multiple sclerosis disease-modifying therapy trials, and ALS (amyotrophic lateral sclerosis) trials.

## Connections
- Standards: [[02_Standards/CDISC\|CDISC]] (SDTM/ADaM), [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/MeSH\|MeSH]], [[02_Standards/RxNorm\|RxNorm]]
- Related platforms: [[04_Governance/YODA Project\|YODA Project]] (Yale-based IPD sharing), [[04_Governance/TransCelerate\|TransCelerate]] (pharma industry data standardisation)
- Trial registry: [[03_Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]] (linked trial registration)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (access to neurological disease trial IPD for meta-analysis and replication)

## Resources
- https://vivli.org
- https://vivli.org/members/ourmembers/ (VIVLI data contributors)
- https://vivli.org/resources/requestingdata/ (access request process)
