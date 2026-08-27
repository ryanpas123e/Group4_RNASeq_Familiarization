# Assignment 3 - RNA-Seq Familiarization

## Student Information

**Name:** Mark Ryan Pasculado

**Group:** Group 4 – Salinity Stress

## Group Paper

**Title:** *Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2*

**Authors:** Muhammad Afzal, Salem S. Alghamdi, Muhammad Altaf Khan, Sulieman A. Al-Faifi, and Muhammad Habib ur Rahman

**Year:** 2023

**Journal:** *Scientific Reports*, 13, 21223

## Assigned RNA-Seq Sample

- **Run accession:** SRR23869379
- **Condition:** Treatment – 48-hour salt stress
- **Biological replicate:** R1
- **Organism:** Faba bean (*Vicia faba* L.), genotype Hassawi-2
- **Tissue:** Leaves
- **Sequencing:** Paired-end
- **Number of reads:** 31,549,121
- **Read length:** 101 bp
- **GC content:** Approximately 43–44%

## Biological Representation

SRR23869379 represents a leaf RNA-seq sample from Hassawi-2 faba bean exposed to 200 mM NaCl for 48 hours. It represents one biological replicate used to examine gene-expression changes during salinity stress.

## FastQC Summary

The sample had generally good sequencing quality. Per-base sequence quality and adapter content passed for both reads. However, FastQC showed a failure in per-base sequence content, while the reverse read (R2) also showed a warning for per-sequence GC content. Overall, the sample was usable but had some QC observations that should be considered before downstream analysis.

## Main QC Observation

The sample had good overall sequencing quality, but FastQC identified some concerns in per-base sequence content and GC content, particularly in the reverse read.

## Conclusion

The analysis provided experience in examining raw RNA-seq data before downstream gene-expression analysis. SRR23869379 contained a large number of paired-end reads with an approximately 101 bp read length and 43–44% GC content. Although the sample had good overall quality, some FastQC warnings and failures were observed. Further quality control, trimming if necessary, and gene-expression analysis would be needed for downstream comparison.
