---
{"dg-publish":true,"permalink":"/02-standards/ch-ebi/","dg-note-properties":{"name":"Chemical Entities of Biological Interest","aliases":["ChEBI"],"website":"https://www.ebi.ac.uk/chebi/","type":"terminology","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2004,"parent_org":"EMBL-EBI"}}
---


# ChEBI — Chemical Entities of Biological Interest

## Overview
ChEBI (Chemical Entities of Biological Interest) is a freely available dictionary
of molecular entities focused on small chemical compounds relevant to biology.
Developed and maintained by EMBL-EBI, ChEBI provides a structured, machine-readable
classification of chemical entities including metabolites, drugs, natural products,
and environmental chemicals — with precise chemical structure, role, and relationship
information. It is an OBO Foundry ontology and a core reference vocabulary for
pharmacological, metabolomic, and biochemical research.

For [[00_Core/Paris Brain Institute\|Paris Brain Institute]], ChEBI is relevant to pharmacological research
(drug mechanisms, neurotransmitter chemistry), metabolomics studies, and the
semantic annotation of chemical compounds in [[02_Standards/OMOP CDM\|OMOP CDM]] drug records and
clinical trial data.

## Key Concept Areas
- **Drugs and pharmacological agents** — CNS drugs, anaesthetics, contrast agents,
  radiopharmaceuticals (PET tracers), therapeutic antibodies
- **Neurotransmitters and neuromodulators** — dopamine, serotonin, GABA,
  glutamate, acetylcholine, noradrenaline
- **Metabolites** — amino acids, lipids, nucleotides, cofactors
- **Natural products** — plant-derived compounds, toxins
- **Environmental chemicals** — pollutants relevant to neurological disease risk

## Role in Clinical and Research Data Standards
ChEBI serves as the chemical entity reference in several interconnected standards:
- **[[02_Standards/OMOP CDM\|OMOP CDM]]** — ChEBI identifiers used in drug and ingredient concept mapping
  alongside RxNorm; ChEBI covers the chemical layer while [[02_Standards/RxNorm\|RxNorm]] covers
  the clinical drug formulation layer
- **[[02_Standards/HL7 FHIR\|HL7 FHIR]]** — ChEBI codes used in medication resources for precise
  chemical identification
- **[[02_Standards/Phenopackets\|Phenopackets]]** — ChEBI used to describe disease-relevant chemical
  exposures and drug treatments in phenotypic data packages
- **Metabolomics** — standard reference in metabolomics databases
  (MetaboLights, HMDB) for compound identification

## Connections
- Produced by: EMBL-EBI
- Part of: OBO Foundry (https://obofoundry.org)
- Complements: [[02_Standards/RxNorm\|RxNorm]] (clinical drug formulations), [[02_Standards/LOINC\|LOINC]] (lab tests),
  [[02_Standards/OMOP CDM\|OMOP CDM]] (drug concepts), [[02_Standards/GO\|GO]] (molecular function of chemical agents)
- Used in: metabolomics, pharmacology, clinical data standardisation
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (pharmacological research, OMOP CDM
  drug mapping, PET radiotracer annotation)

## Resources
- https://www.ebi.ac.uk/chebi/
- https://obofoundry.org/ontology/chebi.html (OBO Foundry entry)
- https://www.ebi.ac.uk/ols/ontologies/chebi (EBI OLS browser)
