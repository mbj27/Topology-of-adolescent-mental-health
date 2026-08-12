# Code repository for Topology-of-adolescent-mental-health

Code correspondence: Maria B. Jelen

### Data
This code uses the ABCD data, obtained from the 5.1 release from the ABCD Study Data Repository from the NIMH Data Archive (https://nda.nih.gov/abcd) following appropriate data access permissions. Authorised access to the ABCD Data Repository is required to obtain ABCD data, hence source data is not shared on this repository. 

Main analysis scripts have been provided with simulated mock datasets to facilitate functionality of scripts, but these will not directly reproduce manuscript results.

### Required software
1. RStudio 4.5.2 (installation: https://rstudio.com/products/rstudio/download/)
2. Python 3.9.10 via Jupyter Noteboook (installation: https://docs.jupyter.org/en/latest/install/notebook-classic.html)
3. (suggested) Visual Studio Code (installation: https://code.visualstudio.com/download?_exp_download=d53503e735)

OS: Windows or macOS. 

Typical installation time: 15-20 min, depending on system/existing Python/R set-up.  

Non-standard hardware: Not required.  


### Instructions

#### To view original code generating results and figures from manuscript

Navigate to /scripts and view files in below order:

1. Data imputation and cleaning (ABCD-dataprep.Rmd)
2. SOM and psychopathology profile development (SOM.ipynb)
     - Training and validaiton of SOM
     - Clustering and alternative assessment of SOM topology - psychopathology profiles
     - Overlap with diagnostic burden
     - Stability over follow-up time points (SOM-followup.ipynb)
3. Resting-state fMRI PLS Analysis 
     - fMRI data cleaning preparation (fMRI_dataprep.ipynb)
     - PLS analysis (PLS-rsFC.ipynb)
4. Polygenic Risk Score PLS Analysis (PLS-PGR.ipynb)
5. Edge-type Analysis - Rich, Feeder and Local connections (PLS-richclub.ipynb)
6. AHBA gene expression x Psychopathology connectivity PLS (Gene_annotation.ipynb)
7. Gene Ontology - g:Profiler documentation

#### To trial main analytical scripts on simulated data

Navigate to /sim, download mock data files and run code files in below order:

1. SOM and psychopathology profile development 
     - Training and validaiton of SOM
     - Clustering and alternative assessment of SOM topology - psychopathology profiles
     - Overlap with diagnostic burden
     - Stability over follow-up time points 
2. Resting-state fMRI PLS Analysis 
3. Polygenic Risk Score PLS Analysis 
4. Edge-type Analysis - Rich, Feeder and Local connections 
5. AHBA gene expression x Psychopathology connectivity PLS 
