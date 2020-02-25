# Kallisto Pipeline

This repository contains various Jupyter lab notebooks that are used in developing scripts to analyze count matrices and create low dimensional analyses. The devel branch will contain the notebooks to track the development of the project while the master will contain completely functional scripts (hopefully). Currently, only the tutorial dataset has been analyzed.
The process of running Kallisto for these projects will also be outlined in the README.
1. Install Kallisto and Bustools from their websites
2. ```mkdir kallisto_bustools_sample/; cd kallisto_bustools_sample/```
3. You can either either make Kallisto a global variable or you can put the Kallisto files in the kallisto_bustools_sample folder.
4. ```cd 01/```
5. For these projects, the index has already been built and placed in the folder.
6. ```./kallisto bus -i <index_file> (cDNA_introns.idx) -o <desired_output_folder> -x <Technology used> -t <Thread Count> <FASTQ1> <FASTQ2> ```

Notes about kallisto, you need at least 2 FASTQ files to do this, the FASTQ files neeed to be gz files, and you can figure out which technologies are available by doing ```./kallisto bus -l```
