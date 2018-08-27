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

You may find a detailed documentation of the ARGP tool at [Wiki](https://github.com/mariakotouza/ARGP-Tool/wiki/Antigen-receptor-gene-profiler-(ARGP)). 

##  License
This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit https://creativecommons.org/licenses/by-nc-sa/4.0/.