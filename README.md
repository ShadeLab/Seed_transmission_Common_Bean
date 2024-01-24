# Seed_transmission_Common_Bean
 Sequence processing and analysis for the Common Bean seed endophyte transmission manuscript
## Github Repository for
# Stable transmission of bean seed microbiome members over three plant generations
## by Abby Sulesky-Grieb, Marie Simonin, A. Fina Bintarti, Brice Marolleau, Matthieu Barret, and Ashley Shade 
<i>This work is not published but is available on bioRxiv.</i>


### Data
The raw data for this study are available in the NCBI SRA under bioproject [PRJNA1058980](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA1058980/)


### To cite this work or code



### Abstract



### Contents

Code is split up into three directories: [Seed_sequence_processing.Rmd](https://github.com/ShadeLab/Seed_transmission_Common_Bean/blob/main/New_Seq_processing_June2023.Rmd), [] and [Analysis](https://github.com/ShadeLab/Centralia_RNA_DNA_multiyear/tree/main/Analysis).

#### Sequence processing
Code used for sequence processing including read QC, OTU clustering, taxonomy assignment, and tree building can be found under [Sequence_processing](https://github.com/ShadeLab/Centralia_RNA_DNA_multiyear/tree/main/Sequence_processing). Scripts were run using SLURM on the MSU HPCC using slurm batch files with suffix .sb and are numbered by their order in the processing workflow. Outputs such as logs, warnings, or errors if any, are designated by the suffix .out and named in accordence with the library, run number, and slurm batch file. 

#### Analysis
Formal analysis can be found under [Analysis](https://github.com/ShadeLab/Centralia_RNA_DNA_multiyear/tree/main/Analysis). All analysis was run with R and code was run in Rmarkdown. In the analysis directory you'll find the raw Rmarkdown files (.Rmd), a github friendly markdown rendering (.md) and the associated figure files from the rendering in separate sub-directories. The analysis was broken down into multiple chunks in separate Rmarkdown files: