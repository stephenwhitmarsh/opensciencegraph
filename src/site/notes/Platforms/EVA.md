---
{"dg-publish":true,"permalink":"/platforms/eva/","dg-note-properties":{"name":"European Variation Archive","aliases":["EVA"],"website":"https://www.ebi.ac.uk/eva/","type":"repository","scope":"european","domain":["genomics"],"status":"active","founded":2013,"parent_org":"EMBL-EBI"}}
---


# EVA — European Variation Archive

## Overview
The European Variation Archive (EVA) is an open-access repository for all types of genetic variant data from all species, operated by EMBL-EBI. Unlike [[Platforms/EGA\|EGA]] (which stores controlled-access individual-level genomic data), EVA stores **variant-level data** — the aggregated, anonymised catalogue of genetic variants identified in studies — which can be shared without privacy restrictions.

EVA is the primary European archive for variant submissions and is a member of the **dbSNP/dbVar** international network alongside NCBI's dbSNP (short variants) and dbVar (structural variants). It receives submissions from European studies and mirrors relevant data from its international partners.

## What EVA Stores
- **Short variants (SNPs and indels)** — single nucleotide polymorphisms and small insertions/deletions in [[Standards/VCF\|VCF]] format
- **Structural variants** — copy number variants (CNVs), inversions, translocations
- **Somatic variants** — from cancer and disease studies
- **Clinical variants** — variants with clinical significance annotations (cross-referenced to ClinVar)
- Species coverage: human (primary focus), model organisms, livestock, plants

## Relationship to dbSNP and ClinVar
EVA, dbSNP (NCBI), and ClinVar together form the international variant data ecosystem: **EVA** — European submission point; open-access; all variant types; **dbSNP** (NCBI) — US mirror; assigns rs# identifiers to short variants; **ClinVar** (NCBI) — clinical interpretation of variants; pathogenicity classifications. EVA and dbSNP exchange data via the INSDC framework.

## Relevance to Neuroscience
For [[Actors/Paris Brain Institute\|Paris Brain Institute]], EVA is relevant as a **deposition target** for variant data from neurogenomics studies at [[Actors/iGENSEQ\|iGENSEQ]] (required for journal publication compliance), an **access point** for variant data from European neurological disease studies, and part of the [[Actors/GA4GH\|GA4GH]] Beacon network — EVA datasets are discoverable via Beacon API queries.

## Connections
- Operated by: EMBL-EBI
- Part of: [[Governance/ELIXIR\|ELIXIR]] data services
- International partners: dbSNP (NCBI), [[Platforms/DDBJ\|DDBJ]] (INSDC network)
- Format: [[Standards/VCF\|VCF]] (primary submission format)
- Standards: [[Actors/GA4GH\|GA4GH]] (Beacon API for variant discovery)
- Controlled-access complement: [[Platforms/EGA\|EGA]] (individual-level data)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (variant deposition from neurological disease genomics studies)

## Resources
- https://www.ebi.ac.uk/eva/
- https://www.ebi.ac.uk/eva/webservices/eva/swagger-ui.html (REST API)
