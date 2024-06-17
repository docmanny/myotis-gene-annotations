---
name: Mis/Unannotated Gene Report
about: Use this template to flag a gene that is either missing or misannotated in
  one or more genomes.
title: Gene XYZ [misannotated | unannotated] in genome(s) A(, B, ...)
labels: Misannotated Gene, Unannotated Gene
assignees: docmanny

---

__Gene:__ XYZ1
__Genomes:__ A, B, C

## Details:

Gene XYZ1 is missing from the GFF3 of genome A. In genomes B & C, the gene exists and has the following IDs:

|genome  |  ID=  |
|----------|-------|
| genomeB  |  EVM.SUPER__5.51 |
| genomeC  |  EVM.SUPER__4.40 |

I used reciprocal best-hit BLAST starting from hg38 to search for XYZ1 orthologs in all genomes, and found XYZ1 in genome A and the missing exons in B & C. 

## Files:

1. GFF3 file describing location & structure of the genes. If its an _unannotated gene_, please list the method used to identify it in the second column of the GFF3, and please use a unique string for the ID attributes of the features. If its a _mis-annotated gene_, please make sure that you preserve the original ID for the gene-level feature from the GFF3. 

2. Any additional lines of evidence that you used to identify the error.
