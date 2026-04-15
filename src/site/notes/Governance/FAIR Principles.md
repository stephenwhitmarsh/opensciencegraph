---
{"dg-publish":true,"permalink":"/governance/fair-principles/","dg-note-properties":{"name":"FAIR Principles","aliases":["FAIR","Findable Accessible Interoperable Reusable"],"website":"https://www.go-fair.org/fair-principles/","type":"framework","scope":"international","domain":["multimodal"],"status":"active","founded":2016,"icon":"https://www.go-fair.org/wp-content/uploads/2019/01/GO_FAIR_favicon.png"}}
---


# FAIR Principles

## Overview
The FAIR Principles are 15 guiding principles for scientific data management and stewardship, published in 2016 by Wilkinson et al. in *Nature Scientific Data* (DOI:10.1038/sdata.2016.18). FAIR stands for **Findable, Accessible, Interoperable, Reusable**. They are not a standard or a certification — they are a set of aspirational properties that data and metadata should have to maximise their value for both humans and machines. They are now mandated by most major funders worldwide including the EU (Horizon Europe, [[Governance/EOSC\|EOSC]], [[Governance/EHDS\|EHDS]]) and
France ([[Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[Governance/Ouvrir la Science\|Ouvrir la Science]]).

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
| Neuroimaging | [[Standards/BIDS\|BIDS]], [[Standards/NIfTI\|NIfTI]], [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/EBRAINS\|EBRAINS]] |
| Neurophysiology | [[Standards/NWB\|NWB]], [[Platforms/DANDI Archive\|DANDI Archive]] |
| Microscopy | [[Standards/OME File Formats\|OME File Formats]], [[Platforms/OMERO\|OMERO]] via [[Actors/OME\|OME]], [[Standards/REMBI\|REMBI]] metadata |
| Genomics | [[Standards/VCF\|VCF]], [[Actors/GA4GH\|GA4GH]], [[Standards/Phenopackets\|Phenopackets]] |
| Clinical / EHR | [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]], [[Governance/Health Data Hub\|Health Data Hub]] |
| Clinical coding | [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/LOINC\|LOINC]], [[Standards/ICD-10\|ICD-10]], [[Standards/CCAM\|CCAM]], [[Standards/MedDRA\|MedDRA]] |
| Disease ontology | [[Standards/MONDO\|MONDO]], [[Standards/ORDO\|ORDO]], [[Standards/HPO\|HPO]] |
| Brain annotation | [[Standards/UBERON\|UBERON]], [[Standards/openMINDS\|openMINDS]], [[Standards/Cognitive Atlas\|Cognitive Atlas]], [[Standards/HED\|HED]] |
| Provenance | [[Standards/PROV-O\|PROV-O]], [[Standards/NIDM\|NIDM]] |
| Data catalogues | [[Standards/DCAT\|DCAT]], [[Standards/Dublin Core\|Dublin Core]] |
| French research data | [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]], [[Governance/OPIDoR\|OPIDoR]] |
| European infrastructure | [[Governance/EOSC\|EOSC]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/OpenAIRE\|OpenAIRE]] |

## Created By
- [[FORCE11\|FORCE11]] — co-authored the original 2016 Wilkinson et al. paper
- [[Governance/GO FAIR\|GO FAIR]] — developed the Three-Point FAIRification Framework
- [[Governance/RDA\|RDA]] — produced the FAIR Data Maturity Model (RDA WG output, 2020)

## Actively Promoted / Measured By
These bodies have FAIR as a core operational mandate — not just alignment:
- [[Governance/GO FAIR\|GO FAIR]] — FAIRification framework and Implementation Networks
- [[Governance/RDA\|RDA]] — FAIR Data Maturity Model, working group outputs
- [[Governance/EOSC\|EOSC]] — mandates FAIR for all EU-funded research data
- [[Actors/INCF\|INCF]] — FAIR neuroscience as explicit mission; FAIR-Checker tool
- [[Governance/ELIXIR\|ELIXIR]] — FAIR data services across European life science nodes
- [[Governance/IFB\|IFB]] — FAIR-Checker tool; FAIR compliance support for French researchers
- [[Governance/Health Data Hub\|Health Data Hub]] — FAIR data access infrastructure for French health data
- [[Governance/ANR Open Science Policy\|ANR Open Science Policy]] — mandates FAIR deposit for all funded projects
- [[Governance/OPIDoR\|OPIDoR]] — DMP tooling implementing FAIR requirements

## Resources
- https://www.go-fair.org/fair-principles/
- Wilkinson et al. (2016) *Nature Scientific Data* DOI:10.1038/sdata.2016.18
- https://www.rd-alliance.org/group/fair-data-maturity-model-wg (RDA Maturity Model)
- https://www.nature.com/articles/s41597-022-01710-x (FAIR assessment review, 2022)
