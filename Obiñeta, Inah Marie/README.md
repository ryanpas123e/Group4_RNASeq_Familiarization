# Assignment 3 — RNA-Seq Literature Familiarization and Data Characterization (Salinity Stress)

# Title: 
Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in faba bean genotype, Hassawi-2
# Citation:  
Afzal, M., Alghamdi, S.S., Khan, M.A., Al-Faifi, S.A., & Habib ur Rahman, M. (2023). Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2. Scientific Reports, 13, 21223. 
ARTCLE LINK: https://doi.org/10.1038/s41598-023-48118-0

# Sequencing Data Summary
# Assigned RNA-seq accession number
- Control; Replicate 1 - 0h salt stress
- SRX19681425 (SRR23869388)
- Link: https://www.ncbi.nlm.nih.gov/sra/SRX19681425
- Paired-End Sequencing

# Number of reads / sequences
- Control_Rep1_R1: 28,209,473
- Control_Rep1_R2: 28,209,473

# Read length
- Control_Rep1_R1: 101 bp
- Control_Rep1_R2: 101 bp

# GC Content
- Control_Rep1_R1: 45%
- Control_Rep1_R2: 45%

| Metric | R1 | R2 |
|---|---|---|
| Per-base sequence quality | Pass — Q ~36.5, all green | Pass — Q ~36.6, all green |
| Adapter content | Pass — 0%, none detected | Pass — 0%, none detected |
| Overrepresented sequences | Warn — some overrepresented sequences flagged | Warn — some overrepresented sequences flagged |
| Per base sequence content | Fail — normal RNA-seq priming bias | Fail — normal RNA-seq priming bias |
| Sequence duplication levels | Fail — biological expression variation (highly expressed genes) | Fail — biological expression variation (highly expressed genes) |
| Per sequence GC content | Pass — 45% | Warn — slight deviation from expected distribution |


| Metric | R1 | R2 |
|---|---|---|
| Number of reads / sequences | 28,209,473 | 28,209,473 |
| Read length | 101 bp | 101 bp |
| Per-base sequence quality | Pass — Q ~36.5, all green | Pass — Q ~36.6, all green |
| Adapter content | Pass — 0%, none detected | Pass — 0%, none detected |
| Overrepresented sequences | Warn — some overrepresented sequences flagged | Warn — some overrepresented sequences flagged |
| Per base sequence content | Fail — normal RNA-seq priming bias | Fail — normal RNA-seq priming bias |
| Sequence duplication levels | Fail — biological expression variation (highly expressed genes) | Fail — biological expression variation (highly expressed genes) |
| Per sequence GC content | Pass — 45% | Warn — slight deviation from expected distribution |


# Short explanation of what the sample represents biologically
- This sample represents leaf tissue from *Vicia faba* (faba bean) at the vegetative three-leaf stage, harvested at 0 hours with no salt exposure. It serves as the unstressed biological control (Replicate 1), providing a baseline gene expression profile for comparison against salt-stressed samples.

# Summary of FastQC result
- Both R1 and R2 showed high overall sequencing quality, with per base sequence quality passing at a mean Phred score of around 36.5 to 36.6 across the entire read length, and no significant adapter contamination was detected. Some overrepresented sequences were flagged as a warning in both files, and per base sequence content failed due to biased base composition at the start of the reads, which is a common artifact of RNA-seq library preparation caused by random hexamer priming rather than a true sequencing problem. Sequence duplication levels also failed, but this is expected for RNA-seq since highly expressed transcripts naturally produce many duplicate reads, and R2 showed a slight deviation from the expected GC distribution, which was flagged as a warning. Overall, this dataset represents high-quality, Illumina-generated paired-end RNA-seq data that is suitable for downstream analysis.

# Answers to the interpretation questions
1.	What biological question was the original RNA-seq study trying to answer?
- The study aimed to identify which genes change expression in Vicia faba (faba bean) leaves under salt stress (200 mM) over time (6–72 hours), to understand how this plant responds and adapts to salinity at the transcriptome level.
  
2.	Why did the authors use RNA-seq instead of only examining the genome?
- The genome is static and identical across all cells and conditions; RNA-seq reveals which genes are actively transcribed and expressed that shows how gene activity changes under salt stress, which DNA sequence alone cannot tell you.
  
3.	What is the difference between genomic DNA and the RNA molecules measured by RNA-seq?
- Genomic DNA contains all genes permanently, in every cell. Meanwhile, RNA represents only genes that are actively expressed at a specific time and tissue; RNA is temporary, dynamic, and reflects functional gene activity.
  
4.	What is a biological replicate and why is it important?
- A biological replicate is an independent sample from a separate plant under the same conditions. It is important to distinguish true treatment effects from natural biological variation, making results statistically reliable and not due to chance.
  
5.	What is the difference between single-end and paired-end sequencing?
- Single-end sequences only one end of each cDNA fragment. Paired-end sequences both ends of the same fragment, producing two reads per fragment, giving better alignment accuracy and longer effective sequence coverage.
  
6.	What is a FASTQ file?
- A standard text file storing raw sequencing data with four lines per record: sequence ID, nucleotide sequence, a + separator, and ASCII-encoded per-base quality scores — combining sequence data with confidence values.
  
7.	What information does FastQC provide?
- FastQC generates a quality control report showing: read length, total reads, GC content, per-base quality scores, adapter contamination, overrepresented sequences, and other metrics to assess sequencing data reliability.
  
8.	What does a high per-base quality score indicate?
- A high score means very low probability of an incorrect base call. It tells that the sequencer is highly confident that the nucleotide identified at that position is accurate.
  
9.	Why can adapter contamination be a problem?
- Remaining adapter sequences do not belong to the sample and can interfere with read alignment, cause mismatches, and produce false gene expression signals, they must be trimmed before analysis.
  
10.	Were all RNA-seq samples in your group similar in quality? Explain.
- Yes, all samples showed comparable read counts (27–28 million), similar read length (101–150 bp), and consistent GC content (43–45%), indicating uniform sequencing quality across control and all time points.
  
11.	Did any sample show a possible quality problem? What was it?
- No major quality failures were observed; all samples had good quality scores and low adapter content. Minor variations in GC or read counts fell within expected biological variation, not technical error.
  
12.	What additional steps would be needed before the researchers could compare gene expression between control and treatment samples?
- Trim adapters and low-quality bases → align reads to the Vicia faba genome/transcriptome → count reads per gene → normalize read counts → perform statistical testing for differential expression.

# Short conclusion 
- This assignment provided hands-on experience examining real RNA-seq data from a published salinity-stress study in faba bean. Working with the Control_Rep1 sample (SRR23869388) showed how raw FASTQ reads are structured and how FastQC quality metrics reveal both the strengths  and expected quirks of RNA-seq data. Locating the BioProject and run accessions on NCBI SRA also demonstrated how public repositories make published sequencing data reproducible and reusable. This foundation in data quality assessment prepares the group for the next stage of the workflow: trimming, alignment or assembly, and differential expression analysis to identify the genes involved in salt-stress tolerance.



