---
{"dg-publish":true,"permalink":"/standards/sam-bam-cram/","tags":["icm/uses"],"dg-note-properties":{"name":"Sequence Alignment Map / Binary Alignment Map / CRAM","aliases":["SAM","BAM","CRAM","SAM/BAM/CRAM","htslib formats"],"website":"https://samtools.github.io/hts-specs/","type":"standard","scope":"international","domain":["genomics"],"status":"active","founded":2009,"parent_org":"GA4GH / hts-specs community (Heng Li / Sanger Institute)","tags":["icm/uses"]}}
---


# SAM / BAM / CRAM — Sequence Alignment Formats

## Overview
SAM (Sequence Alignment Map), BAM (Binary Alignment Map), and CRAM are the universal formats for storing raw and aligned sequencing reads — the primary output of every next-generation sequencing (NGS) pipeline. Developed originally by Heng Li and colleagues at the Wellcome Sanger Institute in 2009 and now governed by [[Actors/GA4GH\|GA4GH]] through the hts-specs community, these formats form the backbone of all genomics data processing: every sample sequenced at [[Actors/iGENSEQ\|iGENSEQ]] passes through SAM/BAM/CRAM before reaching the endpoint formats ([[Standards/VCF\|VCF]] for variants, [[Standards/AnnData\|AnnData]] for single-cell expression counts).

The three formats are tightly related:
- **SAM** — human-readable tab-delimited text; the reference specification
- **BAM** — BGZF-compressed binary equivalent of SAM; the standard working format
- **CRAM** — reference-based compression; smaller than BAM (30–60% reduction); the archival standard

## What These Formats Store
A SAM/BAM/CRAM file stores every sequencing read alongside its alignment to a reference genome:

| Field | Description |
|---|---|
| Read name | Unique identifier for the read |
| FLAG | Bitwise flag encoding strand, pairing, mapping status |
| Reference name | Chromosome / contig the read aligns to |
| Position | 1-based leftmost mapping position |
| MAPQ | Mapping quality (Phred-scaled probability of wrong alignment) |
| CIGAR | Alignment descriptor (matches, insertions, deletions, soft-clips) |
| Sequence | Base calls |
| Quality | Phred-scaled base quality scores |
| Optional tags | Metadata fields (read group, barcode, UMI, sample ID, aligner details) |

The **header section** (lines beginning `@`) stores reference genome metadata, read group information (sample, library, platform), and program records (alignment tool and parameters) — essential provenance for reproducibility.

## The Three Formats in Practice

### SAM
Plain text; human-inspectable with standard tools (`head`, `grep`); used as interchange format and for debugging. Not used for storage or analysis at scale due to size.

### BAM
The working standard. BGZF (Blocked GNU Zip Format) compression enables random access via `.bai` index files — a key property for variant calling and genome browsers. Tools: **samtools**, **Picard**, **GATK**, **IGV**. Typical size: 10–100 GB per whole-genome sample.

### CRAM
Reference-based compression: instead of storing the full sequence, CRAM stores only differences from the reference genome, achieving 30–60% size reduction over BAM with no information loss (lossless) or minor approximation (lossy, for archiving). Requires access to the reference genome for decoding. Increasingly the archival standard — [[Platforms/EGA\|EGA]], SRA, and [[Actors/EMBL\|EMBL]]-EBI's [[Platforms/ENA\|ENA]] all accept CRAM. Governed by [[Actors/GA4GH\|GA4GH]]; encrypted CRAM via Crypt4GH is the recommended format for controlled-access human genomic data submission.

## Position in the NGS Pipeline

```
Sequencer → FASTQ (raw reads)
              ↓ alignment (BWA-MEM2, STAR, HISAT2, minimap2)
            SAM/BAM/CRAM (aligned reads)
              ↓ variant calling (GATK HaplotypeCaller, DeepVariant)
            VCF (variants)
              ↓ OR ↓ counting (featureCounts, STARsolo, Cell Ranger)
            Count matrix → AnnData / h5ad (single-cell expression)
```

BAM/CRAM is the format that sits between raw sequencing and all downstream analyses — variant calling, expression quantification, structural variant detection, methylation calling, and chromatin accessibility analysis all operate on aligned BAM/CRAM files.

## Key Tools (htslib ecosystem)
The **htslib** C library underpins all major tools operating on these formats:
- **samtools** — universal toolkit: view, sort, index, merge, flagstat, idxstats, depth, mpileup
- **Picard** — Java toolkit: mark duplicates, collect metrics, fix mate pairs, add read groups
- **GATK** — Broad Institute variant calling pipeline; operates on BAM/CRAM
- **IGV** (Integrative Genomics Viewer) — interactive BAM visualisation; used at [[Actors/DAC\|DAC]] and [[Actors/iGENSEQ\|iGENSEQ]]
- **DeepVariant** — Google's deep-learning variant caller; BAM/CRAM input

## Data Deposition
BAM/CRAM files are the primary submission format for controlled-access human genomics repositories:
- **[[Platforms/EGA\|EGA]]** (European Genome-phenome Archive) — CRAM recommended for all human WGS/WES submissions; Crypt4GH encryption required
- **[[Platforms/dbGaP\|dbGaP]]** — BAM/CRAM for GWAS and WGS controlled-access submissions
- **[[Platforms/NCBI GEO\|NCBI GEO]]** / SRA — BAM for aligned RNA-seq, ATAC-seq, ChIP-seq data
- **[[Platforms/EVA\|EVA]]** — accepts VCF derived from BAM/CRAM processing; raw reads via [[Platforms/ENA\|ENA]]

## GA4GH Standards Integration
[[Actors/GA4GH\|GA4GH]] governs SAM/BAM/CRAM through the hts-specs repository and has built additional standards on top:
- **Crypt4GH** — encryption standard wrapping BAM/CRAM for secure federated access
- **htsget** — streaming protocol for retrieving subsets of BAM/CRAM over HTTP
- **DRS** (Data Repository Service) — cloud-native URL scheme for referencing BAM/CRAM files in federated analyses
- **WES** (Workflow Execution Service) — runs analysis pipelines on remote BAM/CRAM without data transfer

## Connections
- Governed by: [[Actors/GA4GH\|GA4GH]] (hts-specs)
- Upstream format: [[Standards/FASTQ\|FASTQ]] (raw reads from sequencer)
- Downstream formats: [[Standards/VCF\|VCF]] (variant calling), [[Standards/AnnData\|AnnData]] (expression quantification)
- Deposited in: [[Platforms/EGA\|EGA]], [[Platforms/dbGaP\|dbGaP]], [[Platforms/NCBI GEO\|NCBI GEO]] / SRA, [[Platforms/EVA\|EVA]] (via [[Platforms/ENA\|ENA]])
- Encryption: Crypt4GH ([[Actors/GA4GH\|GA4GH]] standard for controlled-access submissions)
- Relevant to: [[Actors/iGENSEQ\|iGENSEQ]] (primary output of all WGS, WES, RNA-seq, ATAC-seq pipelines); [[Actors/DAC\|DAC]] (analysis pipelines operating on BAM/CRAM); [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] (downstream of banked DNA)

## Resources
- https://samtools.github.io/hts-specs/ (SAM/BAM/CRAM specification)
- https://samtools.github.io/hts-specs/SAMv1.pdf (SAM format specification v1)
- https://samtools.github.io/hts-specs/CRAMv3.pdf (CRAM v3 specification)
- https://www.htslib.org (htslib and samtools)
- https://gatk.broadinstitute.org (GATK variant calling pipeline)
- https://igv.org (IGV — BAM/CRAM visualisation)
