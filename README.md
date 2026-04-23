# Topology-of-adolescent-mental-health

Code correspondence: Maria B. Jelen

This code uses the ABCD data, obtained from the 5.1 release from the ABCD Study Data Repository from the NIMH Data Archive (https://nda.nih.gov/abcd) following appropriate data access permissions. Authorised access to the ABCD Data Repository is required to obtain ABCD data, hence source data is not shared on this repository.


Repo contains code for analysis of the manuscript in these sections:

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
