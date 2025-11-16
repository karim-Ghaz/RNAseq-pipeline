# RNAseq-pipeline
# RNA-seq Pipeline (Snakemake + Salmon + DESeq2)


Ce dépôt contient un pipeline RNA‑seq complet utilisant :
- Snakemake
- Salmon (quantification)
- FastQC / MultiQC
- DESeq2 (analyse différentielle)


## Installation
conda env create -f envs/fastqc.yaml
conda env create -f envs/salmon.yaml
conda env create -f envs/deseq2.yaml


## Lancer le pipeline
snakemake --cores 8 --use-conda --rerun-incomplete


## Organisation
- data/ → fichiers FASTQ
- results/ → résultats générés automatiquement
- config/ → configuration du projet
- scripts/ → scripts d’analyse
