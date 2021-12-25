# Project Description

One of the Millennium Development Goals (2000-2015) was to halve the population without access to improved water sources by 2015. While this goal was met, a newer Sustainable Development Goal aims for everyone to have access to safely managed drinking water (improved water source). Among areas of the world, the African continent has the lowest acess to improved water sources. This report aims to describe the spatial patterns in access to improved water sources in Africa using publicly available 2011-2020 data from the Demagraphic and Health Surveys Program.

## Generate Report Using Renv
<details>
  <summary>Instructions</summary>
  
  ### Necessary Programs
  For this analysis it is necessary to have R and and the following installed on Ubuntu.
  ``` bash
  sudo apt-get update -y
  sudo apt-get install -y libudunits2-dev
  sudo aptitude install libgdal-dev
  ```
  
  ### Restore Package Environment
  Prior to executing the analysis, navigate to the `AfricaDHSWASH` directory and start an R session
  ```bash
  R
  ```
  In the R session, run the following to restore the package environment
  ```R
  renv::restore()
  ```
  There may be a lot of output. Please note any errors or warnings of uninstalled packages that come up.
  Quit the R session once this step is completed.
  ```R
  q()
  ```
  ### Execute Analysis
  To execute the analysis, from the `AfricaDHSWASH` directory, run the following
  ``` bash
  Rscript -e "rmarkdown::render('FInal_Proj_Doc.Rmd', output_file = 'Output/SpatialReport.html', quiet = TRUE)"
  ```
  This will create in the `AfricaDHSWASH/Output` directory, a file called `SpatialReport.html` which contains a report of the findings.
  Please note that this process may take about 10 minutes.
</details>