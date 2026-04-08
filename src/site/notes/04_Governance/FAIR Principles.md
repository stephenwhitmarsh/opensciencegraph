---
{"dg-publish":true,"permalink":"/04-governance/fair-principles/","dg-note-properties":{"name":"FAIR Principles","aliases":["FAIR","Findable Accessible Interoperable Reusable"],"website":"https://www.go-fair.org/fair-principles/","type":"framework","scope":"international","domain":["multimodal"],"status":"active","founded":2016,"icon":"https://www.go-fair.org/wp-content/uploads/2019/01/GO_FAIR_favicon.png"}}
---


# FAIR Principles

## Overview
The FAIR Principles are 15 guiding principles for scientific data management and stewardship, published in 2016 by Wilkinson et al. in *Nature Scientific Data* (DOI:10.1038/sdata.2016.18). FAIR stands for **Findable, Accessible, Interoperable, Reusable**. They are not a standard or a certification — they are a set of aspirational properties that data and metadata should have to maximise their value for both humans and machines. They are now mandated by most major funders worldwide including the EU (Horizon Europe, [[04_Governance/EOSC\|EOSC]], [[04_Governance/EHDS\|EHDS]]) and
France ([[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[04_Governance/Ouvrir la Science\|Ouvrir la Science]]).

## The 15 Principles

### Findable
- **F1** — Data and metadata are assigned a globally unique and persistent identifier
- **F2** — Data are described with rich metadata
- **F3** — Metadata clearly and explicitly include the identifier of the data they describe
- **F4** — Data and metadata are registered or indexed in a searchable resource

### Accessible
- **A1** — Data and metadata are retrievable by their identifier using a standardised
  communications protocol; the protocol is open, free, and universally implementable
- **A1.1** — The protocol allows for an authentication and authorisation procedure
  where necessary
- **A1.2** — The protocol allows for access to metadata even when data are no longer available
- **A2** — Metadata are accessible even when the data are no longer available

### Interoperable
- **I1** — Data and metadata use a formal, accessible, shared, and broadly applicable
  language for knowledge representation
- **I2** — Data and metadata use vocabularies that follow FAIR principles
- **I3** — Data and metadata include qualified references to other data and metadata

### Reusable
- **R1** — Data and metadata are richly described with a plurality of accurate and
  relevant attributes
- **R1.1** — Data and metadata are released with a clear and accessible data usage licence
- **R1.2** — Data and metadata are associated with detailed provenance
- **R1.3** — Data and metadata meet domain-relevant community standards

## Key Distinction: Principles vs Implementation
FAIR principles are **aspirational** — they describe what data *should* be, not
how to achieve it. The actual implementation happens through specific standards
and infrastructures. This distinction matters for the vault:

| Domain | What implements FAIR in practice |
|---|---|
| Neuroimaging | [[02_Standards/BIDS\|BIDS]], [[02_Standards/NIfTI\|NIfTI]], [[03_Platforms/OpenNeuro\|OpenNeuro]], [[03_Platforms/EBRAINS\|EBRAINS]] |
| Neurophysiology | [[02_Standards/NWB\|NWB]], [[03_Platforms/DANDI Archive\|DANDI Archive]] |
| Microscopy | [[02_Standards/OME File Formats\|OME File Formats]], [[03_Platforms/OMERO\|OMERO]] via [[01_Actors/OME\|OME]], [[02_Standards/REMBI\|REMBI]] metadata |
| Genomics | [[02_Standards/VCF\|VCF]], [[01_Actors/GA4GH\|GA4GH]], [[02_Standards/Phenopackets\|Phenopackets]] |
| Clinical / EHR | [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[04_Governance/Health Data Hub\|Health Data Hub]] |
| Clinical coding | [[02_Standards/SNOMED CT\|SNOMED CT]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/CCAM\|CCAM]], [[02_Standards/MedDRA\|MedDRA]] |
| Disease ontology | [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]], [[02_Standards/HPO\|HPO]] |
| Brain annotation | [[02_Standards/UBERON\|UBERON]], [[02_Standards/openMINDS\|openMINDS]], [[02_Standards/Cognitive Atlas\|Cognitive Atlas]], [[02_Standards/HED\|HED]] |
| Provenance | [[02_Standards/PROV-O\|PROV-O]], [[02_Standards/NIDM\|NIDM]] |
| Data catalogues | [[02_Standards/DCAT\|DCAT]], [[02_Standards/Dublin Core\|Dublin Core]] |
| French research data | [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[04_Governance/OPIDoR\|OPIDoR]] |
| European infrastructure | [[04_Governance/EOSC\|EOSC]], [[04_Governance/ELIXIR\|ELIXIR]], [[04_Governance/OpenAIRE\|OpenAIRE]] |

## Created By
- [[04_Governance/FORCE11\|FORCE11]] — co-authored the original 2016 Wilkinson et al. paper
- [[04_Governance/GO FAIR\|GO FAIR]] — developed the Three-Point FAIRification Framework
- [[04_Governance/RDA\|RDA]] — produced the FAIR Data Maturity Model (RDA WG output, 2020)

## Actively Promoted / Measured By
These bodies have FAIR as a core operational mandate — not just alignment:
- [[04_Governance/GO FAIR\|GO FAIR]] — FAIRification framework and Implementation Networks
- [[04_Governance/RDA\|RDA]] — FAIR Data Maturity Model, working group outputs
- [[04_Governance/EOSC\|EOSC]] — mandates FAIR for all EU-funded research data
- [[01_Actors/INCF\|INCF]] — FAIR neuroscience as explicit mission; FAIR-Checker tool
- [[04_Governance/ELIXIR\|ELIXIR]] — FAIR data services across European life science nodes
- [[04_Governance/IFB\|IFB]] — FAIR-Checker tool; FAIR compliance support for French researchers
- [[04_Governance/Health Data Hub\|Health Data Hub]] — FAIR data access infrastructure for French health data
- [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]] — mandates FAIR deposit for all funded projects
- [[04_Governance/OPIDoR\|OPIDoR]] — DMP tooling implementing FAIR requirements

## Resources
- https://www.go-fair.org/fair-principles/
- Wilkinson et al. (2016) *Nature Scientific Data* DOI:10.1038/sdata.2016.18
- https://www.rd-alliance.org/group/fair-data-maturity-model-wg (RDA Maturity Model)
- https://www.nature.com/articles/s41597-022-01710-x (FAIR assessment review, 2022)
