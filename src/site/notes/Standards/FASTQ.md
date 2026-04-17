---
{"dg-publish":true,"permalink":"/standards/fastq/","tags":["icm/uses"],"dg-note-properties":{"name":"FASTQ","aliases":["FASTQ format",".fastq",".fq"],"website":"https://samtools.github.io/hts-specs/SAMv1.pdf","type":"standard","scope":"international","domain":["genomics"],"status":"active","founded":2004,"parent_org":"Wellcome Sanger Institute (Cock et al. 2010; informal community standard)","tags":["icm/uses"]}}
---


# FASTQ — Raw Sequencing Read Format

## Overview
FASTQ is the universal format for storing raw sequencing reads — the direct output of every next-generation sequencing (NGS) instrument. Originally described by Cock et al. (2010, *Nucleic Acids Research*) to formalise an informal convention that had evolved from the Sanger-era FASTA format, FASTQ has no formal governance body but is universally adopted as the starting point of every genomics pipeline. Every sample sequenced at [[Actors/iGENSEQ\|iGENSEQ]] leaves the sequencer as FASTQ files before any downstream processing.

FASTQ stores both the **base calls** (the nucleotide sequence) and their associated **quality scores** (Phred-scaled probability of a base call error) in a simple four-line-per-read text format, making it self-contained and readable by every genomics tool.

## Format Structure
Each read in a FASTQ file occupies exactly four lines:

```
@read_name [optional description]
SEQUENCE
+
QUALITY_SCORES
```

- **Line 1** — `@` followed by the read identifier (instrument, flowcell, lane, tile, coordinates, index)
- **Line 2** — nucleotide sequence (A, T, G, C, N for ambiguous bases)
- **Line 3** — `+` separator (optionally repeating the read name)
- **Line 4** — quality scores encoded as ASCII characters; each character encodes a Phred quality score Q = −10 log₁₀(P), where P is the probability of a base call error

## Phred Quality Scores
The quality encoding maps ASCII characters to error probabilities:

| Phred score | Error probability | Accuracy |
|---|---|---|
| Q10 | 1 in 10 | 90% |
| Q20 | 1 in 100 | 99% |
| Q30 | 1 in 1,000 | 99.9% |
| Q40 | 1 in 10,000 | 99.99% |

Modern Illumina instruments routinely achieve Q30+ for most bases. The current standard encoding is **Phred+33** (Sanger encoding); the older Phred+64 (Illumina 1.3–1.7) is still occasionally encountered in legacy datasets.

## Paired-End Sequencing
Most modern NGS experiments produce **paired-end reads**: two FASTQ files per sample (`_R1.fastq.gz` and `_R2.fastq.gz`), where read 1 and read 2 are sequenced from opposite ends of the same DNA fragment. Paired-end data provides better genome coverage, more accurate alignment, and enables detection of structural variants and splice junctions.

## Compression
Raw FASTQ files are large — a whole-genome sequencing sample at 30× coverage produces ~50–100 GB of uncompressed FASTQ. In practice FASTQ files are always stored and transmitted as **gzip-compressed** (`.fastq.gz` or `.fq.gz`), which typically achieves 4–6× compression. Most tools accept `.fastq.gz` directly without decompression.

## Position in the NGS Pipeline
FASTQ is the first format in the genomics data processing chain:

```
Sequencer → FASTQ (raw reads; base calls + quality scores)
               ↓ quality control (FastQC, MultiQC, Trimmomatic, fastp)
               ↓ alignment (BWA-MEM2, STAR, HISAT2, minimap2, Cell Ranger)
            SAM/BAM/CRAM (aligned reads)
               ↓ variant calling / quantification
            VCF / AnnData
```

### Quality Control
Before alignment, FASTQ files are assessed and optionally trimmed:
- **FastQC** — per-base quality, GC content, adapter contamination, duplication rates
- **MultiQC** — aggregates FastQC reports across all samples in a study
- **Trimmomatic / fastp / Cutadapt** — adapter trimming and quality filtering

### FASTQ in Single-Cell Workflows
For single-cell RNA-seq (10x Genomics), FASTQ files contain cell barcodes and UMIs embedded in the read sequence. Cell Ranger (10x) and STARsolo demultiplex reads to cells and produce count matrices ([[Standards/AnnData\|AnnData]]/h5ad) directly from FASTQ.

## Data Deposition
FASTQ files are the preferred raw data submission format for sequence archives:
- **NCBI SRA** (Sequence Read Archive) — primary US raw read archive; cross-linked with [[Platforms/NCBI GEO\|NCBI GEO]]
- **ENA** ([[Platforms/ENA\|ENA]], European Nucleotide Archive, EMBL-EBI) — primary European raw read archive; INSDC partner
- **DDBJ** — Japanese national sequence archive; INSDC partner
- **[[Platforms/EGA\|EGA]]** — controlled-access human FASTQ; Crypt4GH encryption required for sensitive data

Raw FASTQ deposition is increasingly mandated by journals and funders (NIH DMS Policy, ANR, Horizon Europe) alongside processed data in [[Platforms/NCBI GEO\|NCBI GEO]] or [[Platforms/EGA\|EGA]].

## Connections
- Produced by: [[Actors/iGENSEQ\|iGENSEQ]] (all sequencing modalities: WGS, WES, RNA-seq, scRNA-seq, ATAC-seq)
- Downstream format: [[Standards/SAM-BAM-CRAM\|SAM-BAM-CRAM]] (after alignment); [[Standards/AnnData\|AnnData]] (after single-cell counting)
- Deposited in: NCBI SRA / [[Platforms/ENA\|ENA]] (open), [[Platforms/EGA\|EGA]] (controlled access human data)
- Governed by: [[Actors/GA4GH\|GA4GH]] (hts-specs; FASTQ informally part of the broader sequencing standards ecosystem)
- Analysis: [[Actors/DAC\|DAC]] (quality control pipelines; FastQC, MultiQC, fastp; alignment workflows)
- Related formats: FASTA (sequence only, no quality; used for reference genomes and assemblies)

## Resources
- https://samtools.github.io/hts-specs/SAMv1.pdf (FASTQ encoding described in SAM spec appendix)
- https://www.bioinformatics.babraham.ac.uk/projects/fastqc/ (FastQC quality control tool)
- https://multiqc.info (MultiQC — aggregate QC reports)
- https://www.ncbi.nlm.nih.gov/sra (NCBI SRA — primary FASTQ archive)
- https://www.ebi.ac.uk/ena (ENA — European FASTQ archive)
