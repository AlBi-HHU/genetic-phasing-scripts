# genetic-phasing-scripts
Collections of scripts for data generation and evaluation for Recomb 2022 submission: "Genetic Polyploid Phasing using Marker Signals from low-depth Progeny Samples"

# Recreating ground truth region

Requires:
1. .gfa file containing the HiFi assemblies (ncbi)
2. Solyntus reference genome (public)
3. regions of parental VCF files (zenodo)

Run the snakemake pipeline `Snakefile-ASM` three times setting the chromosome variable to `3`, `4` and `5` respectively.

# Recreating the phasing results

Requires:
1. regions of parental VCF files (zenodo)
2. regions of progeny VCF files (zenodo)
3. ped file, specifying the pedigree relationships (zenodo)

Run the snakemake pipeline `Snakefile-Phase` 

# Recreating the whole-chromosome results

Requires:
1. parental VCF files (ncbi)
2. progeny VCF files (ncbi)
3. ped file, specifying the pedigree relationships (zenodo)

Run the snakemake pipeline `Snakefile-Whole`.

# Data availability

All files marked with either `(zenodo)`, `(public)` or `(ncbi)`, depending on whether the required data was uploaded on zenodo, is publicly available or available via an NCBI project. Please refer to the paper for further details. The NCBI data might be only available at a later point in time.

Link to Zenodo data: https://zenodo.org/record/5645743
Link to parental sequencing data: https://www.ncbi.nlm.nih.gov/bioproject/PRJNA718240/
Link to progeny sequencing data: https://www.ncbi.nlm.nih.gov/bioproject/PRJEB48582/
Link to hifi read data for Altus: https://www.ncbi.nlm.nih.gov/sra/SUB10617521
