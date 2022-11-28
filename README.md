# BENG183project
# scRNA-seq
## Purpose
Imagine we are interested in genes that cause lung cancer. We collect cells from our lung tissue, but there are different cells in this  tissue, and gene expressions are different in different cells. How do we know which gene in which cell is the key abnormality that causes cancer?
![lung tissue](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.37.25.png "cells in lung tissue")
To deal with these problems, techniques that can separately analyze different cells in the same tissue is needed. scRNA-seq is the one that tackle this problem. scRNA-seq can sequence different cells, generate a dataset in which each sample is a cell in the tissue and the features are the gene expression of the cell. 

Most importantly, we can analyze more than 15000 cells in a short period of time, which significantly save researcher's time. And now we are going to explain the stepwise procedure of a scRNA-seq.

## Upstream 
Here we can see the process of sequencing: 
Encoded beads will flow through the microfluidics and meet with the cell. The combination of cell and bead or a mere bead will form a droplet when they enters microfluidic filled by oil, this will ensure each cell will only react with one bead in next step. Then we will use PCR and sequence all reads using normal RNA seq rechniques.
![10X seq](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.35.23.png "10x seq procedure")
### The Beads and Barcodes
The microfluidics's size are controlled to similar size as the bead, which prevent the scene where 2 beads and one cell are in one droplet, this kind of error cannot be filtered out in later data proessing, which makes it important to prevent at upstream steps. The 10x barcodes will indicate the read comes from which cell, and the UMI code can reduce the bias from amplification steps by indicating those reads are multiple copies of same gene or actually different genes. 
![barcodes](https://github.com/GYDTTDYX/BENG183project/blob/main/%E6%88%AA%E5%B1%8F2022-11-28%2009.36.03.png "barcodes")

## Downstream
### Quality Check

### Seurat
