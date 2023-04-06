# Typhoid Genomics Consortium Paper: Global distribution of genotypes and AMR (2022)

This repository holds the tabulated data and code behind the first paper of the [Typhoid Genomics Consortium](https://typhoidgenomics.org/), "Global diversity and antimicrobial resistance of typhoid fever pathogens: insights from 13,000 Salmonella Typhi genomes" (Carey et al, 2022).

## Licenses and and re-use:

* The code in this repository is shared under a GNU general public license v3.0.

* The data, figures and tables in this repository form part of the publication noted above, which is published under a Creative Commons 4.0 License. If you use material in this repository, you should cite both the paper and this repository as the source. **This work represents the culmination of 20 years of typhoid genomics, with over 150 authors. It is here for the benefit of all, but please respect and acknowledge the effort of the authors when you come to re-use the data and ensure you cite appropriately.**

* Raw genome data (fastq readsets) are publicly available under the accessions given in file `TGC_data.csv` in this repository. The genome assemblies used in this analysis are available in FigShare under doi: [10.26180/21431883](https://doi.org/10.26180/21431883). Assemblies of suitable quality (n=12,849; those with identifiers PW_id and PW_displayname in file `TGC_data.csv`) are also included in the online platform Pathogenwatch (https://pathogen.watch/organisms/styphi), where they can be interactively explored and included in user-driven comparative analyses. 

* PubMed identifiers (indicating the original source paper) are given for individual genomes in the file `TGC_data.csv` in this repository. **If you use this data in a manner that focuses on particular subsets of genomes (e.g. those from a particular country or substudy), we ask that you please use this to identify and cite the relevant source papers in addition to citing the consortium paper** - this ensures data contributors are maximally credited for their work, and are more likely to be able to continue to generate and share Typhi sequences for research and public health benefit.

## Main data file 

`TGC_data.csv`

* line list of all genomes including data accessions, source information, plus genome-derived genotype and AMR variables

* see metadata template [bit.ly/typhiMeta](https://bit.ly/typhiMeta) for details of source data coding

* countries were assigned to geographical regions according to the [United Nations Statistics Division standard M49] (https://unstats.un.org/unsd/methodology/m49/overview/), using 'intermediate region' label where assigned and 'subregion' otherwise 

* genotype and AMR columns are derived using the [Mykrobe implementation](https://github.com/katholt/genotyphi) of the [GenoTyphi](https://doi.org/10.1093/infdis/jiab414) scheme, and [Typhi Pathogenwatch](https://doi.org/10.1038/s41467-021-23091-2)

`UN_region_coords.csv` 

* GPS coordinates for world regions, used to generate world map of genotypes


## Genotype analysis

`/genotypes` directory

* `genotypes.Rmd` = R markdown file for all analysis, generating tables and figures

* `genotypes.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format; output from executing Rmd file)

* supplementary table files (CSV format; output from executing Rmd file)

## AMR analysis

`/AMR` directory

* `AMR_summary.Rmd` = R markdown file for all analysis, generating tables and figures

* `AMR_summary.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format; output from executing Rmd file)

* supplementary table files (CSV format; output from executing Rmd file)

## Plotting phylogenetic trees

`/trees` directory

* `trees.Rmd` = R markdown file for all analysis, generating tables and figures

* `trees.html` = knitR output of Rmd file, including output figures

* tree files (`.nwk` format) = neighbour-joining core genome trees downloaded from Pathogenwatch

* `pw232_to_ID.csv` = file mapping tip names in 2.3.2 tree file to identifiers in the main consortium metadata file

* figure files (PNG and PDF format; output from executing Rmd file)

