# TapeStation Data

This directory contains exported TapeStation electropherograms used for validation of SNP-specific primers in the SELECT-seq study.

## Experimental design

For each target gene, SNP-specific primers were designed with a 3′ terminal nucleotide corresponding to each of the four possible bases (A, T, G, or C) at the SNP position.

Each TapeStation file contains PCR products generated using:

* No genomic DNA input (negative control)
* U-2 OS genomic DNA
* T-47D genomic DNA

combined with primers ending in:

* A
* T
* G
* C

resulting in a total of 12 lanes per target gene:

```text
Negative_A
Negative_T
Negative_G
Negative_C

U2OS_A
U2OS_T
U2OS_G
U2OS_C

T47D_A
T47D_T
T47D_G
T47D_C
```

## Interpretation

The expected target amplicon size for each gene is listed in Supplementary Table 1.

An internal ACTB (β-actin) control amplicon is present at approximately 105 bp and serves as a positive amplification control.

Specific amplification of the target locus is indicated by the presence of a peak at the expected target amplicon size. Primer specificity can be assessed by comparing amplification across the four allele-specific primer designs and between U-2 OS and T-47D genomic DNA samples.

## Sample preparation

PCR was performed as described in the Methods section of the manuscript.

For TapeStation analysis:

* 1 μL of PCR product was loaded directly onto the TapeStation system.
* PCR products were analysed without prior purification.

## Relationship to Figure 1D

The quantitative analysis shown in Figure 1D was derived from TapeStation measurements. For each reaction, only peaks corresponding to the expected target amplicon size were considered. The concentration of the target-gene amplicon was normalized to the concentration of the ACTB control amplicon (approximately 105 bp). Reactions in which no peak was detected at the expected target amplicon size were assigned a value of zero. The resulting target/ACTB ratios were used for downstream comparisons.
