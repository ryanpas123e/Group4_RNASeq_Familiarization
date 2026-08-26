# RNA-Seq Literature Familiarization and Data Characterization 
**Student Name:** Jade Angela Suan

**Group Number:** Group 4 — Salinity Stress

## Title: Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in faba bean genotype, Hassawi-2
**Citation:** Afzal M, Alghamdi SS, Khan MA, Al-Faifi SA, Rahman MHU. (2023) *Scientific Reports*. DOI: 10.1038/s41598-023-48673-9

**RNA-seq accession number:** SRR23869373 (R1 and R2)

**Condition:** Treatment — 6h salt stress (200 mM NaCl), Replicate 1

**Description:** Leaf tissue from salt-tolerant faba bean genotype Hassawi-2, harvested 6 hours after salt application. Represents the early transcriptomic response to salinity stress.

**Layout:** Paired-end sequencing

**Number of reads:** 28,211,353 (R1)

**Read Length:** 101 bp

**GC content:** R1: 43% / R2: 44%

## FastQC Summary Results

| Metric | R1 | R2 |
|---|---|---|
| Per-base sequence quality |  Pass — Q ~36, all green |  Pass — Q ~35–36, all green |
| Adapter content |  Pass — 0% none detected |  Pass — 0% none detected |
| Overrepresented sequences |  Pass — None found |  Warn — PolyG artifact 0.24%, Illumina noise |
| Per base sequence content |  Fail — Normal RNA-seq priming bias |  Fail — Normal RNA-seq priming bias |
| Sequence duplication levels |  Fail — Biological expression variation |  Fail — Biological expression variation |

**Overall quality:** Excellent. All critical metrics pass. Failures are expected for RNA-seq. No trimming required.

## Screenshots — 9 Figures

**Figure 1.** Galaxy interface showing the Download and Extract Reads from NCBI SRA tool with accession SRR23869373 entered

**Figure 2.** Galaxy job submission confirmation showing successful SRA download job added to queue

**Figure 3.** FASTQ file preview for R1 (forward reads) displaying the standard 4-line sequence format

**Figure 4.** FASTQ file preview for R2 (reverse reads) confirming paired-end data structure

**Figure 5.** FastQC Basic Statistics summary for R1 — showing total reads (28,211,353), read length (101 bp), and GC content (43%)

**Figure 6.** FastQC Basic Statistics summary for R2 — showing total reads, read length (101 bp), and GC content (44%)

**Figure 7.** FastQC Per Base Sequence Quality Plot — R1, showing all quality scores in the green region at approximately Q36

**Figure 8.** FastQC Per Base Sequence Quality Plot — R2, showing all quality scores in the green region at approximately Q35–36

**Figure 9.** FastQC Overrepresented Sequences — minor poly-G artifact (0.24%) in R2, common Illumina sequencing artifact not biological contamination

## Interpretation Questions

**1.** The study aims to identify genes and molecular pathways associated with salinity stress tolerance in faba bean by comparing gene expression under normal and salt stress conditions.

**2.** The genome contains all genes but does not show which are active. RNA-seq measures gene expression, which genes are transcribed and at what levels under specific conditions.

**3.** Genomic DNA is static and identical in all cells; RNA is dynamic and changes depending on tissue, development stage, and environment.

**4.** An independent sample from a separate plant grown and treated identically. It accounts for natural variation and ensures results are reliable.

**5.** Single-end reads one end of the fragment; paired-end reads from both ends, providing more information and better alignment accuracy.

**6.** Standard sequencing output format containing the nucleotide sequence and a Phred quality score for each base.

**7.** Quality control tool that evaluates read quality, read length, GC content, adapter contamination, duplication levels, and overrepresented sequences.

**8.** Indicates highly accurate base calls. Consistently high scores across all positions confirm reliable data.

**9.** Leftover adapter sequences interfere with read alignment and cause incorrect mapping results.

**10.** All samples show very similar excellent quality - high quality scores, 101 bp length, no adapters, GC 43–45%.

**11.** R2 shows a minor poly-G artifact (0.24%) - a common Illumina sequencing artifact, not biological contamination.

**12.** Trim if needed → align reads to transcriptome → count gene expression → normalize → identify differentially expressed genes.

## Conclusion
The RNA-seq data for this sample is of excellent quality consistently high per-base quality scores, no adapter contamination, and uniform read length. The warnings and failures observed are characteristic of RNA-seq methodology and do not indicate technical issues. The data is clean, reliable, and suitable for downstream analysis such as transcriptome assembly and differential gene expression testing.





