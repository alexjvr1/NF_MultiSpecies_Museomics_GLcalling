# NF_MultiSpecies_Museomics_GLcalling

A fully reproducible pipeline for extimating genotype likelihoods and genetic diversity from NGS data. 

The pipeline is designed for museomic studies with both modern and museum NGS data and can 
be run on multiple species simultaneously. It is particularly well suited to low coverage 
whole genome sequencing data from museum samples, where SNP calls can be unreliable. 

The pipeline is built in Nextflow, a workflow tool that is scalable and can be deployed on multiple
computing infrastructures. It is packaged with a Docker container that contains all the dependencies 
for easy installation and reproducibility. 

## Quickstart

1. Install Nextflow using this command: 

```
curl -s https://get.nextflow.io | bash 
```

Add the executable to your PATH

```
export PATH=$PATH:path/to/nextflow/download
```

If you're using Nextflow prior to v.22.03.0-edge, DSL2 must be [explicitly enabled](https://www.nextflow.io/docs/latest/dsl1.html) in the main.nf file

2. Download the Docker image (optional):

The Docker image contains all the required dependencies for the pipeline. 

```

```

3. Launch the pipeline:

```
nextflow run Velocity-NF -profile docker
```

## Pipeline Description

![alt_txt](https://github.com/alexjvr1/NF_MultiSpecies_Museomics_GLcalling/blob/main/docs/images/Velocity_Pipeline.png)

## Input files



## Pipeline parameters


--mus_run1, --mus_run2, --mus_run3

--mod_run1, --mod_run2, --mod_run3

Specifies the location of the FASTQ reads for multiple sequencing runs of the same individuals to be concatenated together. 

--mus_reads

--mod_reads

Specifies the location of the FASTQ

--mus_bam

--mod_bam


--genome


--invariant_sites


