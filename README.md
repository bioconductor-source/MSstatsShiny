# MSstatsShiny

This repository contains the code for the R Shiny app MSstatsShiny, which 
utilizes MSstats, MSstatsTMT, and MSstatsPTM to analyze proteomics experiments.

## Availability

The application is available both online and locally, with planned release on 
Bioconductor in October 2022.

### Online

The online application is located at 
[http://www.msstatsshiny.com/](http://www.msstatsshiny.com/). The online version
is constrained by the processing limits of the server. Due to this we recommend 
only processing small datasets on the platform. Large datasets will likely run 
out of memory on the data summarization step.

### Local

For large file processing, it is recommend you use a local install of the 
application. To install and run the application locally, please follow these 
steps.

1. Download [R](https://www.r-project.org/) and [RStudio](https://www.rstudio.com/products/rstudio/download/) - [How to](https://rstudio-education.github.io/hopr/starting.html).
4. Install the dependencies listed below.
5. Install the package by executing `devtools::install_github("Vitek-Lab/MSstatsShiny")` in the console.
5. Run the application by executing `library(MSstatsShiny)` and `launch_MSstatsShiny()` or `MSstatsShiny::launch_MSstatsShiny()` in the console.

#### Dependencies


  `install.packages(c('shiny', 'shinyBS', 'shinybusy', 'shinyjs', 'uuid', 'DT', 'knitr',
                    'plotly', 'ggrepel', 'gplots', 'tidyverse', 'data.table', 'BiocManager', 'devtools'))`
                    
  `BiocManager::install(c('MSstatsPTM', 'biomaRt'))`

## Processing instructions

Instructions for processing your dataset are listed directly in the application. The general workflow includes: uploading your data into the application, run level summarization and vizualization, and data modeling to determine differential proteins. For questions on how to process your data please see the Help section of the application.

