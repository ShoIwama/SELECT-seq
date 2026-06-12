# SELECT-seq

Pre-Sequencing Enrichment of SNP Edits in One-Pot Single-Cell Whole Transcriptome Sequencing

## Overview

This repository contains source data and analysis scripts associated with the SELECT-seq manuscript. SELECT-seq combines SNP-specific amplification during whole-transcriptome amplification with Cas12a-based fluorescence detection, enabling pre-sequencing identification and enrichment of single cells carrying specific nucleotide variants.

### `data/`

Contains processed data tables used for figure generation and downstream analyses, including fluorescence measurements, count matrices or summary data, and source data used in the manuscript figures.

### `scripts/`

Contains notebooks and scripts used to generate figures and perform analyses described in the manuscript, including:

* SNP-specific amplification analysis
* Cas12a fluorescence analysis
* SELECT-seq and Smart-seq3 benchmarking
* NRF2 T80K concordance analysis
* Figure and supplementary figure generation

### `tapestation/`

Contains exported TapeStation electropherograms used for validation of SNP-specific primers. Each PDF corresponds to one target gene and contains negative control, U-2 OS genomic DNA, and T-47D genomic DNA reactions tested with primers ending in A, T, G, or C.

The expected target amplicon size for each gene is provided in Supplementary Table 1. The ACTB internal control amplicon is approximately 105 bp. For Figure 1D, only peaks corresponding to the expected target amplicon size were used for quantification.

## Data notes

Large raw sequencing files are not included in this repository. Processed data required to reproduce the manuscript figures are provided in the `data/` directory. Raw sequencing data availability is described in the manuscript.
