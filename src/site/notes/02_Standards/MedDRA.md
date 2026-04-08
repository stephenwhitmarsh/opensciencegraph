---
{"dg-publish":true,"permalink":"/02-standards/med-dra/","tags":["icm/uses"],"dg-note-properties":{"name":"Medical Dictionary for Regulatory Activities","aliases":["MedDRA"],"website":"https://www.meddra.org","type":"terminology","scope":"international","domain":["clinical"],"status":"active","founded":1994,"parent_org":"International Council for Harmonisation of Technical Requirements (ICH)","tags":["icm/uses"]}}
---


# MedDRA — Medical Dictionary for Regulatory Activities

## Overview
MedDRA is the international medical terminology developed under the auspices of
the International Council for Harmonisation of Technical Requirements for
Pharmaceuticals for Human Use (ICH). It is the required standard for adverse
event coding in clinical trial regulatory submissions to the EMA, FDA, and
national agencies including the French **ANSM** (Agence Nationale de Sécurité
du Médicament). Any clinical trial conducted at [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]
or through [[04_Governance/AP-HP\|AP-HP]] that submits to the EU Clinical Trials Regulation (CTR)
requires MedDRA coding for adverse events.

## Structure
MedDRA uses a five-level hierarchy:
1. **SOC** (System Organ Class) — top level, e.g. *Nervous system disorders*
2. **HLGT** (High Level Group Term)
3. **HLT** (High Level Term)
4. **PT** (Preferred Term) — the primary coding level for adverse events
5. **LLT** (Lowest Level Term) — most granular, maps to verbatim terms

## Neuroscience Relevance
The **Nervous System Disorders** SOC contains terms for:
- Dementia and cognitive impairment (AEs in Alzheimer's trials)
- Movement disorders (Parkinson's trials, dyskinesia as AE)
- Seizures and epilepsy events
- Headache, nausea (common neurological trial AEs)
- Peripheral neuropathy (chemotherapy-related)

## Connections
- Required by: [[04_Governance/ECRIN\|ECRIN]] (multinational EU clinical trials), [[04_Governance/AP-HP\|AP-HP]] (ANSM submissions)
- Complements: [[02_Standards/CDISC\|CDISC]] (SDTM format for AE data uses MedDRA coding)
- Related: [[02_Standards/ICD-10\|ICD-10]] (diagnostic coding vs AE coding — different purposes)
- Implemented in: [[02_Standards/OMOP CDM\|OMOP CDM]] (MedDRA vocabulary available in Athena)
- Relevant to: [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] (all clinical trials under EU CTR)

## Resources
- https://www.meddra.org
- https://www.meddra.org/how-to-use/support-documentation/english (guides)
- https://www.ema.europa.eu/en/human-regulatory/research-development/data-medicines-iso-idmp-standards/eudravigilance/meddra (EMA MedDRA page)
