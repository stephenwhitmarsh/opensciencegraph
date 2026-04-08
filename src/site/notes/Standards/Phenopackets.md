---
{"dg-publish":true,"permalink":"/standards/phenopackets/","dg-note-properties":{"name":"GA4GH Phenopacket Schema","aliases":["Phenopackets","GA4GH Phenopackets"],"website":"https://www.ga4gh.org/product/phenopackets/","type":"standard","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2019,"parent_org":"GA4GH"}}
---


# Phenopackets - GA4GH Phenopacket Schema

## Overview
The GA4GH Phenopacket Schema is a community standard for the computable exchange of clinical and phenotypic data linked to genomic information. It provides a human- and machine-readable structure that captures a patient's phenotypic features (using [[Standards/HPO\|HPO]] terms), diagnoses, biosample data, genomic variants (via [[Standards/VCF\|VCF]] / VRS), medical actions, and pedigree information in a single coherent package. Adopted as an ISO standard (ISO/TS 5435:2022), it is the key bridge between the clinical phenotype world and the genomics world, and is directly relevant to rare neurological disease work at [[Actors/Paris Brain Institute\|Paris Brain Institute]].

## Created / Governed By
- [[Actors/GA4GH\|GA4GH]] — Clinical & Phenotypic Data Capture Work Stream
- ISO approved as ISO/TS 5435:2022

## Key Features
- Links phenotypic descriptions (using [[Standards/HPO\|HPO]]) to genomic variant data ([[Standards/VCF\|VCF]]/VRS)
- Supports rare disease, complex disease, and cancer use cases
- Integrates pedigree data (family history) for Mendelian disease analysis
- Modular design: compatible with any ontology or terminology
- Interoperable with [[Standards/HL7 FHIR\|HL7 FHIR]] (FHIR implementation guide published)
- Interoperable with [[Standards/OMOP CDM\|OMOP CDM]] for EHR-linked cohorts

## Use Cases in Neuroscience
- Rare neurological disease diagnostics (e.g. rare epilepsies, rare dementias)
- Neurogenomics cohort phenotyping for GWAS and rare variant studies
- Patient stratification in precision neurology
- Data submission to [[Governance/BBMRI-ERIC\|BBMRI-ERIC]] biobank network and [[Governance/EHDS\|EHDS]] secondary use

## Connections
- Governed by: [[Actors/GA4GH\|GA4GH]]
- Ontology used: [[Standards/HPO\|HPO]] (Human Phenotype Ontology — primary phenotype vocabulary)
- Variant format: [[Standards/VCF\|VCF]], GA4GH VRS
- Interoperates with: [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/SNOMED CT\|SNOMED CT]]
- Adopted by: [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/EHDS\|EHDS]] (genomic secondary use)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (rare neurological disease genomics)

## Resources
- https://www.ga4gh.org/product/phenopackets/
- https://phenopacket-schema.readthedocs.io
- https://github.com/phenopackets/phenopacket-schema
