---
{"dg-publish":true,"permalink":"/02-standards/omim/","dg-note-properties":{"name":"Online Mendelian Inheritance in Man","aliases":["OMIM"],"website":"https://omim.org","type":"terminology","scope":"international","domain":["genomics","clinical"],"status":"active","founded":1966,"parent_org":"Johns Hopkins University / McKusick-Nathans Institute of Genetic Medicine"}}
---


# OMIM — Online Mendelian Inheritance in Man

## Overview
Online Mendelian Inheritance in Man (OMIM) is the authoritative compendium of
human genes and genetic phenotypes, maintained by Johns Hopkins University since
1966 (originally as a print catalogue by Victor McKusick). Each entry in OMIM
has a unique **MIM number** identifying either a gene or a phenotype/disease,
and describes the molecular basis, inheritance pattern, clinical features, and
genotype-phenotype relationships.

OMIM is the primary reference database linking specific genetic variants to
human disease phenotypes, and is central to rare disease genomics, variant
interpretation, and neurogenomics workflows at institutions like
[[00_Core/Paris Brain Institute\|Paris Brain Institute]].

## MIM Number System
OMIM assigns unique 6-digit identifiers:
- **Gene entries** (e.g. SNCA gene — MIM #163890) — describe the gene,
  its function, and associated phenotypes
- **Phenotype entries** (e.g. Parkinson disease 1 — MIM #168601) — describe
  the disease, its clinical features, inheritance, and causative genes
- **#** prefix — phenotype with known molecular basis
- **%** prefix — phenotype with unknown molecular basis or suspected genetic
- **+** prefix — gene of known sequence and phenotype

## Role in Neurological Disease Research
OMIM is the primary lookup for:
- **Rare neurological disease diagnosis** — identifies causative genes for
  rare movement disorders, hereditary ataxias, hereditary spastic paraplegias,
  lysosomal storage diseases, and channelopathies
- **Variant interpretation** — ClinVar and clinical genetics labs use OMIM
  phenotype entries as reference when classifying variants as pathogenic
- **Gene discovery** — novel gene-disease associations reported in OMIM
  before appearing in other databases

## Integration with Open Science Standards
- **[[02_Standards/HPO\|HPO]]** — OMIM phenotype entries cross-referenced with HPO terms;
  HPO uses OMIM as a primary source for rare disease phenotype descriptions
- **[[02_Standards/MONDO\|MONDO]]** — OMIM MIM numbers are a primary source harmonised in MONDO;
  `OMIM:xxxxxx` cross-references appear in every MONDO rare disease concept
- **[[02_Standards/ORDO\|ORDO]]** — Orphanet maps its ORDO identifiers to OMIM MIM numbers
- **[[02_Standards/Phenopackets\|Phenopackets]]** — OMIM disease IDs used alongside HPO terms to
  describe rare disease cases in GA4GH Phenopackets
- **[[02_Standards/VCF\|VCF]]** / variant annotation — variant annotation pipelines (Ensembl VEP,
  ANNOVAR) include OMIM phenotype annotations in output
- **[[02_Standards/GO\|GO]]** — OMIM gene entries cross-linked to GO functional annotations

## Connections
- Produced by: Johns Hopkins University / McKusick-Nathans Institute
- Maps to / cross-references: [[02_Standards/HPO\|HPO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ORDO\|ORDO]], [[02_Standards/Phenopackets\|Phenopackets]]
- Used in variant annotation: [[02_Standards/VCF\|VCF]] pipelines (Ensembl VEP, ANNOVAR)
- Used by: [[02_Standards/ERN Vocabularies\|ERN Vocabularies]] (ERN-RND, ERN-EpiCARE rare disease registries),
  clinical genetics labs, [[01_Actors/iGENSEQ\|iGENSEQ]] (variant interpretation)
- Related: ClinVar (NCBI — clinical variant classifications referencing OMIM)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (rare neurological disease
  genomics, variant interpretation, HPO/ORDO phenotyping)

## Resources
- https://omim.org
- https://omim.org/downloads (bulk data downloads — CC BY-NC-ND licence)
- https://www.ncbi.nlm.nih.gov/clinvar/ (ClinVar — clinical variant db using OMIM)
