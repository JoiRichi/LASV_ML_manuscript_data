# LASV_ML_Manuscript_Data

## Overview
This repository contains the data and code supporting the LASV manuscript. It is one of three repositories associated with the project. For complete project details, see the links below:

## Project Repositories
- **Data and Processing:** [LASV_ML_Manuscript_Data](https://github.com/JoiRichi/LASV_ML_manuscript_data)
- **Lassa Virus Phylogenetics:** [LASV_Phylogenetics_Pipeline](https://github.com/JoiRichi/LASV_phylogenetics_pipeline)
- **Lassa Virus Lineage Prediction:** [LASV_Lineage_Prediction](https://github.com/JoiRichi/LASV_lineage_pred)

## Jupyter Notebooks on Google Colab
- **General Preprocessing:** [Notebook Link](https://colab.research.google.com/drive/1JOgS2-dDoQ7OPHPcXm3AIBDnGQAFxIyR)
- **Motif Search Using RF MD Pcorr:** [Notebook Link](https://colab.research.google.com/drive/1M1yYB65MOWUpMYcn24Jfm6jvZZ13QJ6l)
- **Lassa Virus Lineage Prediction Training:** [Notebook Link](https://colab.research.google.com/drive/1G0lEjuvPR07bcb181Rfhm-S0WenMFSmR)

## Repository Structure
This repository stores all data and intermediates related to the project.

### Directories and Contents

- **raw_ncbi**: Contains nucleotide sequences and accompanying metadata of Lassa virus  available on NCBI Virus until 01/12/2023.
  
- **last_mafft_alignment**: Contains the aligned extracted GPC sequences using LAST and MAFFT, available [here](https://mafft.cbrc.jp/alignment/server/specificregion-last.html). [Reference gene](https://github.com/JoiRichi/LASV_phylogenetics_pipeline/blob/main/config/gly_ref_LASV.gb). The alignment file and raw metadata file (stored in raw_ncbi) serve as inputs for the [General Preprocessing](https://colab.research.google.com/drive/1JOgS2-dDoQ7OPHPcXm3AIBDnGQAFxIyR) notebook.
  
- **alignment_preprocessing**: Contains outputs from the [General Preprocessing](https://colab.research.google.com/drive/1JOgS2-dDoQ7OPHPcXm3AIBDnGQAFxIyR) notebook. The alignment from MAFFT was filtered to produce passed files, which were manually curated and translated to amino acids using Aliview. These files are inputs for the [Lassa Virus Phylogenetics](https://github.com/JoiRichi/LASV_phylogenetics_pipeline) pipeline, [Motif Search Using RF MD Pcorr](https://colab.research.google.com/drive/1M1yYB65MOWUpMYcn24Jfm6jvZZ13QJ6l), and [Lassa Virus Lineage Prediction Training](https://colab.research.google.com/drive/1G0lEjuvPR07bcb181Rfhm-S0WenMFSmR) notebooks.
  
- **result_motiff_search**: Contains results from the [Motif Search Using RF MD Pcorr](https://colab.research.google.com/drive/1M1yYB65MOWUpMYcn24Jfm6jvZZ13QJ6l) notebook.
  
- **lineage_annotation**: Contains sequence IDs grouped into lineages based on annotated clades from the [Lassa Virus Phylogenetics](https://github.com/JoiRichi/LASV_phylogenetics_pipeline) analysis. These files contain target variables for the [Lassa Virus Lineage Prediction Training](https://colab.research.google.com/drive/1G0lEjuvPR07bcb181Rfhm-S0WenMFSmR) notebook.

For further details, please refer to the respective notebooks and repositories linked above.
