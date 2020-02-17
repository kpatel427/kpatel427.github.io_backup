---
layout: other_pages
title: Bioinformatics Scientist
subtitle: Beginner | Curious | Learner
sitemap:
  priority: 0.9
---


## De novo transcriptome assembly and RNA-seq quantification of aberrant ATRX transcript
- performed *de novo* transcriptome assembly and quantification of aberrant ATRX transcripts (ATRX - gene responsible for chromatin remodelling and lack of function of these genes result in ALT pathway activation).
- performed gene abundance estimation of RNA-Seq data (i.e. quantification) for all samples in the analysis.
- Visualized assembled transcripts using GViz R Bioconductor package.  
**Tools/softwares : StringTie**  
**Languages: R, python**


## Identification of MYCN repressed targets and understanding their role in immune evasion
- Called broad (histone marks) and narrow (TF) peaks using HMCan and Macs2
- Annotated the peaks and performed enriched motif searching using Homer
- performed statistical tests (wilcox/independent t-test/correlations) to identify significant difference in expression and correlation with MYCN expression across high risk - low risk cohorts.  
**Statistical analysis: Wilcox, independent t-test**  
**Tools/softwares : MACS2, Homer, HMCan**  
**Algorithms: unsupervised clustering (hierarchical clustering), dimensionality reduction (PCA)**  
**Languages: R, bash**  


## Pediatric Cancer Web Portal
- Rshiny Web portal to visualize and analyze transcriptomic data from PDXs, cell line and patient data along with associated metadata (MYCN      Status, TP53 Status and ALK Status) for Neuroblastoma datasets.
- A few among visualization utilities include gene-gene correlations, top gene correlations, Kaplan-meier survival plots, visualization of copy number data and mutation data.
- Multi-dataset meta analysis across datasets to get correlation between two genes, correlation of genes across MYCN status and survival data.
- Allows user to visualize gene expression and correlations at various time points in mouse-human hybrid time-series data
- Fetched, formatted and normalized (RMA normalization using Affy R package) Neuroblastoma datasets from NCBI GEO (using GEOQuery R package)  
**Statistical analysis: correlations, ANOVA, t-test**  
**Tools/softwares : RShiny, R**  
**Languages: R**  


## Deconvulate Human and murine reads from RNASeq tumor data
- Using BBSplit tool (BBMAP tool) on RNASeq tumor reads
- Aligning reads to respective reference genome 
- Performing post-alignment quality control and report generation
- Calling gene abundance estimations  
**Tools/softwares : BBSplit(BBMap suite), STAR, Multi-QC**  
**Languages: R, bash**  


## Studying motif landscape for identified targets among high-risk Neuroblastoma patient expression data
- Calling enriched motifs among promoter peak regions of identified target genes.
- Performing unsupervised clustering methods to group and visualize target genes.
- Visualizing (oncoprints) motif occurrences in the peak regions of genes of interest.
- Visualizing CpG islands in IGV among the peak regions
- Fetching methylation data corresponding to the targets and visualizing methylation sites in IGV  
**Statistical analysis: Wilcox, independent t-test**  
**Tools/softwares : MACS2, Homer, HMCan, MEME suite (FIMO, MAST), ToppGene, Enrichr**  
**Algorithms: unsupervised clustering (hierarchical clustering), dimensionality reduction (PCA)**  
**Languages: R, bash**  


## Identifying Neuroblastoma specific proteins interacting with MYC (boxes) using CRISPR screen data 
- Looked at dependency scores for genes of interest using broad CCLE CRISPR screen data
- Narrowed down genes specific to Neuroblastoma lines with those having significant difference (using statistical methods) in dependency scores when compared to non-Neuroblastoma cell lines
- Visualized dependency score distributions between neuroblastoma and non-neuroblastoma cell lines.  
**Statistical analysis: Wilcox**  
**Algorithms: dimensionality reduction (PCA)**  
**Languages: R**  


## To determine bimodality of MYCN amplification in Neuroblastoma RNASeq data
- Used Whole Exome data to calculate MYCN depth vs exome depth
- Correlated MYCN expression with depth to see how well they correlate
- Overlayed mycn depth with mycn expression data across various cell lines to visualize if MYCN copy number align with MYCN expression levels  
**Tools/softwares : bedtools**  
**Languages: R, bash**  

