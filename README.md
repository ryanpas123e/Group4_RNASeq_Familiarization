# Group4_RNASeq_Familiarization
# Members
  - Batigulao, Jehiah Bless
  - Obiñeta, Inah Marie A.
  - Oficiar, Francis Kyle
  - Pasculado, Mark Ryan
  - Suan, Jade Angela

# 1. Title and Citation of the Group Paper
# Title: 
Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in faba bean genotype, Hassawi-2
# Citation: 
Afzal, M., Alghamdi, S.S., Khan, M.A., Al-Faifi, S.A., & Habib ur Rahman, M. (2023). Transcriptomic analysis reveals candidate genes associated with salinity stress tolerance during the early vegetative stage in fababean genotype, Hassawi-2. Scientific Reports, 13, 21223.  https://doi.org/10.1038/s41598-023-48118-0
# Article link: 
- DOI Link: https://doi.org/10.1038/s41598-023-48118-0
- PMC Link: https://pmc.ncbi.nlm.nih.gov/articles/PMC10692206/
# Study Accession / BioProject Number
- BioProject: PRJNA943415
- Repository: NCBI SRA
- NCBI SRA Link: https://www.ncbi.nlm.nih.gov/sra/?term=PRJNA943415

# Assigned RNA-Seq Runs to Group Members
  - Obiñeta — SRX19681425 (SRR23869388) — Control Replicate 1 — 0h salt stress — Paired End
  - Suan — SRX19681440 (SRR23869373) — Treatment Replicate 1 — 6h salt stress — Paired End
  - Batigulao — SRX19681430 (SRR23869383) — Treatment Replicate 1 — 24h salt stress — Paired End
  - Pasculado — SRX19681434 (SRR23869379 ) — Treatment Replicate 1 — 48h salt stress — Paired End
  - Oficiar — — Treatment Replicate 1 — 72h salt stress — Paired End

# Short Summary of the Experimental Design 
The study examined the transcriptomic response of faba bean (*Vicia faba L.*), salt-tolerant genotype "Hassawi-2," to salinity stress at the early vegetative (three-leaf) stage. Seedlings were treated with 200 mM NaCl, and leaf tissue was sampled at five time points after treatment (6h, 12h, 24h, 48h, and 72h), alongside untreated control seedlings. Each condition included 3 biological replicates. RNA was extracted from leaf tissue and sequenced using Illumina paired-end RNA-seq. Since no faba bean reference genome was used by the authors, transcripts were assembled de novo using Trinity, annotated against public databases (NR, Swiss-Prot, KEGG, GO, Pfam), and differential expression between control and each stress time point was assessed using edgeR, with results validated by qRT-PCR.


