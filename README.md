# Analysis-of-data-by-dpMIG-seq
<br>
On this page, we deposited the code for the analysis of data obtained by dpMIG-seq.


## 1. Performance comparison between dpMIG-seq and MIG-seq
### 1-1. Analysis of the number of polymorphisms between primer sets using tomato

<br>
The files related to this analysis are stored in the directory "1-1.Analysis_of_the_number_of_polymorphisms_between_primer_sets_using_tomato".  
<br>
In polymorphism_detection_pipline.sh,<br>
raw fastq files were trimmed using trimmomatic,<br>
mapped to reference genome using bwa, and variant calling was performed using samtools mpileup.  
<br>
In order for this script to work, the fastq file must be downloaded from SRA and placed in the "rawdata" folder.
<br>
<br>
Comparison_of_number_of_polymorphisms.R<br>
<br>
<br>

### 1-2. Analysis of common loci between different primer sets
<br>
The script that calculates the commonality of polymorphisms using the results of analysis #1 as input is ~.
<br>

### 1-3. Analysis of the sequence to which the primers annealed
<br>
　〜A script called ~ can be used to extract sequences from the observed sequence reads that the primers are thought to have annealed to. <br>
 The frequency of these sequences is then aggregated for each sequence, and a sub-analysis is performed to determine how many different types of sequences the primers annealed to for each primer set. <br>
 <br>
 
## 2. Performance evaluation of dpMIG-seq on various_crops
<br>
We are investigating the number of bases in the region that can be stably sequenced by dpMIG-seq and MIG-seq using 11 plant species. <br>
First, trimming, mapping, and bam sorting are done with a script called ~. <br>
<br>
Then, the R script named ~ is used to calculate the results. <br>
<br>

## 3. Investigation of the amount of data required for effective application of dpMIG-seq in wheat
<br>
First, we obtained 2 Gb data volumes for two tetraploid wheat lines and calculated the change in the number of polymorphisms per data volume. <br>
The script for this analysis is ~.<br>
<br>
Next, we demonstrated whether it could be used effectively to select a group during backcrossing. <br>
The script for this analysis is ~.<br>

## 4. Development of a method to apply dpMIG-seq without DNA purification 
<br>
Included is a script on evaluating the effectiveness of dpMIG-seq using lysate as a template. <br>
First, we analyzed the number of detectable polymorphisms and commonality of polymorphisms between the five library construction methods in tomato and rice. <br> 
<br> <br>Then, we analyzed the number of polymorphisms detected and the commonality of polymorphisms among the five library construction methods in tomato and rice.
Next, we tested whether the results of PCA analysis were consistent with the polymorphisms detected by the five library construction methods. <br> <br>
This analysis can be performed with a script called ~. <br>

## 5. Linkage analysis using F2 populations of rice
<br>
This script performs polymorphism detection, linkage map construction (LEP-MAP3) and QTL analysis (R/qtl) on dpMIG-seq of rice F2 population. <br>
<br>

## 6. Linkage analysis using a F2 populations of tomato
<br>
This script performs polymorphism detection, linkage map construction (LEP-MAP3) and QTL analysis (R/qtl) on dpMIG-seq of tomato F2 population. <br>
<br>

## 7. Linkage analysis using RILs of soy
<br>
This script performs polymorphism detection, linkage map construction (LEP-MAP3) and QTL analysis (R/qtl) on dpMIG-seq of soy RILs population. <br>
<br>


