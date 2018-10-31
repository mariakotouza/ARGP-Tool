# Antigen receptor gene profiler (ARGP)

ARGP is a software framework that provides analytics services on NGS Data, implemented in [R Shiny](https://shiny.rstudio.com/).

## Installation

#### R Shiny packages

```
install.packages(c("shiny","shinyFiles", "shinyjs", "shinyBS"))
```

#### Other packages for data processing and visualization

```
install.packages(c("DT","plyr","dplyr","pryr","data.table","stringr","tidyr","xtable","plot3D","gridExtra","stringdist","plotly"))
source("http://bioconductor.org/biocLite.R")
biocLite("Biostrings")
source("https://bioconductor.org/biocLite.R") 
biocLite("motifStack")
```

##  Run the Application

- You can run the application by pressing the **"Run App"** button, from either **ui.R** or **server.R** script.
- The Datasets you want to process together must be contained into a folder organised into sub-folders. The Data folder contains some sample datasets.
- All the datasets that you select to process together must have the same column names (attributes).
- In order to successfully run the pipeline, you need to run the preselection and selection steps first. In the case that you do not want to filter out any rows from the dataset, you just have to press the Apply and Execute buttons at the Preselection and Selection panels accordingly, before continuing with the pipeline steps. The information at the Visualization and the Overview tabs will become available when the execution of the pipeline is completed. You will get a corresponding message for each step that you have selected (e.g. "Clonotypes run!") when this happens. 
- If you want to use only those attributes of the tables that are necessary to run the pipeline, you need to set the variable use_only_useful_columns equal to True, otherwise you set it equal to False. You can see those attributes in the param/ used_columns.csv and param/ used_columns_only_useful.csv files accordingly. 


You may find a detailed documentation of the ARGP tool at [Wiki](https://github.com/mariakotouza/ARGP-Tool/wiki/Antigen-receptor-gene-profiler-(ARGP)). 

##  License
This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit https://creativecommons.org/licenses/by-nc-sa/4.0/.