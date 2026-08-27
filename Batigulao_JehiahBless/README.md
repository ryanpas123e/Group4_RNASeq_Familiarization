Assignment 3 — RNA-Seq Literature Familiarization and Data Characterization (Group 4: Salinity Stress)

Title:
Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in faba bean genotype, Hassawi-2

Citation: 
Afzal, M., Alghamdi, S. S., Khan, M. A., Al-Faifi, S. A., & Rahman, M. H. U. (2023). Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2. Scientific Reports, 13(1), 21223. https://doi.org/10.1038/s41598-023-48118-0

Study Organism:
The organism used in the study was the salt-tolerant faba bean genotype Hassawi-2 (_Vicia faba L_.).

Tissue:
Leaf tissue from plants at the three-leaf early vegetative stage was used for RNA extraction and RNA sequencing.

Biological Question:
The study investigated how the transcriptome of faba bean changes in response to different durations of salt stress. Specifically, the authors aimed to identify genes and molecular mechanisms associated with salt-stress tolerance at 6, 12, 24, 48, and 72 hours of exposure.

Assigned RNA-Seq Dataset

RNA-seq Run Accession:SRR23869383  
Experiment Accession:SRX19681430  
Link: https://www.ncbi.nlm.nih.gov/sra/SRX19681430[accn]
Condition:Treatment – 24-hour salt stress  
Treatment: 200 mM NaCl  
Tissue:Leaf tissue  
Paired-end sequencing

Number of reads / sequences
Treatment_24hrs_Rep1_R1: 31,558,920
Treatment_24hrs_Rep1_R2: 31,558,920
Read length
Treatment_24hrs_Rep1_R1: 101 bp
Treatment_24hrs_Rep1_R2: 101 bp
GC Content
Treatment_24hrs_Rep1_R1: 45%
Treatment_24hrs_Rep1_R2: 46%

FASTQ File Examination
The FASTQ file contains four lines for each sequencing read:
1. Sequence identifier
2. Nucleotide sequence
3. Separator line
4. Quality-score characters

FASTQ vs FASTA
A FASTA genome file contains sequence information, while a FASTQ file contains both the nucleotide sequence and sequencing quality information. FASTQ quality scores allow researchers to identify reads or bases that may have lower sequencing confidence and therefore help evaluate raw sequencing data quality.

FastQC Results
FastQC was performed on both R1 and R2 because the dataset is paired-end.

R1 FastQC
Basic Statistics
- Total sequences: 31,558,920
- Total bases: 3.1 Gbp
- Sequences flagged as poor quality: 0
- Sequence length: 101 bp
- GC content: 45%

FastQC Results
- Per-base sequence quality: PASS
- Per-sequence quality scores: PASS
- Per-base sequence content: FAIL
- Per-sequence GC content: PASS
- Per-base N content: PASS
- Sequence length distribution: PASS
- Sequence duplication levels: FAIL
- Overrepresented sequences: PASS
- Adapter content: PASS

R1 Interpretation
R1 showed generally good sequencing quality based on the per-base sequence quality and per-sequence quality results. However, FastQC reported failures for per-base sequence content and sequence duplication levels. The per-base sequence content failure indicates nucleotide composition bias, particularly toward the beginning of the reads. The sequence duplication failure indicates that a considerable proportion of sequences were duplicated.

R2 FastQC
Basic Statistics
- Total sequences: 31,558,920
- Total bases: 3.1 Gbp
- Sequences flagged as poor quality: 0
- Sequence length: 101 bp
- GC content: 46%

FastQC Results
- Per-base sequence quality: PASS
- Per-sequence quality scores: PASS
- Per-base sequence content: WARN
- Per-sequence GC content: WARN
- Per-base N content: PASS
- Sequence length distribution: PASS
- Sequence duplication levels: FAIL
- Overrepresented sequences: WARN
- Adapter content: PASS

R2 Interpretation
R2 also showed good per-base sequence quality, with all bases having high quality scores. However, FastQC reported warnings for per-base sequence content and per-sequence GC content. R2 also failed the sequence duplication level module. An overrepresented poly-G sequence was detected, occurring in approximately 0.48% of reads, and FastQC reported no identified source for this sequence. Adapter content still received a PASS result.

