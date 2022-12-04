# BENG183project
# scRNA-seq
## Purpose
Imagine we are interested in genes that cause lung cancer. We collect cells from our lung tissue, but there are different cells in this tissue. If we treat all kinds of cells as the same type, which is exactly what we do in bulk RNA-seq, since gene expressions are different in different cells, it is obvious that we will lose important information. How do we know which gene in which kinds of cells is the key abnormality that causes cancer?
![lung tissue](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.37.25.png "cells in lung tissue")
###### Figure1: Lung tissue
To deal with these problems, techniques that can separately analyze different cells in the same tissue are needed. scRNA-seq is the one that tackles this problem. scRNA-seq can sequence different cells, and generate a dataset in which each sample is a cell in the tissue and the features are the gene expression of the cell. And most importantly, this technique allows us to analyze more than 15000 cells in a short period of time, which significantly save researchers time. 
![difference]("https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-12-04%2015.06.13.png")
###### Figure2: Difference Between Bulk RNA-seq and scRNA-seq
Due to the efficiency and effectiveness of the technique, it is useful to learn more about scRNA-seq technology.

## Upstream 
### Sequencing Process
Here we can see the process of sequencing: 
Encoded beads will flow through the microfluidics and meet with the cell. The microfluidics are well designed so that only one beads are allowed to pass. The combination of a cell, a bead, and reagents will form a droplet when they enter the microfluidic that is filled with oil. Then the connection of barcode and RNA will starts. After RNA gets barcoded, we will use PCR to amplify reads and sequence all reads using RNA-seq techniques.
![10X seq](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.35.23.png "10x seq procedure")
###### Figure 2: 10X seq
### The Beads and Barcodes
We can notice there are few region on our barcode. These barcodes are critical for researchers to know the origin of different RNA reads, and there are different function for different region. The 10x barcodes region will indicate the origin of the read, and the UMI code region can reduce the bias from amplification steps by indicating reads that are multiple copies of the same gene or actually different genes. After that, we will start our downstream analysis. 
![barcodes](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.36.03.png "barcodes")
###### Figure3: Bead and Barcode

## Downstream
### Quality Check

### Seurat

## Reference
1. “Brent Cornell.” BioNinja, http://www.ib.bioninja.com.au/options/option-d-human-physiology/d6-transport-of-respiratory/lung-tissue.html. 
2. “Recent Advances in Single-Cell Genomics Techniques.” Genomics Research from Technology Networks, https://www.technologynetworks.com/genomics/articles/recent-advances-in-single-cell-genomics-techniques-324695. 
3. IBioEducation, director. Single Cell Sequencing. YouTube, YouTube, 28 Aug. 2020, https://www.youtube.com/watch?v=k9VFNLLQP8c&amp;t=479s. Accessed 4 Dec. 2022. 

