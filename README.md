# Summer_Internship_2020

**Objective**

In this study, I analyzed  coronaviruses (CoVs) genes differential expression infections to determine how each virus differs during infection. Here, I focused the analysis on samples from severe acute respiratory syndrome (SARS-CoV), Middle East Respiratory Syndrome (MERS), and severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2).  

**RAW FASTQ FILES**

* The raw sequence data (fastq files) for SARS-CoV was downloaded from GEO [GSE56192](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE56192), including its corresponding Mock-treated controls. 

* The raw sequence data (fastq files) for the SARS-CoV-2 infections was downloaded from GEO ([GSE147507](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE147507)), including its corresponding Mock-treated controls). 

* The raw sequence data (fastq files) for the MERS infections was downloaded from GEO [GSE139516](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE139516), including its corresponding Mock-treated controls.

**Pipeline Workflow**

*   PreProcessing
    
      * PCR clean - to remove duplicates from the PCR run  thus reducing redundancy. 
      * Trimmomatic - removes adapter sequences
      
*   Mapping 

      * Bowtie-2t
      
* Quantification 

    * RSEM -  Fragment Per Kilobase of transcript per Million mapped reads  for Paired-End Reads

* Differential Gene Expression

    * DESeq2
    
* Machine Learning 

    * Principal Component Analysis


