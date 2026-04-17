---
{"dg-publish":true,"permalink":"/platforms/ena/","dg-note-properties":{"name":"European Nucleotide Archive","aliases":["ENA"],"website":"https://www.ebi.ac.uk/ena","type":"repository","scope":"international","domain":["genomics"],"status":"active","founded":2008,"parent_org":"EMBL-EBI"}}
---


# ENA — European Nucleotide Archive

## Overview
The European Nucleotide Archive (ENA) is the primary European open-access repository for raw nucleotide sequence data, operated by [[Actors/EMBL\|EMBL]]-EBI. It is one of three partner databases in the **International Nucleotide Sequence Database Collaboration (INSDC)**, alongside NCBI's Sequence Read Archive ([[Platforms/NCBI GEO\|NCBI GEO]]/SRA) and [[Platforms/DDBJ\|DDBJ]] (DNA Data Bank of Japan). The three databases mirror each other's data continuously, providing global redundancy and unrestricted access.

ENA accepts and archives raw sequencing reads (FASTQ, BAM, CRAM), assembled sequences, and annotated sequences from all organisms. It is the mandatory European deposition point for raw sequencing data associated with publications, and is the open-access raw data companion to [[Platforms/EGA\|EGA]] — which handles controlled-access human genomic data that cannot be publicly released.

## Scope
- **Raw reads** — FASTQ, BAM, and CRAM files from all sequencing technologies
- **Assembled sequences** — genome assemblies, transcriptome assemblies, metagenomes
- **Annotated sequences** — genes, coding sequences, non-coding RNA, regulatory elements
- **Functional annotations** — linked to protein databases (UniProt) and genome browsers (Ensembl)

## Relationship to EGA
ENA and [[Platforms/EGA\|EGA]] are complementary archives operated by [[Actors/EMBL\|EMBL]]-EBI serving distinct use cases:

| Feature | ENA | [[Platforms/EGA\|EGA]] |
|---|---|---|
| Access | Fully open | Controlled (DAC approval required) |
| Data sensitivity | Non-sensitive (model organisms, non-human, aggregated) | Sensitive human genomic/phenotypic data |
| Raw format | FASTQ, BAM, CRAM | FASTQ, BAM, CRAM (Crypt4GH encrypted) |
| Governance | EMBL-EBI (INSDC framework) | EMBL-EBI + CRG (Barcelona) |

In practice, a human genomics study will deposit raw FASTQ/CRAM files in [[Platforms/EGA\|EGA]] (controlled access), while the non-sensitive processed outputs (normalised expression matrices, variant summaries) may go to [[Platforms/NCBI GEO\|NCBI GEO]] or [[Platforms/EVA\|EVA]].

## INSDC Partnership
ENA, [[Platforms/NCBI GEO\|NCBI SRA]], and [[Platforms/DDBJ\|DDBJ]] synchronise data daily under the INSDC framework, meaning data submitted to any one archive becomes accessible via all three. This makes ENA the European mirror of all globally deposited raw sequence data.

## Connections
- Operated by: [[Actors/EMBL\|EMBL]]-EBI
- INSDC partners: [[Platforms/NCBI GEO\|NCBI GEO]] (SRA), [[Platforms/DDBJ\|DDBJ]]
- Controlled-access counterpart: [[Platforms/EGA\|EGA]] (human sensitive data)
- Open variant archive: [[Platforms/EVA\|EVA]] (short variants derived from ENA data)
- Part of: [[Governance/ELIXIR\|ELIXIR]] (core data resource)
- Standards: [[Standards/FASTQ\|FASTQ]], [[Standards/SAM-BAM-CRAM\|SAM-BAM-CRAM]], [[Actors/GA4GH\|GA4GH]] (Crypt4GH for sensitive submissions routed via EGA)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (raw sequencing data deposition from [[Actors/iGENSEQ\|iGENSEQ]] for non-sensitive and model organism studies)

## Resources
- https://www.ebi.ac.uk/ena
- https://www.ebi.ac.uk/ena/browser/submit (submission portal)
- https://www.insdc.org (INSDC collaboration)
