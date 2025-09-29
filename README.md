# MiCM RNA-seq Analysis II

## Overview

Participants will learn how to use DESeq2 to identify differentially expressed genes and become familiar with design matrices. The session will also introduce concepts essential for working with real-world data, such as incorporating covariates and interaction terms into models. Additionally, participants will learn how to apply Over-Representation analysis (ORA) and Gene Set Enrichment Analysis (GSEA) for uncovering biologically meaningful patterns. Hands-on examples and exercises will help reinforce concepts and guide participants through a typical RNA-seq workflow.
   
## Requirements
* Familiarity with R
* Access to an IDE (Rstudio is recommended)
   
## Sofware
* [R](https://www.r-project.org/) (>=4.0.0)
* [Rstudio](https://posit.co/products/open-source/rstudio/?sid=1)

In R, install the following libraries (in case they are not already installed):
```{r}
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("DESeq2")
BiocManager::install("vsn")
install.packages("hexbin")
install.packages("pheatmap")
install.packages("RColorBrewer")
BiocManager::install("EnhancedVolcano")
install.packages("ggplot2")
install.packages("ggbeeswarm")
install.packages("ashr")
install.packages("knit")
BiocManager::install("fgsea")
install.packages("GSA")
install.packages("enrichR")
```

## Outline
* [01 - DESeq2](https://arielmadr.github.io/MiCM_RNA_Seq_2/Exercises/scripts/01_run_DESeq2.nb.html)
* [02 - GSEA and ORA](https://arielmadr.github.io/MiCM_RNA_Seq_2/Exercises/scripts/02_gsea_and_ora.nb.html)

## References

*<This workshop uses processed RNA-seq counts from this [study](https://doi.org/10.1016/j.stem.2021.04.028)>*

*<This workshop  used material adapted from the following sources:>*

* [DESeq2 vignette](https://www.bioconductor.org/packages/release/bioc/vignettes/DESeq2/inst/doc/DESeq2.html)
* [RNA-seq workflow](https://master.bioconductor.org/packages/release/workflows/vignettes/rnaseqGene/inst/doc/rnaseqGene.html)
* [fgsea vignette](https://bioconductor.org/packages/release/bioc/vignettes/fgsea/inst/doc/fgsea-tutorial.html)
* [enrichR vignette](https://cran.r-project.org/web/packages/enrichR/vignettes/enrichR.html)
* [MiCM intro to RNA](https://github.com/aosakwe/MiCM_IntroToRNA)

*Workshop created as part of the McGill Initiative in Computational Medicine*
