# BENG183project
# scRNA-seq
## Purpose
Imagine we are interested in genes that cause lung cancer. We collect cells from our lung tissue, but there are different cells in this tissue, and gene expressions are different in different cells. How do we know which gene in which kinds of cells is the key abnormality that causes cancer?
![lung tissue](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.37.25.png "cells in lung tissue")
To deal with these problems, techniques that can separately analyze different cells in the same tissue are needed. scRNA-seq is the one that tackles this problem. scRNA-seq can sequence different cells, and generate a dataset in which each sample is a cell in the tissue and the features are the gene expression of the cell. And most importantly, this technique allows us to analyze more than 15000 cells in a short period of time, which significantly save researchers time. 
Due to the efficiency and effectiveness of the technique, it is useful to learn more about scRNA-seq technology.

## Upstream 
### Sequencing Process
Here we can see the process of sequencing: 
Encoded beads will flow through the microfluidics and meet with the cell. The combination of a cell, a bead, and reagents will form a droplet when they enter the microfluidic that is filled with oil, this step ensures each cell will only react with one bead. After RNA gets barcoded, we will use PCR to amplify reads and sequence all reads using RNA-seq techniques.
![10X seq](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.35.23.png "10x seq procedure")
### The Beads and Barcodes
The beads and barcodes are critical for researchers to know the origin of different RNA reads. The 10x barcodes will indicate the origin of the read, and the UMI code can reduce the bias from amplification steps by indicating those reads are multiple copies of the same gene or actually different genes. After that, we will start our downstream analysis. 
![barcodes](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.36.03.png "barcodes")

## Downstream
### Quality Check

### Seurat

## Reference
IBioEducation, director. Single Cell Sequencing. YouTube, YouTube, 28 Aug. 2020, https://www.youtube.com/watch?v=k9VFNLLQP8c&amp;t=479s. Accessed 4 Dec. 2022. //
“Brent Cornell.” BioNinja, http://www.ib.bioninja.com.au/options/option-d-human-physiology/d6-transport-of-respiratory/lung-tissue.html. //
“Recent Advances in Single-Cell Genomics Techniques.” Genomics Research from Technology Networks, https://www.technologynetworks.com/genomics/articles/recent-advances-in-single-cell-genomics-techniques-324695. 
