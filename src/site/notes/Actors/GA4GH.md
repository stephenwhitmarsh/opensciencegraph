---
{"dg-publish":true,"permalink":"/actors/ga-4-gh/","dg-note-properties":{"name":"Global Alliance for Genomics and Health","aliases":["GA4GH"],"website":"https://www.ga4gh.org","type":"consortium","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2013}}
---


# GA4GH - Global Alliance for Genomics and Health

## Overview
GA4GH is the international standards-setting body for genomics and health-related data sharing, analogous to [[Actors/INCF\|INCF]] for neuroscience. Founded in 2013 by a consortium of research and clinical institutions, it develops a coordinated suite of technical standards and policy frameworks to enable responsible, federated sharing of genomic and clinical data at scale. Its standards are directly relevant to [[Actors/Paris Brain Institute\|Paris Brain Institute]] through neurogenomics research, rare neurological disease diagnostics, and compliance with [[Governance/EHDS\|EHDS]] secondary use requirements.

## Standards Governed
- [[Standards/VCF\|VCF]] — Variant Call Format; the universal standard for genomic variant data
- [[Standards/Phenopackets\|Phenopackets]] — computable phenotype + genomic data exchange standard (ISO approved)
- [[Standards/SAM-BAM-CRAM\|SAM-BAM-CRAM]] — sequence alignment formats for raw and aligned sequencing reads
- Data Use Ontology (DUO) — machine-readable consent and data access conditions
- Beacon API — protocol for querying variant presence across federated datasets
- Variation Representation Specification (VRS) — unambiguous computational representation of genomic variants
- Crypt4GH — encryption standard for genomic files (BAM, CRAM, VCF)
- Data Repository Service (DRS), Workflow Execution Service (WES), Task Execution Service (TES) — cloud-native APIs for data access and analysis

## Organisation
GA4GH works through eight thematic Work Streams (Clinical & Phenotypic Data Capture, Data Security, Genomic Knowledge Standards, Large Scale Genomics, Metadata, Network & Cloud, Regulatory & Ethics, and Variant Interpretation) and is informed by 24+ Driver Projects representing major genomics initiatives.

## GA4GH Neuroscience Community
The **GA4GH Neuroscience Community** (https://www.ga4gh.org/community/neuroscience-community/) is a cross-cutting community of practice co-led by GA4GH and [[Actors/INCF\|INCF]], focused on applying GA4GH genomic data standards to neuroscience research. It works on:
- Adapting [[Standards/Phenopackets\|Phenopackets]] and [[Standards/VCF\|VCF]] for neurological disease genomics
- Connecting brain disease genomics with clinical phenotype data ([[Standards/HPO\|HPO]], [[Standards/ORDO\|ORDO]])
- Interoperability between genomics repositories ([[Platforms/EGA\|EGA]], [[Platforms/dbGaP\|dbGaP]]) and neuroscience data archives ([[Platforms/DANDI Archive\|DANDI Archive]], [[Platforms/OpenNeuro\|OpenNeuro]])
- Relevant to [[Actors/Paris Brain Institute\|Paris Brain Institute]] through neurogenomics programmes and [[Actors/iGENSEQ\|iGENSEQ]] data deposition

## Connections
- Standards produced: [[Standards/VCF\|VCF]], [[Standards/Phenopackets\|Phenopackets]], [[Standards/SAM-BAM-CRAM\|SAM-BAM-CRAM]]
- Ontologies used: [[Standards/HPO\|HPO]] (Human Phenotype Ontology, integrated in Phenopackets)
- Interoperates with: [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/SNOMED CT\|SNOMED CT]]
- Adopted by: [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/ELIXIR\|ELIXIR]], [[Actors/UK Biobank\|UK Biobank]], [[Governance/Health Data Hub\|Health Data Hub]]
- Required by: [[Governance/EHDS\|EHDS]] (genomic data secondary use from March 2031)
- Partners: [[Actors/INCF\|INCF]] (GA4GH–INCF Neuroscience Community co-lead programme)
- Related: [[Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[Governance/EATRIS\|EATRIS]], [[Governance/ECRIN\|ECRIN]]

## Resources
- https://www.ga4gh.org
- https://www.ga4gh.org/genomic-data-toolkit/
