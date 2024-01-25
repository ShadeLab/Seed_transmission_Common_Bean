# Seed_transmission_Common_Bean
 Sequence processing and analysis for the Common Bean seed endophyte transmission manuscript
## Github Repository for
# Stable transmission of bean seed microbiome members over three plant generations
## by Abby Sulesky-Grieb, Marie Simonin, A. Fina Bintarti, Brice Marolleau, Matthieu Barret, and Ashley Shade 
<i>This work is not published but will soon be available on bioRxiv.</i>


### Data
The raw data for this study are available in the NCBI SRA under bioproject [PRJNA1058980](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA1058980/)


### To cite this work or code
Coming soon.


### Abstract
Coming soon.


### Contents

Code is split up into three directories: [Seed_sequence_processing.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Seed_sequence_processing.Rmd), [Seed_analysis_sequence_decontam.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Seed_analysis_sequence_decontam.Rmd) and [Bean_seed_transmission_analysis_clean.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Bean_seed_transmission_analysis_clean.Rmd). Files necessary to run R code are located in [R_Analysis_Files](https://github.com/ShadeLab/Seed_transmission_Common_Bean/tree/main/R_Analysis_Files).

#### Sequence processing
Code used for sequence processing including read QC, ASV clustering, taxonomy assignment, and tree building can be found under  [Seed_sequence_processing.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Seed_sequence_processing.Rmd). Scripts were run in QIIME2 using SLURM on the MSU HPCC using slurm batch files with suffix .sb. 

#### Sequence decontamination
Code for sequence decontamination by extraction group can be found in [Seed_analysis_sequence_decontam.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Seed_analysis_sequence_decontam.Rmd). Output ASV table, taxonomy and metadata files from QIIME2 were used to create a Phyloseq object in R, labelled multigen_phyloseq.rds. Files are available in R_Analysis_Files folder. 

#### Analysis
Formal analysis can be found under  [Bean_seed_transmission_analysis_clean.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/Bean_seed_transmission_analysis_clean.Rmd). All analysis was run with R and code was run in Rmarkdown. After sequence decontamination, the phylogenetic tree was added to the Phyloseq object, and metadata was updated with additional variables for analysis. These files are labelled tree.nwk and seed_meta_update.csv. The updated Phyloseq object is labelled seed_phyloseq_decontam_updatemeta.rds. The list of core bean seed ASVs and the bean root core taxa FASTA file can be found in the R_Analysis_Files folder.


### Funding
This work was supported by the United States Department of Agriculture award 2019-67019-29305, and by the Michigan State University [Plant Resilience Institute](https://plantresilience.msu.edu). 

### More info
[ShadeLab](http://ashley17061.wixsite.com/shadelab/home)