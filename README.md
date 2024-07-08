# sceQTL_leukemia
This repository contains the R and shell scripts used for the analysis "Single-cell expression quantitative trait loci mapping identifies cell type-specific genetic regulation of patients with leukemia in lymph nodes".

Publication DOI: TBD

Contact: Shifang Li, Immunology-Vaccinology, FARAH, ULg. email: fruceslee@gmail.com

All the statistical analyses were performed by in-house R/Python script or published tools/packages.

**1.1 Single-cell RNA-seq analysis, cell type identification, and cell status identification**

Single-cell analysis by Seurat; cell status identification by RNA velocity.

**1.2 Identification of single-cell expression quantitative traits loci (sceQTL)**

The eQTL of each cell type or diseases were estimated using a linear model which is implemented in tensorqtl. The single-cell co-expression QTL was identified using a weighted linear model. 

**1.3 Estimation of shared signals**

We used MASH (MASHR) to estimate the shared eQTL signals between each pair of eQTL summary statistics. 

**1.4 Summary-based Mendelian randomization (SMR) and TWAS analysis**

This mediation effect of gene expression on the disease was estimated using SMR & HEIDI and TWAS methods.

**1.5 Colocalization analysis**

COLOC was applied to identify the colocalized genes between sceQTL and GWAS loci in Asia populations. The COLOC hypothesis shared common genetic causal variants in the given region by the genetic colocalization analysis of two potentially related phenotypes. 

**1.6 Single-cell Co-expression analysis**

To determine the co-expression profiles we used CS-CORE, which is powered by WGCNA.

**1.7 Replication of the identified sc-eQTL**

To validate the identified eQTL, we checked their effect size in the publicly available dataset GTEx. 

**1.8 Overlapping with epigenetics modifications**

The publicly available dataset scATAC-seq was employed. 
