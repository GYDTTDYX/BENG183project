# BENG183project
# scRNA-seq
## Purpose
Imagine we are interested in genes that cause lung cancer. We collect cells from our lung tissue, but there are different cells in this  tissue, and gene expressions are different in different cells. How do we know which gene in which kinds of cells is the key abnormality that causes cancer?
![lung tissue](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.37.25.png "cells in lung tissue")
To deal with these problems, techniques that can separately analyze different cells in the same tissue is needed. scRNA-seq is the one that tackle this problem. scRNA-seq can sequence different cells, generate a dataset in which each sample is a cell in the tissue and the features are the gene expression of the cell. And most importantly, this technique allow us to analyze more than 15000 cells in a short period of time, which significantly save researcher's time. 
Due to the efficiency and effectiveness of the technique, it is useful to learn more about scRNA-seq technology.

## Upstream 
### Sequencing Process
Here we can see the process of sequencing: 
Encoded beads will flow through the microfluidics and meet with the cell. The combination of a cell, a bead, and reagents will form a droplet when they enters the microfluidic that filled by oil, this step ensures each cell will only react with one bead. After RNA get barcoded, we will use PCR to amplify reads and sequence all reads using RNA seq techniques.
![10X seq](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.35.23.png "10x seq procedure")
### The Beads and Barcodes
The beads and barcodes is critical for researchers to know the origin of different RNA reads. The 10x barcodes will indicate the origin of read, and the UMI code can reduce the bias from amplification steps by indicating those reads are multiple copies of same gene or actually different genes. After that, we will starts our downstream analysis. 
![barcodes](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.36.03.png "barcodes")

## Downstream
### Quality Check

### Seurat
