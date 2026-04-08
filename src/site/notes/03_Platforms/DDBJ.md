---
{"dg-publish":true,"permalink":"/03-platforms/ddbj/","dg-note-properties":{"name":"DNA Data Bank of Japan","aliases":["DDBJ"],"website":"https://www.ddbj.nig.ac.jp","type":"repository","scope":"international","domain":["genomics"],"status":"active","founded":1986,"parent_org":"National Institute of Genetics (NIG) / Research Organization of Information and Systems (ROIS), Japan"}}
---


# DDBJ — DNA Data Bank of Japan

## Overview
The DNA Data Bank of Japan (DDBJ) is Japan's national nucleotide sequence database
and the Asian partner in the **International Nucleotide Sequence Database
Collaboration (INSDC)**, alongside [[03_Platforms/NCBI GEO\|NCBI GEO]] / NCBI (USA) and ENA / EMBL-EBI
(Europe). DDBJ collects, annotates, and distributes nucleotide sequence data
submitted by researchers worldwide and fully mirrors all data with its INSDC
partners — meaning data submitted to any of the three databases is automatically
available from all three.

## INSDC Collaboration
The INSDC ensures that nucleotide sequence data is globally accessible regardless
of where it was submitted:
- **DDBJ** (Japan) — accepts submissions from Asia-Pacific region; operates
  DDBJ Sequence Read Archive (DRA) for raw reads
- **NCBI** (USA) — GenBank for annotated sequences; SRA for raw reads
- **ENA** (EMBL-EBI, Europe) — European Nucleotide Archive

All three databases exchange data daily and provide identical access to the
complete INSDC dataset. For European researchers, submission to ENA is most
natural; DDBJ is the equivalent entry point for Japanese/Asian data producers.

## DDBJ Services
- **DDBJ** — annotated nucleotide sequences (equivalent to GenBank/ENA)
- **DRA** — DDBJ Sequence Read Archive; raw next-generation sequencing reads
- **GEA** — Genomic Expression Archive; functional genomics data (equivalent
  to [[03_Platforms/NCBI GEO\|NCBI GEO]] and ArrayExpress)
- **JGA** — Japanese Genotype-phenotype Archive; controlled-access human data
  (equivalent to [[03_Platforms/EGA\|EGA]])
- **D-way** — unified submission portal for all DDBJ services

## Relevance to Open Neuroscience
For [[00_Core/Paris Brain Institute\|Paris Brain Institute]], DDBJ is relevant as:
- Part of the **global sequence data infrastructure** — BIDS datasets on
  [[03_Platforms/OpenNeuro\|OpenNeuro]] linking to associated genomics data will ultimately have that
  sequence data mirrored in DDBJ via INSDC
- **JGA** is a controlled-access repository for sensitive Japanese genomic data
  from neurological disease cohorts, increasingly relevant for international
  collaborations
- DDBJ's GEA hosts Japanese brain transcriptomics datasets accessible to
  French researchers

## Connections
- Part of: INSDC (with [[03_Platforms/NCBI GEO\|NCBI GEO]] / NCBI and ENA / EMBL-EBI)
- Operated by: NIG / ROIS (Japan)
- Controlled-access equivalent: JGA (Japanese Genotype-phenotype Archive)
- Open-access expression data: GEA (mirrors [[03_Platforms/NCBI GEO\|NCBI GEO]] / ArrayExpress)
- Standards: [[02_Standards/VCF\|VCF]], [[01_Actors/GA4GH\|GA4GH]] (Beacon API)
- Relevant to: [[00_Core/Paris Brain Institute\|Paris Brain Institute]] (global sequence data access;
  international genomics collaborations)

## Resources
- https://www.ddbj.nig.ac.jp
- https://ddbj.nig.ac.jp/resource/sra-submission (DRA submission)
- https://www.insdc.org (INSDC collaboration overview)
