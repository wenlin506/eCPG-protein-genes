Protein-coding genes in eukaryotic genome often produce alternatively spliced transcripts. This observation is intensified with accumulating short-read NGS sequencing data, however, there are issues in the accurate spliced isoforms expression profiles. Furthermore, identifying authentic translated peptide products requires tissue-specific transcript expression profiles. In the current study, we utilized the long-read GSE192955 dataset to identify the most abundantly expressed protein-coding transcripts isoforms. This dataset derived from 30 normal human tissues, discovered 18,094 highly expressed representative protein-coding transcripts (Ref-Tx) from a total of 18,557 human protein-coding genes. 14,546 Ref-Tx transcripts corresponded with annotated MANE-select transcripts. Comparing with the previous GTEx datsets, the GSE192955 long-read dataset exhibits more Rank1 Ref-Tx discovery and enhanced MANE-select transcript concordance. We also developed a bioinformatics tool for expression visualization on the protein-coding genes from 30 normal human tissues. There are few python scrips utilized for the expression data processing and gene annotation. 
Script1: Processing all MANE annotated genes from GSE192955 dataset.
Script2: Calculate gene expression values for each 30 tissue types.

Data files used for python scripts:
data1: iCPG_19338_StdRef_GSE192955
data2: GTEx_V8_V9_and_GSE192995_CDS_Rank
data3: GSE_unique_notV8
data4: GSE192955_30ClontechTissue

All scripts are provided with the source txt format. 
Script1 used data1, data2 and data3 files. This script processes all MANE annotated genes from GSE192955 dataset into xml format. 
It creates the following data columns: 'iCPG_ID', 'T2T_chr', 'Correct_19591ID_19338', 'V8_gene_id', 'V8_transcript_id', 'V8_chr', 'V8_gene_name', 'V8_Tx_TPM', 'V8_Gene_TPM', 'V8_Tx%', 'V8_Tx_type', 'V8_Tx_count', 'V8_Rank', 'V8_exon_count', 'V8_Tx_length', 'V8_Tx_CDS_len', 'V8_Ref_Tx', 'MANE_chr', 'MANE_match', 'MANE_gene', 'MANE_name', 'MANE_Tx', 'MANE_Tx_by_gene', 'MANE_by_v8_Tx', 'V9_gene_id', 'V9_name', 'V9_chr', 'V9_Tx_match', 'V9_Tx_TPM', 'V9_Gene_TPM', 'V9_Tx%', 'V9_Tx_count', 'V9_Rank', 'V9_Tx_type', 'V9_Ref_Tx', 'ONT_gene_id_by_Tx', 'ONT_Tx_id_by_V8', 'ONT_gene_name', 'ONT_Tx_count', 'ONT_Tx_FPKM', 'ONT_Gene_FPKM', 'ONT_Tx%', 'ONT_Rank', 'ONT_Ref_Tx', 'ONT_testis_1', 'ONT_testis_2', 'ONT_brain', 'match_GSE_gene', 'match_GSE_Tx', 'GSE_AVG_Tx', 'GSE_AVG_gene', 'GSE_Tx%', 'GSE_Rank', 'GSE_Ref_Tx', 'CDS_len_v34_pc_tx', 'Tx_type_v34_annotation', 'PC_Tx%', 'principal' 

Script2 used data4 file. This script generates tissue expression data from the GSE192955 dataset. 
It creates the following data columns: 'gene_ID', 'transcript_ID', 'Brain', 'Caudate_Nucleus', 'Cerebellum', 'Cerebral_Cortex', 'Corpus_Callosum', 'Fetal_Brain', 'Fetal_Spinal_Cord', 'Frontal_Lobe', 'Hippocampus', 'Medulla_Oblongata', 'Pons', 'Spinal_Cord', 'Temporal_Lobe', 'Thalamus', 'bladder', 'blood', 'colon', 'heart', 'kidney', 'liver', 'lung', 'ovary', 'pancreas', 'prostate', 'skeletal_muscle', 'small_intestine', 'spleen', 'stomach', 'testis', 'thyroid', 'Brain_gene', 'Caudate_Nucleus_gene', 'Cerebellum_gene', 'Cerebral_Cortex_gene', 'Corpus_Callosum_gene', 'Fetal_Brain_gene', 'Fetal_Spinal_Cord_gene', 'Frontal_Lobe_gene', 'Hippocampus_gene', 'Medulla_Oblongata_gene', 'Pons_gene', 'Spinal_Cord_gene', 'Temporal_Lobe_gene', 'Thalamus_gene', 'bladder_gene', 'blood_gene', 'colon_gene', 'heart_gene', 'kidney_gene', 'liver_gene', 'lung_gene', 'ovary_gene', 'pancreas_gene', 'prostate_gene', 'skeletal_muscle_gene', 'small_intestine_gene', 'spleen_gene', 'stomach_gene', 'testis_gene', 'thyroid_gene', 'AVG_Tx', 'AVG_gene', 'Tx%', 'Rank', 'Ref_Tx'. 

You can download and execute the python scripts and required datafiles in the same directory. For example: script1_Processing_all_MANE_annotated_genes_from_GSE192955_dataset.txt
Step 1: Save your code to a file
Make sure your Python code is saved in a file ending in .py. For example, save it as script1_Processing_all_MANE_annotated_genes_from_GSE192955_dataset.py, and place this .py file in the exact same folder where your dataset is located.

Step 2: Open your Command Line and Navigate to the Folder
Open your Command Prompt (Windows) or Terminal (Mac/Linux), and use the cd (change directory) command to navigate to the folder where your script and CSV file live.

Step 3: Run the Script 
Once your command line is pointing to the correct folder, execute the script by running:
(Windows):
python script1_Processing_all_MANE_annotated_genes_from_GSE192955_dataset.py
(Mac/Linux): 
python3 script1_Processing_all_MANE_annotated_genes_from_GSE192955_dataset.py
Output file:
For example, GeneID ENSG00000000457 and symbol SCYL3 of chromosome 1 output xml file is iCPG_chr1_GeneID_ENSG00000000457_SCYL3.xml 


