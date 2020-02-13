---
layout: page
title: Bioinformatics Scientist
subtitle: Beginner | Curious | Learner
sitemap:
  priority: 0.9
---


1. De novo transcriptome assembly and RNA-seq quantification of aberrant ATRX transcript
- performed de novo transcriptome assembly and quantification of aberrant ATRX transcripts (ATRX - gene responsible for chromatin remodelling and lack of function of these genes result in ALT pathway activation) using StringTie.
- performed a gene abundance estimation of RNA-Seq data (i.e. quantification) for all samples in the analysis.
- assembled transcripts were then merged into a uniform set of transcripts using StringTie merge and a quantification of merged transcripts and genes in each sample was performed.
- Visualized assembled transcripts using GViz R Bioconductor package.
Tools/softwares : StringTie
Languages: R, python

2. Identifying MYCN-repressed genes in mycn-amplified pdx's
- performed differential expression analysis using DESEQ2 for mycn-amplified cell line and Target patient data
- called peaks using MACS2 and HMCan for mycn-amplified pdx's
- overlapped histone peaks with mycn-amp peaks
- Motif analysis and annotation of peaks was performed for overlapping peaks using homer
- visualized coverage of active and repressed genes in chipseq data of mycn-amp pdx's as heatmaps
- identified genes associated with motifs called with high confidence values in homer
- performed statistical tests (wilcox/independent t-test) to identify significant difference in expression across high risk - low risk and mycn amp - non-amp samples.
Statistical analysis: Wilcox, independent t-test
Tools/softwares : MACS2, Homer, HMCan, MEME suite (FIMO, MAST)
Algorithms: unsupervised clustering (hierarchical in heatmaps, PCA)
Languages: R, bash
	2a. Peak calling pipelines for chipseq data of Histone marks and TF sites
	- Called broad (histone marks) and narrow (TF) peaks using HMCan and Macs2
	- Annotated the peaks and performed motif searching using Homer
	- created a list of genes associated with the most significant motif hits
	- Generating heatmaps from ChIP-Seq data to visualize enhancers, super-enhancers and promoters called (using ROSE and LILY) around TSS

4. Pediatric Cancer Web Portal
- Rshiny Web app to visualize and analyze transcriptomic data from PDXs, cell line and patient data along with associated metadata (MYCN Status, TP53 Status and ALK Status)
- A few among visualization utilties are gene-gene correlations, top gene correlations, Kaplan-meier plots, visualization of copy number data and mutation data.
- Multi-dataset meta analysis across datasets to get correlation between two genes, correlation of genes across MYCN status and survival data.
- Allows user to visualize gene expression and correlations at various time points in mouse-human hybrid time-series data
- Fetched, formatted and normalized (RMA normalization using Affy R package) NBL datasets from NCBI GEO (GEOQuery R package)
Statistical analysis: correlations, ANOVA, t-test
Tools/softwares : RShiny, R
Languages: R

5. Deconvulate Human and murine reads from RNASeq tumor data
- Using BBSplit tool (BBMAP tool)
- Aligning reads to respective ref genome 
- Calling gene abundance estimations
Tools/softwares : BBSplit(BBMap suite), STAR
Languages: R, bash

6. Studying motif landscape for identified targets among high-risk patient expression data
- Calling enriched motifs (Homer) among promoter peak regions of identified target genes.
- Performing dimensionality reduction and clustering methods to see which of those targets group together.
- Visualizing motif occurrences in peak region of genes of interest by generating oncoprints.
- Visualizing CpG islands among the peak regions in IGV
- Fetching methylation data corresponding to the targets and visualizing methylation sites in IGV
Statistical analysis: Wilcox, independent t-test
Tools/softwares : MACS2, Homer, HMCan, MEME suite (FIMO, MAST), ToppGene, Enrichr
Algorithms: unsupervised clustering (hierarchical in heatmaps, PCA)
Languages: R, bash

7. Identifying NBL specific proteins interacting with MYC (boxes) using CRISPR data 
- Looked at dependency scores for genes of Interest using broad CCLE CRISPR screen data
- Narrowed down genes specific to NBL with those having significant difference (using statistical methods) in dependency scores across NBL and non-NBL lines
Statistical analysis: Wilcox
Algorithms: dimensionality reduction (PCA)
Languages: R

8. Applying regression methods to identify genes contributing to density/resistance of cellLines to certain drug (MM4)

9. To determine bimodality of amplification in RNASeq data
- Used Whole Exome data to calculate MYCN depth vs exome depth
- Correlated MYCN expr with depth to see how well they correlate
- Overlayed mycn depth with mycn expression data across various cell lines
Tools/softwares : bedtools
Languages: R, bash

