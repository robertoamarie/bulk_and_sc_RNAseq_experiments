READAPT THE README

# bulk-RNAseq analysis

Project for Transcriptomics Course 2021 (MSc Bioinformatics for Computational Genomics) helded by Prof. Giulio Pavesi at Università degli Studi di Milano.

The vignette can be viewed here [GitHub page](https://mariachiaragrieco.github.io/bulk-RNAseq/)


## **Description**
The aim of this project is to perform a bioinformatic analysis on bulk RNA-seq samples for finding and characterizing DE genes. 

The RNA-seq data are retrieved from [Recount2](https://jhubiostatistics.shinyapps.io/recount/) and the analysis is done on three tissues (three replicates per tissue): colon, heart and liver.
Data for each tissue are in the “Ranged Summarized Experiment” format of Recount2.

For calling DE genes [edgeR](http://bioconductor.org/packages/release/bioc/html/edgeR.html) is used to investigated all pairwise comparisons:
* Colon vs Heart
* Colon vs Liver
* Heart vs Liver

For each tissue a list of DE genes is obtained comprising:
* genes found to be up-(down-)regulated with respect to either one of the other two
* genes found to be up- (down-) regulated with respect to both the other two

Then, a functional enrichment analysis is performed in order to determine whether the enriched GO annotations are consistent wiht the fact that the genes are up-regulated (or down-regulated) in the specific tissue.


## References
Collado-Torres L, Nellore A, Kammers K, Ellis SE, Taub MA, Hansen KD, Jaffe AE, Langmead B, Leek JT. Reproducible RNA-seq analysis using recount2. Nature Biotechnology, 2017. doi: 10.1038/nbt.3838.

Robinson MD, McCarthy DJ, Smyth GK (2010). “edgeR: a Bioconductor package for differential expression analysis of digital gene expression data.” Bioinformatics, 26(1), 139-140. doi: 10.1093/bioinformatics/btp616. 








# sc-RNAseq-brain analysis

Project for Transcriptomics Course 20__ (MSc Bioinformatics for Computational Genomics) helded by Prof. Giulio Pavesi at Università degli Studi di Milano.

The vignette can be viewed here ________



## **Description**
The aim of this project is to perform a single cell RNA-Seq study for finding and characterizing cell subtypes

Single-cell RNA-Seq data are retrieved from [PanglaoDB](https://panglaodb.se/index.html) analyzed in this study [“Structural Remodeling of the Human Colonic Mesenchyme in Inflammatory Bowel Disease” (Kinchen J. et al. 2018)](https://pubmed.ncbi.nlm.nih.gov/30270042/) aimed to define how the colonic mesenchyme remodels to fuel inflammation and barrier dysfunction in IBD (Inflammatory Bowel Disease).

The general workflow of the computational analysis here described is based on [Seurat](https://satijalab.org/seurat/) and follows the [Seurat vignette](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html), to find “well defined” clusters to which assign a cell type based on the DE/marker genes found in each.

## References

"Kinchen J, Chen HH, Parikh K, et al. Structural Remodeling of the Human Colonic Mesenchyme in Inflammatory Bowel Disease." Cell. 2018;175(2):372-386.e17. doi:10.1016/j.cell.2018.08.067

"ScRNA-Seq Analysis Workflow." (Hillje, R. 2020.) GitHub Repository. https://romanhaa.github.io/projects/scrnaseq_workflow/; GitHub.
