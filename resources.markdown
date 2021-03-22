---
layout: page
title: Resources
permalink: /Resources/
---

This page summarises some resources, which might be useful to others. Most of them are hosted on my [GitHub](https://github.com/boasvdp).

### Snakemake pipelines

For most projects, I try to make the code reproducible using a combination of [Conda](https://docs.conda.io/en/latest/) and [Snakemake](https://snakemake.readthedocs.io/en/stable/). From the Snakemake readthedocs:

> The Snakemake workflow management system is a tool to create reproducible and scalable data analyses. Workflows are described via a human readable, Python based language.

Integrating Conda with Snakemake ensures that the software can be easily installed, and the right version are available to reproduce the results. Several of the pipelines available are:

- SNP typing for longitudinal *E. coli* samples

This Snakemake pipeline performs a read mapping analysis to determine whether strains have persisted in participants, which were sampled longitudinally. The read mapping analysis first groups strains by sequence type, then finds the best reference genome available for that sequence type and finally maps the reads on the reference genome to obtain a measure of differences. In addition, several typing analyses have been included.

[GitHub link](https://github.com/boasvdp/COMBAT)

https://zenodo.org/badge/DOI/10.5281/zenodo.4582689.svg

- Genomic epidemiology of zoonotic *Streptococcus suis*

We performed a survey of several European reference laboratories to obtain zoonotic *S. suis* cases. These were Illumina sequenced and put into context of a global collection of *S. suis* isolates.

[GitHub link](https://github.com/boasvdp/Ssuis_genomic_epidemiology)

- Hybrid assembly

The pipeline used for our MRA publication on *Streptococcus suis* collects long-read (ONT) and short-read (Illumina) data, performs hybrid assembly and performs some basic typing of the assemblies. Several QC steps have been implemented as well. 

[GitHub link](https://github.com/boasvdp/MRA_Streptococcus_suis)

- Outbreak analysis

For a benchmarking exercise for the Special Interest Group Bioinformaticians in Medical Microbiology Netherlands, I created a general workflow to analyse data from hospital outbreaks of (resistant) bacteria.

[GitHub link](https://github.com/boasvdp/benchmark_SIGNL)
