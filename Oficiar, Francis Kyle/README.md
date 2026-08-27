# RNA-Seq Literature Familiarization and Data Characterization
**Student Name:** Oficiar, Francis Kyle A.

**Group Number:** Group 4 — Salinity Stress

## Title: Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in faba bean genotype, Hassawi-2
**Citation:** Afzal M, Alghamdi SS, Khan MA, Al-Faifi SA, Rahman MHU. (2023) *Scientific Reports*. DOI: 10.1038/s41598-023-48673-9

**RNA-seq accession number:** SRR23869378 (R1 and R2)

**Condition:** Treatment — 72 hrs salt stress (200 mM NaCl), Replicate 1

**Description:** Leaf tissue from salt-tolerant faba bean genotype Hassawi-2, harvested 6 hours after salt application. Represents the early transcriptomic response to salinity stress.

**Layout:** Paired-end sequencing

**Number of reads:** 31508305 (R1)

**Read Length:** 101 bp

**GC content:** R1: 43% / R2: 44%

## FastQC Quality Summary

| Metric | Forward Read (R1) | Reverse Read (R2) |
|---|---|---|
| **Per-base sequence quality** | **Pass** — Mean Q scores approximately 36.1–36.7; consistently high across all 101 bases | **Pass** — Mean Q scores approximately 35.7–36.4; consistently high across all 101 bases |
| **Adapter content** | **Pass** — No meaningful adapter contamination detected; only trace levels were present | **Pass** — No meaningful adapter contamination detected; only trace adapter levels were present |
| **Overrepresented sequences** | **Pass** — No overrepresented sequences detected | **Warn** — Poly-G sequence detected at approximately 0.265% |
| **Per-base sequence content** | **Fail** — Strong nucleotide bias at the first few bases, followed by a more stable composition | **Fail** — Nucleotide bias at the first few bases, followed by a more stable composition |
| **Per-sequence GC content** | **Pass** — GC content approximately 42% with an acceptable distribution | **Warn** — GC content approximately 43%; distribution shows an unusual high-GC tail |
| **Sequence duplication levels** | **Fail** — Only 29.05% of sequences were deduplicated, indicating high duplication | **Fail** — Only 30.71% of sequences were deduplicated, indicating high duplication |

**Overall quality:** Generally good. Both reads have excellent per-base quality and negligible adapter contamination. However, both reads show failed per-base sequence-content and sequence-duplication modules. The reverse read also has a Poly-G overrepresented sequence warning and a per-sequence GC-content warning. Trimming is not urgently required for quality reasons, but Poly-G trimming and duplicate levels should be evaluated before downstream analysis.

## Screenshots — 9 Figures

**Figure 1.** NCBI PubMed Central page for the study by Afzal et al. (2023).

**Figure 2.** Downloaded RNA Sequence data from NCBI into Galaxy.

**Figure 3.** Representative FASTQ file preview for the forward paired-end RNA-Seq reads 

**Figure 4.** Representative FASTQ file preview for the reverse paired-end RNA-Seq reads

**Figure 5.** FastQC Report on forward read (R1) RNA-seq FASTQ file

**Figure 6.** FastQC Report on reverse rea	d (R2) RNA-seq FASTQ file 

## Interpretation Questions

**1.** The study aimed to investigate the transcriptomic response of Vicia faba (faba bean) to salinity stress. Specifically, it sought to identify differentially expressed genes (DEGs) that contribute to salt tolerance or sensitivity by comparing leaf samples collected at different time points, such as 48 hours and 72 hours, under salt stress.

**2.** While the genome provides the genetic blueprint of what could happen, RNA-seq captures the functional state of the cell and shows what is happening under a specific condition. It allows researchers to quantify changes in gene expression, identify alternative splicing, and discover novel transcripts that are active during salt stress.

**3.** Genomic DNA is the stable, inherited genetic material present in almost every cell. The RNA molecules measured by RNA-seq are temporary transcripts produced from DNA when genes are expressed. Unlike DNA, RNA levels can change in response to environmental conditions and reflect the cell’s current biological activity.

**4.** A biological replicate is an independent biological sample from the same experimental condition, such as RNA extracted from different plants exposed to the same treatment. Biological replicates account for natural biological variation and help determine whether observed gene-expression changes are consistent and statistically reliable.

**5.** Single-end sequencing reads a DNA fragment from one end only. Paired-end sequencing reads the same fragment from both ends. Paired-end sequencing can improve mapping accuracy and help resolve transcript isoforms and other genomic features.

**6.** A FASTQ file is a text-based file that stores nucleotide sequences and their corresponding Phred quality scores. Each read usually contains four lines: the sequence identifier, the nucleotide sequence, a separator line, and the encoded quality-score string.

**7.** FastQC is a diagnostic tool used to assess sequencing-data quality. It evaluates per-base quality scores, GC-content distribution, sequence duplication, read length, adapter contamination, and overrepresented sequences that may indicate technical artifacts.

**8.** A high per-base quality score indicates a low probability of sequencing error. For example, a Phred score of Q30 represents an approximately 1 in 1,000 probability that a base was called incorrectly, corresponding to about 99.9% base-call accuracy.

**9.** Adapter contamination can interfere with read alignment and gene-expression analysis because adapter sequences do not originate from the biological sample. If present, they may reduce mapping rates and introduce bias, so they should be removed when necessary.

**10.** The samples were broadly similar in their technical characteristics, including paired-end sequencing, approximately 101-bp reads, and comparable read numbers. However, the samples showed high sequence duplication, with approximately 29–30% of sequences being deduplicated. This may reflect highly abundant transcripts, library complexity, or technical effects from library preparation.

**11.** Yes. The reverse reads showed a possible quality concern because they failed the per-base sequence-content module and received a warning for per-sequence GC content. They also contained a low-level overrepresented Poly-G sequence. However, both reads had high per-base quality and negligible adapter contamination, so the data may still be usable after appropriate quality assessment and preprocessing.

**12.** Before comparing gene expression between control and salt-stress samples, the researchers should perform quality control and trim adapters, low-quality bases, and Poly-G sequences if necessary. The cleaned reads should then be aligned to the Vicia faba reference genome or transcriptome, followed by gene-expression quantification. The data should be normalized, and statistical differential-expression analysis should be performed using biological replicates to identify genes that are significantly upregulated or downregulated under salt stress.

## Conclusion

Overall, this RNA-seq study used paired-end sequencing to investigate how salinity stress affects gene expression in Vicia faba. RNA-seq was appropriate because it measures actively expressed RNA molecules rather than only the genes present in genomic DNA, allowing researchers to identify genes and pathways involved in salt tolerance or sensitivity. The samples showed generally good sequencing quality, with 101-bp reads, high per-base quality scores, and little adapter contamination. However, failed per-base sequence-content and sequence-duplication modules were observed, along with a low-level Poly-G artifact and GC-content warning in the reverse reads. These issues should be assessed during preprocessing, but the data appear suitable for downstream analysis. Before comparing control and salt-stress samples, the reads should be cleaned, aligned or quantified, normalized, and analyzed statistically using biological replicates to identify reliable differential gene-expression patterns.
