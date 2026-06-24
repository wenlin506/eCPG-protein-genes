Protein-coding genes in eukaryotic genome often produce alternatively spliced transcripts. This observation is intensified with accumulating short-read NGS sequencing data, however, there are issues in the accurate spliced isoforms expression profiles. Furthermore, identifying authentic translated peptide products requires tissue-specific transcript expression profiles. In the current study, we utilized the long-read GSE192955 dataset to identify the most abundantly expressed protein-coding transcripts isoforms. This dataset derived from 30 normal human tissues, discovered 18,094 highly expressed representative protein-coding transcripts (Ref-Tx) from a total of 18,557 human protein-coding genes. 14,546 Ref-Tx transcripts corresponded with annotated MANE-select transcripts. Comparing with the previous GTEx datsets, the GSE192955 long-read dataset exhibits more Rank1 Ref-Tx discovery and enhanced MANE-select transcript concordance. We also developed a bioinformatics tool for expression visualization on the protein-coding genes from 30 normal human tissues. There are few python scrips utilized for the expression data processing and gene annotation. 
Script1: Processing all MANE annotated genes from GSE192955 dataset.
Script2: Extracting GSE192955 unique transcripts (not observed in the GTEx V8 short-read dataset).
Script3: Parsing GSE192955 expression dataset into 30 tissue types.

Data files used for python scripts:
data1:
data2:
data3:
data4:
data5:
data6:
data7:

All scripts are provided with the source txt format and python format. Script1 used data1, data2 and data3 files. Script2 used data1 and data7 files. Script3 used data4 and data5 files. You can download and execute the python scripts and required datafiles in the same directory.

