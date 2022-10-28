# Typhoid Genomics Consortium Paper: Global distribution of genotypes and AMR (2022)

This repo holds the data and code behind the first paper of the [Typhoid Genomics Consortium](https://typhoidgenomics.org/).

## Main data file 

`TGC_data_271022.csv`

* line list of all genomes including data accessions, source information, plus genome-derived genotype and AMR variables

* see metadata template [bit.ly/typhiMeta](bit.ly/typhiMeta) for details of source data coding

* genotype and AMR columns are derived using the [Mykrobe implementation](https://github.com/katholt/genotyphi) of the [GenoTyphi](https://doi.org/10.1093/infdis/jiab414) scheme, and [Typhi Pathogenwatch](https://doi.org/10.1038/s41467-021-23091-2)

`UN_region_coords.csv` 

* GPS coordinates for world regions, used to generate world map of genotypes

## Genotype analysis

`/genotypes` directory

* `genotypes_281022.Rmd` = R markdown file for all analysis, generating tables and figures

* `genotypes_281022.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format; output from executing Rmd file)

* supplementary table files (CSV format; output from executing Rmd file)

## AMR analysis

`/AMR` directory

* `AMR_summary_281022.Rmd` = R markdown file for all analysis, generating tables and figures

* `AMR_summary_281022.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format; output from executing Rmd file)

* supplementary table files (CSV format; output from executing Rmd file)

## Plotting phylogenetic trees

`/trees` directory

* `trees.Rmd` = R markdown file for all analysis, generating tables and figures

* `trees.html` = knitR output of Rmd file, including output figures

* tree files (`.nwk` format) = neighbour-joining core genome trees downloaded from Pathogenwatch

* `pw232_to_ID.csv` = file mapping tip names in 2.3.2 tree file to identifiers in the main consortium metadata file

* figure files (PNG and PDF format; output from executing Rmd file)

