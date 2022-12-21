# Typhoid Genomics Consortium Paper: Global distribution of genotypes and AMR (2022)

This repo holds the tabulated data and code behind the first paper of the [Typhoid Genomics Consortium](https://typhoidgenomics.org/).

Raw data are publicly available under the accessions given in file `TGC_data.csv` in this repository, and the genome assemblies used in this analysis are available in FigShare under doi: [10.26180/21431883](https://doi.org/10.26180/21431883). Assemblies of suitable quality (n=12,849; those with identifiers PW_id and PW_displayname in file `TGC_data.csv`) are included in the online platform Pathogenwatch (https://pathogen.watch/organisms/styphi), where they can be interactively explored and included in user-driven comparative analyses.

## Main data file 

`TGC_data.csv`

* line list of all genomes including data accessions, source information, plus genome-derived genotype and AMR variables

* see metadata template [bit.ly/typhiMeta](bit.ly/typhiMeta) for details of source data coding

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

