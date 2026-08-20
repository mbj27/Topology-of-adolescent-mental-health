# Code repository for Topology-of-adolescent-mental-health

Code correspondence: Maria B. Jelen

### Data
This code uses the ABCD data, obtained from the 5.1 release from the ABCD Study Data Repository from the NIMH Data Archive (https://nda.nih.gov/abcd) following appropriate data access permissions. Authorised access to the ABCD Data Repository is required to obtain ABCD data, hence source data is not shared on this repository. 

A demo containing main analysis scripts has been provided with simulated mock datasets to demonstrate functionality, but these cannot reproduce manuscript results.

### Required software
1. RStudio 4.5.2 (installation: https://rstudio.com/products/rstudio/download/)
2. Python 3.9.10 via Jupyter Noteboook (installation: https://docs.jupyter.org/en/latest/install/notebook-classic.html)
3. (suggested) Visual Studio Code (installation: https://code.visualstudio.com/download?_exp_download=d53503e735)

Required packages can be found in software_env.txt.  
OS: Coded on Windows, tested on macOS.   
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
3. Stability over follow-up time points (SOM-followup.ipynb)
4. Resting-state fMRI PLS Analysis 
     - fMRI data cleaning preparation (fMRI_dataprep.ipynb)
     - PLS analysis (PLS-rsFC.ipynb)
5. Polygenic Risk Score PLS Analysis (PLS-PGR.ipynb)
6. Edge-type Analysis - Rich, Feeder and Local connections (PLS-richclub.ipynb)
7. AHBA gene expression x Psychopathology connectivity PLS (Gene_annotation.ipynb)
8. Gene Ontology - g:Profiler documentation

*To apply analysis for your own data*, the code can be adapted for novel appropriately formatted data. Key formatting steps, including alignment, expected shape after cleaning etc., are included in scripts.

*To replicate the reported analysis*, authorised access to ABCD data is required. Preprocessing files demonstrate steps to obtain analysis variables from raw data.

#### To trial functionality of main analytical scripts on simulated data

Navigate to /demo, download mock data files and and code scripts, then run code files in below order:

1. SOM and psychopathology profile development (SOM_mock.ipynb)
     - Training and validation of SOM
     - Clustering and alternative assessment of SOM topology - psychopathology profiles
     - Overlap with diagnostic burden
2. Stability over follow-up time points (SOM-followup_mock.ipynb)
3. Resting-state fMRI PLS Analysis (PLS-rsFC_mock.ipynb)
4. Polygenic Risk Score PLS Analysis
5. Edge-type Analysis - Rich, Feeder and Local connections (PLS-richclub_mock.ipynb)
6. AHBA gene expression x Psychopathology connectivity PLS (Gene_annotation_mock.ipynb)

Expected demo run time: ~10 minutes.  
Expected outputs specified in /demo/README.md
Mock datasets, a trained SOM and classifier, and intermediate data processing files are provided.  
Note that all data in the demo is was generated randomly from normal/binomial distributions and does not have any affiliation with ABCD data. Participant pseudoidentifiers and associated data do not in any way correspond to real participants.

### Citation
Code is affiliated with the below preprint:
The topology of adolescent mental health
Maria B. Jelen, Alexa Mousley, Kayson Fakhar, Estherina Trachtenberg, Yuankai He, Robert Kohler, Shambhavi Aggarwal, Varun Warrier, Danilo Bzdok, Sarah W. Yip, Duncan E. Astle
medRxiv 2026.07.13.26357465; doi: https://doi.org/10.64898/2026.07.13.26357465
