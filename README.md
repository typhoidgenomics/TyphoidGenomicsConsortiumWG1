# Typhoid Genomics Consortium Paper: Global distribution of genotypes and AMR (2022)

This repo holds the data and code behind the first paper of the [Typhoid Genomics Consortium](https://typhoidgenomics.org/).

## Main data file 

`TGC_data_121022.csv`

* line list of all genomes including data accessions, source information, plus genome-derived genotype and AMR variables

* see metadata template [bit.ly/typhiMeta](bit.ly/typhiMeta) for details of source data coding

* genotype and AMR columns are derived using the [Mykrobe implementation](https://github.com/katholt/genotyphi) of the [GenoTyphi](https://doi.org/10.1093/infdis/jiab414) scheme, and [Typhi Pathogenwatch](https://doi.org/10.1038/s41467-021-23091-2)

## Genotype analysis

`/genotypes` directory

* `genotypes_121022.Rmd` = R markdown file for all analysis, generating tables and figures

* `genotypes_121022.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format)

* supplementary table files (CSV format)

## AMR analysis

`/AMR` directory

* `AMR_summary_191022.Rmd` = R markdown file for all analysis, generating tables and figures

* `AMR_summary_191022.html` = knitR output of Rmd file, including all figures and numbers included in text

* figure files (PNG and PDF format)

* supplementary table files (CSV format)