FastQC Summary
Overall, the RNA-seq dataset showed good base-level sequencing quality, as both R1 and R2 passed the per-base sequence quality module and no sequences were flagged as poor quality. Both R1 and R2 also passed the adapter-content module. However, some quality concerns were observed, particularly high sequence duplication and nucleotide-composition bias. R2 additionally showed warnings for per-sequence GC content and an overrepresented poly-G sequence. The FastQC results therefore indicate that the dataset has generally good sequencing quality but contains some characteristics that should be considered during later RNA-seq preprocessing and analysis.

Interpretation Questions
1. What biological question was the original RNA-seq study trying to answer?
The study aimed to determine how gene expression and the transcriptome of the salt-tolerant faba bean genotype Hassawi-2 change during different periods of salt stress. The authors examined responses at 6, 12, 24, 48, and 72 hours after exposure to 200 mM NaCl to identify genes and molecular mechanisms associated with salt-stress tolerance.

2. Why did the authors use RNA-seq instead of only examining the genome?
RNA-seq was used because the researchers wanted to examine the RNA molecules being expressed under salt stress. A genome mainly provides information about the organism's DNA, while RNA-seq provides information about which genes are actively expressed and how their expression changes under different conditions.

3. What is the difference between genomic DNA and the RNA molecules measured by RNA-seq?
Genomic DNA contains the organism's complete genetic information and is relatively stable. RNA molecules represent transcripts produced from genes and can change depending on the cell's condition, developmental stage, or environmental stress. RNA-seq therefore provides information about the transcriptome rather than simply the DNA sequence.

4. What is a biological replicate and why is it important?
A biological replicate is an independent biological sample from the same experimental condition. Biological replicates are important because they allow researchers to measure natural biological variation and determine whether observed differences are consistent rather than caused by variation in only one sample.

5. What is the difference between single-end and paired-end sequencing?
In single-end sequencing, each DNA fragment is sequenced from only one end. In paired-end sequencing, both ends of the same fragment are sequenced, producing two reads, commonly called R1 and R2. Paired-end sequencing can provide additional information about the location and structure of transcripts.

6. What is a FASTQ file?
A FASTQ file is a sequencing-data file format that contains the sequence identifier, nucleotide sequence, separator line, and quality-score characters for each read. It therefore contains both sequence information and the quality information associated with the sequencing bases.

7. What information does FastQC provide?
FastQC provides a quality assessment of raw sequencing data. It can report read number, read length, GC content, per-base sequence quality, nucleotide composition, N content, sequence duplication, overrepresented sequences, and adapter content.

8. What does a high per-base quality score indicate?
A high per-base quality score indicates that the sequencing base calls have high confidence and are less likely to contain sequencing errors. In this dataset, both R1 and R2 passed the per-base sequence quality assessment.

9. Why can adapter contamination be a problem?
Adapter sequences are artificial sequences introduced during library preparation. If they remain in sequencing reads, they can interfere with downstream analysis, including read alignment and transcript quantification. Adapter contamination can therefore reduce the reliability of subsequent RNA-seq analyses.

10. Were all RNA-seq samples in your group similar in quality? Explain.
The samples were generally expected to have similar overall sequencing quality because they came from the same RNA-seq study and sequencing experiment. However, the FastQC results should be compared among all group members to determine whether there are noticeable differences. For my assigned sample, R1 and R2 both had high per-base quality, but they differed in some QC warnings, particularly sequence composition and overrepresented sequences.

11. Did any sample show a possible quality problem? What was it?
Yes. My assigned sample showed several possible quality concerns. R1 failed the per-base sequence content and sequence duplication modules. R2 showed warnings for per-base sequence content, per-sequence GC content, and overrepresented sequences, and it also failed the sequence duplication module. R2 contained an overrepresented poly-G sequence representing approximately 0.48% of the reads.

12. What additional steps would be needed before the researchers could compare gene expression between control and treatment samples?
Before comparing gene expression, the sequencing reads would normally undergo quality control and preprocessing, including assessment and possible removal of low-quality bases and adapter sequences. The reads would then need to be processed for transcriptome assembly or alignment, followed by transcript/gene quantification. The resulting expression data would need appropriate normalization and statistical analysis before differential expression between control and treatment samples could be determined.

Conclusion
This activity provided an introduction to RNA-seq data and the characterization of raw sequencing reads using Galaxy and FastQC. The assigned dataset, SRR23869383, contained paired-end 101-bp reads with generally high per-base sequencing quality. However, FastQC identified sequence duplication and nucleotide-composition issues, as well as an overrepresented poly-G sequence in R2. These results show why raw RNA-seq data should be examined carefully before proceeding to downstream transcriptome and gene-expression analyses.









