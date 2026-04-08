---
{"dg-publish":true,"permalink":"/01-actors/ga-4-gh/","dg-note-properties":{"name":"Global Alliance for Genomics and Health","aliases":["GA4GH"],"website":"https://www.ga4gh.org","type":"consortium","scope":"international","domain":["genomics","clinical"],"status":"active","founded":2013}}
---


# GA4GH - Global Alliance for Genomics and Health

## Overview
GA4GH is the international standards-setting body for genomics and health-related
data sharing, analogous to [[01_Actors/INCF\|INCF]] for neuroscience. Founded in 2013 by a
consortium of research and clinical institutions, it develops a coordinated suite
of technical standards and policy frameworks to enable responsible, federated
sharing of genomic and clinical data at scale. Its standards are directly relevant
to [[00_Core/Paris Brain Institute\|Paris Brain Institute]] through neurogenomics research, rare neurological
disease diagnostics, and compliance with [[04_Governance/EHDS\|EHDS]] secondary use requirements.

## Standards Governed
- [[02_Standards/VCF\|VCF]] — Variant Call Format; the universal standard for genomic variant data
- [[02_Standards/Phenopackets\|Phenopackets]] — computable phenotype + genomic data exchange standard (ISO approved)
- SAM/BAM/CRAM — sequence alignment formats for raw and aligned sequencing reads
- Data Use Ontology (DUO) — machine-readable consent and data access conditions
- Beacon API — protocol for querying variant presence across federated datasets
- Variation Representation Specification (VRS) — unambiguous computational
  representation of genomic variants
- Crypt4GH — encryption standard for genomic files (BAM, CRAM, VCF)
- Data Repository Service (DRS), Workflow Execution Service (WES),
  Task Execution Service (TES) — cloud-native APIs for data access and analysis

## Organisation
GA4GH works through eight thematic Work Streams (Clinical & Phenotypic Data
Capture, Data Security, Genomic Knowledge Standards, Large Scale Genomics,
Metadata, Network & Cloud, Regulatory & Ethics, and Variant Interpretation)
and is informed by 24+ Driver Projects representing major genomics initiatives.

## GA4GH Neuroscience Community
The **GA4GH Neuroscience Community** (https://www.ga4gh.org/community/neuroscience-community/)
is a cross-cutting community of practice co-led by GA4GH and [[01_Actors/INCF\|INCF]], focused on
applying GA4GH genomic data standards to neuroscience research. It works on:
- Adapting [[02_Standards/Phenopackets\|Phenopackets]] and [[02_Standards/VCF\|VCF]] for neurological disease genomics
- Connecting brain disease genomics with clinical phenotype data ([[02_Standards/HPO\|HPO]], [[02_Standards/ORDO\|ORDO]])
- Interoperability between genomics repositories ([[03_Platforms/EGA\|EGA]], [[03_Platforms/dbGaP\|dbGaP]]) and
  neuroscience data archives ([[03_Platforms/DANDI Archive\|DANDI Archive]], [[03_Platforms/OpenNeuro\|OpenNeuro]])
- Relevant to [[00_Core/Paris Brain Institute\|Paris Brain Institute]] through neurogenomics programmes
  and [[01_Actors/iGENSEQ\|iGENSEQ]] data deposition

## Connections
- Standards produced: [[02_Standards/VCF\|VCF]], [[02_Standards/Phenopackets\|Phenopackets]]
- Ontologies used: [[02_Standards/HPO\|HPO]] (Human Phenotype Ontology, integrated in Phenopackets)
- Interoperates with: [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/SNOMED CT\|SNOMED CT]]
- Adopted by: [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[04_Governance/ELIXIR\|ELIXIR]], [[01_Actors/UK Biobank\|UK Biobank]], [[04_Governance/Health Data Hub\|Health Data Hub]]
- Required by: [[04_Governance/EHDS\|EHDS]] (genomic data secondary use from March 2031)
- Partners: [[01_Actors/INCF\|INCF]] (GA4GH–INCF Neuroscience Community co-lead programme)
- Related: [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]], [[04_Governance/EATRIS\|EATRIS]], [[04_Governance/ECRIN\|ECRIN]]

## Resources
- https://www.ga4gh.org
- https://www.ga4gh.org/genomic-data-toolkit/
