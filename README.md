This repository contains the R code discussed in the paper [Exploring microbial diversity using cell-size fractionated enrichment incubations from subsurface aquifers at Äspö, Sweden](https://doi.org/10.1038/s42003-026-09706-8).

The raw data was deposited at the [ENA](https://www.ebi.ac.uk/ena) with PRJEB71769 as reference, and consists of 15 metagenomes and 98 16S samples. The nucleotide sequences of the metagenome-assembled genomes were deposited in [Figshare](https://doi.org/10.6084/m9.figshare.31228549).

The following files are required in the R script ```didactic-spork.qmd``` and can be found in the mag subdirectory: 

* The read coverage of each MAG: ```coverm-mapping.tsv```
* The functional annotation: ```emapper.tsv.gz```
* The taxonomical annotation: ```gtdbtk.summary.tsv```
* CheckM2 output: ```quality-report.tsv```
* The output of KEGG mapper to evaluate module completeness: ```kegg-mapper.tsv.gz```
* Trait profiling based on the MAG's functional potential: ```metabolic.tsv.gz```

The following files were part of the analysis of the 16S data and were uploaded to the ampliseq subdirectory:

* The ASV tabke: ```ASV_table.tsv.gz```
* The ASV's taxonomy including nucleotide sequence: ```ASV_tax_seqs.tsv.gz```
* Metadata: ```metadata.tsv```
* The summary of the bioinformatic pipeline: ```overall_summary.tsv```
* The additional ASVs used in the network analysis: ```survey-amplicons.tsv.gz```

These files are not related to sequence data but are required as well:
* Hydrochemistry of the groundwaters: ```sicada.tsv```
* Cell counts using epifluorescence microscopy: ```micro_cultures.tsv```
* Real-time PCR on the enrichment incubations: ```qpcr.tsv```