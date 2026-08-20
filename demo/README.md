### Instructions for demo
Download mock data files and and code scripts, then run code files in below order:

1. SOM and psychopathology profile development (SOM_mock.ipynb)
- Training and validation of SOM
- Clustering and alternative assessment of SOM topology - psychopathology profiles
- Overlap with diagnostic burden
Expected output: trained SOM object and visualisation (som.p), visualisation of overlap with diagnostic burden, psychopathology profiles significant after permutation (significant_islands_report_mock.json), assignment of participants to psychopathology profiles (som_island_membership.csv)

2. Stability over follow-up time points (SOM-followup_mock.ipynb)
Expected output: correlation between distance vector to profiles at baseline and at follow-up timepoints

3. Resting-state fMRI PLS Analysis (PLS-rsFC_mock.ipynb)
Expected output: PLS Correlation model of behaviour and brain connectivity (pls_membership_mock.joblib), visualisation of behavioural and brain loadings, visualisation of shared and unique edges, post-hoc GLM of confounds

4. Polygenic Risk Score PLS Analysis (PLS-PGR_mock.ipynb)
Expected output: PLS Correlation model of behaviour and polygenic risk scores (pls_gene_mock.joblib), visualisation of behavioural and brain loadings, correlation between PLS-rsFC and PLS_PGR, post-hoc GLM of confounds

5. Edge-type Analysis - Rich, Feeder and Local connections (PLS-richclub_mock.ipynb)
Expected output: connection types across fMRI matrices

6. AHBA gene expression x Psychopathology connectivity PLS (Gene_annotation_mock.ipynb)
Expected output: list of genes from encoding (GWAS) (genelist_gwas_clean.txt) and regional expression (AHBA atlas) (genelist_abagenleft_clean.txt) for input into gene ontology analysis

Expected demo run time: ~10 minutes.
Mock datasets, a trained SOM and classifier, and intermediate data processing files are provided.
Note that all data in the demo is was generated randomly from normal/binomial distributions and does not have any affiliation with ABCD data. Participant pseudoidentifiers and associated data do not in any way correspond to real participants.
