# Analysis-of-data-by-dpMIG-seq
<br>
On this page, we publish the code for the analysis of data obtained by dpMIG-seq.


## 1. Analysis of the number of polymorphisms between primer sets using tomato
<br>
The files related to this analysis are stored in the directory "1.Analysis_of_the_number_of_polymorphisms_between_primer_sets_using_tomato".  
<br>
In polymorphism_detection_pipline.sh,<br>
raw fastq files were trimmed using trimmomatic,<br>
mapped to reference genome using bwa, and variant calling was performed using samtools mpileup.  
<br>
In order for this script to work, the fastq file must be downloaded from SRA and placed in the "rawdata" folder.
<br>
<br>
<br>
Comparison_of_number_of_polymorphisms.R<br>
<br>
<br>
<br>
### Analysis of common loci between different primer sets
<br>
<br>
１番の解析結果を入力として、多型の共通性を計算するスクリプトは、。

### Analysis of the sequence to which the primers annealed



## 4. Evaluating the effectiveness of dpMIG-seq in crop species with various genome sizes



## 5. Investigation of the amount of data required for effective application of dpMIG-seq in wheat



## 6. Linkage analysis using segregating populations of rice, tomato, and melon



## 7. Development of a method to apply dpMIG-seq without DNA purification 
