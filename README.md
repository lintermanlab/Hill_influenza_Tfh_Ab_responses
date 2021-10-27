# Hill_influenza_Tfh_Ab_responses

Supporting Hill et al. "Impaired HA-specific T follicular helper cell and antibody responses to influenza vaccination are linked to inflammation in humans"
Elife (2021).

This repository contains immune parameter data and processed RNA sequencing data behind various figures in the paper.

The relevant data is supplied in the folder `/data`.


See manuscript for description of methods and contact Dr Danika Hill for further information (Danika.hill@monash.edu). 

## Description of files

All are R data files.

### Cohort1_RNAseq.RData
Contains 2 data objects:
1)	`ALFNA14.vsd` a DESeq2 S4 dataset containing gene expression data after normalisation using the `RUVseq` package and variance stabilizing transformation using `DESeq2`.
2)	`ALFNA14.DESeq` contains differential gene expression results for the various comparisons (timepoint, age group etc). 

### Cohort2_RNAseq.RData
Contains 2 data objects:
1)	`ALFNA16.vsd` a DESeq2 S4 dataset containing gene expression data after normalisation using the `RUVseq` package and variance stabilizing transformation using `DESeq2`.
2)	`ALFNA16.DESeq` contains differential gene expression results for the various comparisons (timepoint, age group etc). 

### Cohort1_immune_vars.RData
Contains 2 data objects:
1)	`ALFNA14.vars` is a dataframe containing data for each variable included in the paper for each time point for 32 participants (both age groups). 
2)	`Cali09.14.D42` is a vector of the normalised antibody titre at d42 used for correlation analysis. 

### Cohort2_immune_vars.RData
Contains 3 data objects:
1)	`ALFNA16.vars` is a dataframe containing data for each variable included in the paper for each time point for 42 participants (both age groups).
2)	`Cali09.16.D42` is a vector  of the normalised antibody titre at d42 used for correlation analysis. 


### Bioconductor packages

- `RUVSeq` https://bioconductor.org/packages/RUVSeq/
- `DESeq2` https://bioconductor.org/packages/DESeq2/


