---
{"dg-publish":true,"permalink":"/03-platforms/brain-code/","dg-note-properties":{"name":"Brain-CODE","aliases":["BrainCODE","Ontario Brain Institute Brain-CODE"],"website":"https://www.braincode.ca","type":"platform","scope":"international","domain":["neuroimaging","clinical","genomics","multimodal"],"status":"active","founded":2012,"parent_org":"Ontario Brain Institute"}}
---


# Brain-CODE

## Overview
Brain-CODE is the large-scale neuroinformatics platform of the **[[01_Actors/OBI\|OBI]]** (Ontario
Brain Institute), developed since 2012 for the collection, curation, federation,
sharing, and analysis of multimodal neuroscience data across brain disorders.
It serves 240+ researchers at 40+ institutions across Canada, storing data from
OBI's five Integrated Discovery Programs (IDPs) alongside data from other
research teams.

Brain-CODE is one of the three primary data platforms integrated into the
**[[01_Actors/CONP\|CONP]]** (Canadian Open Neuroscience Platform) portal — alongside [[03_Platforms/LORIS\|LORIS]]
and [[03_Platforms/XNAT\|XNAT]] — and has been a pioneer of **[[04_Governance/FAIR Principles\|FAIR Principles]]** implementation
in clinical neuroscience since its inception.

## Platform Architecture
Brain-CODE is built around five core components:

1. **Data capture** — standardised web forms using Common Data Elements (CDEs)
   across OBI's IDP studies; supports clinical, neuroimaging, genetic, and
   behavioural data
2. **Data storage** — secure, encrypted storage on Canadian-hosted infrastructure;
   Privacy-by-Design; participant data de-identified
3. **Data integration** — cross-disorder harmonisation through shared CDEs;
   supports queries across data modalities and brain disorders
4. **Analytics** — web-based high-performance computing environment; advanced
   software and tools for data management, curation, and analytics
5. **Federation** — bidirectional links to external databases:
   - [[03_Platforms/LORIS\|LORIS]] at McGill University (federated neuroimaging data exchange)
   - [[03_Platforms/XNAT\|XNAT]] (imaging data integration)
   - [[01_Actors/CONP\|CONP]] portal (all data releases registered and discoverable)
   - ICES (Institute for Clinical Evaluative Sciences) health administrative data
     via Privacy-Preserving Record Linkage (PPRL)

## FAIR Implementation
Brain-CODE was one of the earliest platforms to operationalise [[04_Governance/FAIR Principles\|FAIR Principles]]
in clinical neuroscience (since 2012), documented in a 2023 paper in
*Frontiers in Neuroinformatics*:

- **Findable** — all data releases registered on [[01_Actors/CONP\|CONP]] portal with DATS metadata;
  DOIs assigned; standardised metadata schemas
- **Accessible** — web-based portal (https://www.braincode.ca); controlled access
  model with Data Access Committee review; standardised consent language for
  de-identified data reuse
- **Interoperable** — Common Data Elements; [[03_Platforms/LORIS\|LORIS]] and [[03_Platforms/XNAT\|XNAT]] federation;
  DATS metadata model compatible with CONP portal indexing
- **Reusable** — standardised consent for secondary research use; data governance
  policy published; data releases include documentation

## Data Releases and Open Datasets
Brain-CODE hosts 10+ datasets on the [[01_Actors/CONP\|CONP]] portal, including:
- **ONDRI** (Ontario Neurodegenerative Disease Research Initiative) — multimodal
  longitudinal data on Alzheimer's, Parkinson's, ALS, vascular and FTD
- **CHILD-BRIGHT** — cerebral palsy; brain-based childhood disability
- **POND** — neurodevelopmental disorders (autism, ADHD, OCD, fragile X)
- Depression and concussion programme datasets

Datasets are described using a customised DATS (Data Tags Suite) metadata model
and are accessible via DataLad through the CONP portal.

## Privacy and Governance
- Privacy-by-Design architecture
- **PPRL** (Privacy-Preserving Record Linkage) using El Gamal homomorphic encryption
  for linking with health administrative data
- Data Access Committee governs external data requests
- Informatics Steering Committee oversees platform direction
- Brain-CODE Governance Policy publicly available

## Connections
- Operated by: [[01_Actors/OBI\|OBI]] (Ontario Brain Institute)
- Canadian federation: [[01_Actors/CONP\|CONP]] (all data releases registered; OBI/Rotman is CONP sponsor)
- Platform interoperability: [[03_Platforms/LORIS\|LORIS]] (McGill; federated neuroimaging exchange),
  [[03_Platforms/XNAT\|XNAT]] (imaging integration), [[03_Platforms/OSF\|OSF]], [[03_Platforms/Zenodo\|Zenodo]] (CONP data sources)
- International: [[03_Platforms/EBRAINS\|EBRAINS]], [[03_Platforms/OpenNeuro\|OpenNeuro]] (CONP developing interoperability)
- Standards: [[04_Governance/FAIR Principles\|FAIR Principles]], [[02_Standards/BIDS\|BIDS]] (neuroimaging), DATS metadata model
- Related platforms: [[03_Platforms/Synapse AMP-AD\|Synapse AMP-AD]] (comparable open neuroscience data platform),
  [[03_Platforms/NCBI GEO\|NCBI GEO]] (open genomics complement)

## Resources
- https://www.braincode.ca (Brain-CODE portal)
- https://braininstitute.ca/research-data-sharing/brain-code (OBI overview)
- https://doi.org/10.3389/fninf.2023.1158378 (FAIR in action: Brain-CODE, 2023)
- https://braininstitute.ca/docs/Brain-CODE-Governance-Policy-version-FINAL.pdf
