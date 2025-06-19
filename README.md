# Exploring the Global Landscape of Rare Causal and Common High-Risk Variants in Parkinson’s Disease

<div align="center">
    <a href="https://gp2.org/">
    <img src="https://www.michaeljfox.org/sites/default/files/styles/grant_image_opportunity_detail/public/grant/GP2%20Logo.png?itok=OhZkYS-H" alt="GP2 Logo" width="200">
</a>
</div>


`GP2 ❤️ Open Science 😍`

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15699539.svg)](https://doi.org/10.5281/zenodo.15699539)    [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


**Last Updated:** June 2025

## Summary
This repository contains the code and workflow used in the study:
**“Exploring the Global Landscape of Rare Causal and Common High-Risk Variants in Parkinson’s Disease”.**

In this analysis, we screened sequencing (GP2 Release 8) and genotyping (GP2 Release 9) data from 69,881 individuals, including 41,139 clinically affected individuals (PD and other neurodegenerative phenotypes) and 28,742 unaffected individuals (controls, population cohorts, and healthy family members).

The notebooks provided here demonstrate how we extracted variant carriers and metadata, performed initial annotation across multiple ancestries using plink, bcftools, and annovar.

## Data Statement
* The data was obtained from the Global Parkinson’s Genetics Program (GP2) release 8 (GP2 release 8, DOI: [10.5281/zenodo.13755496](https://doi.org/10.5281/zenodo.13755496); GP2 release 9, DOI: [10.5281/zenodo.14510099](https://doi.org/10.5281/zenodo.14510099)) and access can be requested through the Accelerating Medicines Partnership in Parkinson’s Disease (AMP-PD) via the online application process (https://www.amp-pd.org/).

## Citation
If you use this repository or find it helpful for your research, please cite the corresponding manuscript:

>**Exploring the Global Landscape of Rare Causal and Common High-Risk Variants in Parkinson’s Disease**
>Lange LM, Fang ZH, Makarious MB, Kuznetsov N, et al.,
>Global Parkinson’s Genetics Program (GP2), 2025
[*DOI: pending publication*]

## Figures and Supplementary Figures
*(pending publication)*

## Tables and Supplementary Tables
*(pending publication)*

### Helpful Links 
- [GP2 Website](https://gp2.org/)
    - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
    - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation
The `analyses/` directory includes all the analyses discussed in the manuscript or links to the respective GitHubs where analyses were followed.
```
THIS REPO
├── LICENSE
├── README.md
├── analyses/
|   ├── 00_GP2_metadata.ipynb
|   ├── 01_GP2_WGS_R8_variant_extraction_and_annotation.ipynb
│   └── 02_GP2_NBA_R9_variant_extraction_and_annotation.ipynb
├── figures/
└── tables/
```

## Analyses

- Languages: Python, bash

| **Notebook**                   | **Description**                                                                                                                                                         |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 00_GP2_metadata.ipynb | Extract metadata for identified carriers (from GP2 NBA, CES and WGS) |
| 01_GP2_WGS_R8_variant_extraction_and_annotation.ipynb | Extract variant carriers and perform annotation using GP2 WGS and CES data (PLINK files from Release 8) |
| 02_GP2_NBA_R9_variant_extraction_and_annotation.ipynb | Extract variant carriers and perform annotation using GP2 NBA data (PLINK files from Release 9) |


## Software

| **Software** | **Version(s)** | **Resource URL** | **RRID** | **Notes** |
|--------------|----------------|------------------|----------|-----------|
| Python | 3.8+ | [http://www.python.org/](http://www.python.org/) | RRID:SCR_008394 | Used for downstream analysis and scripting. |
| PLINK | 1.9 / 2.0 | [http://www.cog-genomics.org/plink/](http://www.cog-genomics.org/plink/) | RRID:SCR_001757 | Used for variant filtering and extraction. |
| BCFtools | 1.17+ | [http://www.htslib.org/](http://www.htslib.org/) | RRID:SCR_005227 | Used for variant extraction. |
| ANNOVAR | Latest | [https://annovar.openbioinformatics.org/en/latest/](https://annovar.openbioinformatics.org/en/latest/) | RRID:SCR_012821 | Used for variant annotation. |

## Disclaimer
This notebook accompanies the manuscript **"Exploring the Global Landscape of Rare Causal and Common High-Risk Variants in Parkinson’s Disease"** and is intended to facilitate transparency and reproducibility of the variant extraction and annotation workflow.
