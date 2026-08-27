# Assignment 3 – RNA-Seq Familiarization

## Student Information

**Student:** Pasculado, Mark Ryan  
**Group:** Group 4 – Salinity Stress

---

## Group Paper

### Title

*Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2*

### Citation

Afzal, M., Alghamdi, S. S., Khan, M. A., Al-Faifi, S. A., & Rahman, M. H. ur. (2023). Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2. *Scientific Reports, 13*, 21223.

**DOI:** 10.1038/s41598-023-48118-0

**BioProject:** PRJNA943415

---

## Assigned RNA-Seq Sample

**Run accession:** SRR23869379

**Condition:** Treatment – 48-hour salt stress

**Biological replicate:** R1

**Sequencing type:** Paired-end

**Number of reads:** 31,549,121

**Read length:** 101 bp

**GC content:** Approximately 43–44%
**SRA Link:** https://www.ncbi.nlm.nih.gov/sra/SRX19681434[accn]

---
## Biological Meaning of the Sample

SRR23869379 represents a leaf RNA-seq sample from the salt-tolerant faba bean genotype Hassawi-2 exposed to 200 mM NaCl for 48 hours. The sample was used to examine changes in gene expression associated with prolonged salinity stress.

---
## Sequencing Data Summary

| RNA-seq Characteristic | Forward Read (R1) | Reverse Read (R2) |
|---|---|---|
| **RNA-seq run accession** | SRR23869379 | SRR23869379 |
| **Condition** | 48-hour salt stress | 48-hour salt stress |
| **Sequencing type** | Paired-end | Paired-end |
| **Number of reads/sequences** | 31,549,121 | 31,549,121 |
| **Read length** | ~98 bp | ~98 bp |
| **File size** | ~1.8 GB | ~1.8 GB |
| **GC content** | ~43–44% | ~43–44% |
| **Per-base sequence quality** | Pass | Pass |
| **Adapter content** | Pass | Pass |
| **Overrepresented sequences** | Pass | Warning |
| **Main QC observation** | **Fail:** Per Base Sequence Content | **Fail:** Per Base Sequence Content; **Warn:** Per Sequence GC Content |

### Overall QC

The sample showed good overall sequencing quality, but both R1 and R2 had a failure in Per Base Sequence Content. R2 also showed a warning for Per Sequence GC Content. Overall, the sample was generally of good quality but showed some sequence-content bias that should be considered during further analysis.

## FastQC Results

The sample showed generally good sequencing quality. It contained 31,549,121 reads with a read length of approximately 101 bp and a GC content of about 43–44%.

However, FastQC showed a **failure in Per Base Sequence Content** for the forward read (R1) and a **failure in Per Base Sequence Content with a warning for Per Sequence GC Content** in the reverse read (R2). Other quality indicators, including general per-base sequence quality, adapter content, and overrepresented sequences, were generally acceptable.

Overall, the sample was comparable to the other group samples but had some QC warnings that should be considered during further analysis.

---
## Interpretation Questions

### 1. What biological question was the original RNA-seq study trying to answer?

The study aimed to determine how salinity stress affects gene expression in faba bean and to identify genes involved in salt-stress tolerance.

### 2. Why did the authors use RNA-seq instead of only examining the genome?

RNA-seq shows which genes are actively expressed and how their expression changes under salt stress, whereas the genome mainly shows which genes are present.

### 3. What is the difference between genomic DNA and the RNA molecules measured by RNA-seq?

Genomic DNA contains the organism's complete genetic information, while RNA molecules reflect genes that are actively expressed in a particular tissue or condition.

### 4. What is a biological replicate and why is it important?

A biological replicate is an independent sample from the same experimental condition. Replicates help measure biological variation and determine whether observed gene-expression differences are reliable.

### 5. What is the difference between single-end and paired-end sequencing?

Single-end sequencing reads a DNA fragment from one end, while paired-end sequencing reads the same fragment from both ends.

### 6. What is a FASTQ file?

A FASTQ file contains nucleotide sequences together with quality scores for each base.

### 7. What information does FastQC provide?

FastQC evaluates sequencing quality, including base quality, GC content, sequence length, adapter contamination, duplication, and overrepresented sequences.

### 8. What does a high per-base quality score indicate?

A high per-base quality score indicates that the sequencing instrument has high confidence in the accuracy of the base calls.

### 9. Why can adapter contamination be a problem?

Adapter contamination can interfere with read alignment and gene-expression analysis, so adapter sequences may need to be removed through trimming.

### 10. Were all RNA-seq samples in your group similar in quality? Explain.

The samples were generally similar, with comparable read lengths, read numbers, and GC contents. However, some samples showed minor FastQC warnings or differences.

### 11. Did any sample show a possible quality problem? What was it?

Yes. SRR23869379 showed a failure in Per Base Sequence Content for both R1 and R2, while R2 also had a warning for Per Sequence GC Content. However, its overall sequencing quality was good.

### 12. What additional steps would be needed before comparing gene expression?

The reads should undergo quality control and trimming if necessary, followed by transcript quantification or alignment, normalization, and statistical differential-expression analysis.

# Conclusion

This activity helped us understand how RNA-seq data are obtained and evaluated before gene-expression analysis. My assigned sample, SRR23869379, represented a faba bean leaf exposed to 200 mM NaCl for 48 hours. The sample had generally good sequencing quality, although FastQC identified some concerns involving per-base sequence content and GC content. Further analysis would require additional quality control, transcript assembly or alignment, expression quantification, normalization, and differential gene-expression analysis.

