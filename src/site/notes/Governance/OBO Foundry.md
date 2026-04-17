---
{"dg-publish":true,"permalink":"/governance/obo-foundry/","dg-note-properties":{"name":"Open Biological and Biomedical Ontology Foundry","aliases":["OBO Foundry","OBO"],"website":"https://obofoundry.org","type":"consortium","scope":"international","domain":["genomics","clinical","multimodal"],"status":"active","founded":2001,"parent_org":"OBO Foundry Operations Committee"}}
---


# OBO Foundry — Open Biological and Biomedical Ontology Foundry

## Overview
The OBO Foundry is an international consortium of ontology developers committed to developing a suite of interoperable, open biomedical ontologies. Founded in 2001 and formalised in 2007 with the publication of the OBO Foundry principles (*Nature Biotechnology*, Ashburner et al.), it provides the governance framework and quality standards for a coordinated family of ontologies that form the semantic backbone of modern biomedical data integration. For this vault, OBO Foundry is the parent consortium for many of the terminology nodes that appear as standards used across the ICM ecosystem.

OBO Foundry occupies the same role for biomedical ontologies that [[Actors/INCF\|INCF]] occupies for neuroscience data standards and [[Actors/GA4GH\|GA4GH]] occupies for genomics standards: it is the governing body that sets principles, reviews candidate ontologies, and coordinates interoperability across member ontologies.

## Foundry Principles
OBO ontologies must adhere to a set of shared principles ensuring quality and interoperability:
- **Open** — freely available under CC BY 3.0 or equivalent
- **Common format** — OWL2 and/or OBO flat file format
- **Unique identifiers** — globally unique, stable term IDs (e.g. `HP:0001250`, `GO:0007268`)
- **Versioned** — dated releases with stable identifiers across versions
- **Scope** — each ontology has a defined, non-overlapping domain
- **Textual definitions** — all terms have human-readable definitions
- **Interoperability** — ontologies reuse terms from other OBO Foundry members rather than duplicating them (e.g. UBERON anatomy terms are reused in HPO, GO, and MONDO)

## Key OBO Foundry Ontologies in This Vault
The following OBO Foundry member ontologies have dedicated nodes:

| Ontology | Node | Domain |
|---|---|---|
| GO | [[Standards/GO\|GO]] | Gene function (biological process, molecular function, cellular component) |
| HPO | [[Standards/HPO\|HPO]] | Human phenotypes for rare disease genomics |
| UBERON | [[Standards/UBERON\|UBERON]] | Cross-species anatomy |
| MONDO | [[Standards/MONDO\|MONDO]] | Unified disease ontology (harmonises ICD, OMIM, ORDO) |
| ORDO | [[Standards/ORDO\|ORDO]] | Orphanet rare disease classification |
| OBI | [[Standards/OBI\|OBI]] | Biomedical investigation protocols and assays |
| Cell Ontology | [[Standards/Cell Ontology\|Cell Ontology]] | Cell type classification |
| ChEBI | [[Standards/ChEBI\|ChEBI]] | Chemical entities of biological interest |
| MeSH | [[Standards/MeSH\|MeSH]] | Medical subject headings (NLM; OBO aligned) |

## Tools and Infrastructure
- **OntoBee** — OBO ontology browser (https://www.ontobee.org)
- **EBI OLS** (Ontology Lookup Service) — EMBL-EBI ontology browser supporting all OBO Foundry members (https://www.ebi.ac.uk/ols)
- **BioPortal** — NCBO ontology portal hosting OBO and non-OBO ontologies (https://bioportal.bioontology.org)
- **Protégé** — primary ontology editing tool used by OBO Foundry curators (https://protege.stanford.edu)
- **ROBOT** — command-line tool for OBO ontology manipulation and quality control (https://robot.obolibrary.org)

## Connections
- Member ontologies: [[Standards/GO\|GO]], [[Standards/HPO\|HPO]], [[Standards/UBERON\|UBERON]], [[Standards/MONDO\|MONDO]], [[Standards/ORDO\|ORDO]], [[Standards/OBI\|OBI]], [[Standards/Cell Ontology\|Cell Ontology]], [[Standards/ChEBI\|ChEBI]]
- Complements: [[Actors/GA4GH\|GA4GH]] (genomics data standards), [[Actors/INCF\|INCF]] (neuroscience data standards), [[Standards/HL7 FHIR\|HL7 FHIR]] (clinical interoperability)
- Adopted by: [[Standards/OMOP CDM\|OMOP CDM]] (Athena vocabulary includes OBO terms), [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/ELIXIR\|ELIXIR]], [[Platforms/EBRAINS\|EBRAINS]]
- Reference publication: Ashburner et al. (2001) *Gene Ontology*; Smith et al. (2007) *Nature Biotechnology* doi:10.1038/nbt1346

## Resources
- https://obofoundry.org (OBO Foundry portal — full ontology list)
- https://www.ebi.ac.uk/ols (EBI Ontology Lookup Service)
- https://obofoundry.org/principles/fp-000-summary.html (OBO Foundry Principles)
- https://github.com/OBOFoundry (GitHub organisation)
