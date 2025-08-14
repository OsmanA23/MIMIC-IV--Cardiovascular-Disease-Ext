Abstract—Acute Myocardial Infarction (AMI) is a leading cause
of death worldwide, and early, accurate detection is critical to improving patient outcomes.
Traditional diagnostic approaches often
struggle to leverage large, complex, and unstructured clinical text in
electronic health records (EHRs). This study evaluates BioBERT,
ClinicalBERT, PubMedBERT, and Clinical Longformer for AMI
detection using the Medical Information Mart for Intensive Care
version 4 (MIMIC-IV) Extended Cardiac Dataset under zero-shot
and few-shot prompting. Zero-shot prompting generally matched or
outperformed few-shot performance, with PubMedBERT achieving
the highest AUC of 91.70% and maintaining strong sensitivity
(86.23%) and specificity (81.60%). ClinicalBERT reached an AUC
of 90.55% in zero-shot, and BioBERT achieved 90.05%, both
showing competitive sensitivity and specificity. Clinical Longformer
recorded slightly lower AUCs (84.53% zero-shot, 85.38% few-shot)
but remained balanced across metrics. Based on overall accuracy,
generalization ability, and stability, zero-shot PubMedBERT is
identified as the most suitable model for deployment, highlighting
the potential of domain-specific LLMs to enable early and reliable
AMI detection in clinical decision support systems.

This repository contains Jupyter notebooks for preprocessing and modelling tasks on the MIMIC-IV Extended Cardiac Dataset for Acute Myocardial Infarction (AMI) detection.
The modelling files generally have the same setup and flow, with the difference being the transformer model import and results.

## Files

- MIMIC_IV_Ext_EDA_preprocessing.ipynb  
  Preprocessing and exploratory data analysis (EDA) of MIMIC-IV clinical notes.

- MIMIC_IV_Modelling-BioBERT-main.ipynb  
  Modelling using the BioBERT transformer.

- MIMIC_IV_Modelling-ClinicalBioBERT-main.ipynb  
  Modelling using the ClinicalBERT transformer.

- MIMIC_IV_Modelling-ClinicalLongformer-main.ipynb  
  Modelling using the Clinical-Longformer transformer.

- MIMIC_IV_Modelling-PubMedBERT-main.ipynb  
  Modelling using the PubMedBERT transformer.
