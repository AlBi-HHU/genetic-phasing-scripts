# genetic-phasing-scripts
Collections of scripts for data generation and evaluation for Recomb 2022 submission: "Genetic Polyploid Phasing using Marker Signals from low-depth Progeny Samples"

# Recreating ground truth region

Requires:
1. .gfa file containing the HiFi assemblies
2. Solyntus reference genome
3. parental VCF files

Run the snakemake pipeline `Snakefile-ASM` three times setting the chromosome variable to `3`, `4` and `5` respectively.

# Recreating the phasing results

Requires:
1. parental VCF files
2. progeny VCF files
3. ped file, specifying the pedigree relationships

Run the snakemake pipeline `Snakefile-Phase` 

# Recreating the whole-chromosome results

Requires:
1. parental VCF files
2. progeny VCF files
3. ped file, specifying the pedigree relationships

Run the snakemake pipeline `Snakefile-Whole`.

# Data availability

All files marked with either `[zenodo]`, `[public]` or `[ncbi]`, depending on whether the required data was uploaded on zenodo, is publicly available or available via an NCBI project. Please refer to the paper for further details. The NCBI data might be only available at a later point in time.