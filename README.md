# BenchmarkingEnsemblesInCCP

Code repository for the paper: 'Bogaert, M., & Delaere, L. (2023). Ensemble Methods in Customer Churn Prediction: A Comparative Analysis of the State-of-the-Art. Mathematics, 11(5), 1137.' 

## Requirements

The code has been built in R (version 4.2.2) and R-studio. All important libraries are loaded in the first code chunk. If the required packages are not installed, make sure that you run `install.packages` first. For `catboost` follow  the guidelines on https://catboost.ai/en/docs/installation/r-installation-binary-installation. For `scmamp` follow the guidelines on https://github.com/b0rxa/scmamp. 

## How to run the code? 

Since the code is a R-markdown file, it is advised that you open the file in R-studio. 

In the paper there are 11 data sets of which 3 are proprietary and 8 publicly available. Since these propietary data sets are confidential, they cannot be shared. Hence, the first 3 data sets in the code should be discarded. The other 8 data sets are online available and can be downloaded from the following links: 
* https://www.kaggle.com/becksddf/churn-in-telecoms-dataset/data# 
* https://www.kaggle.com/shubh0799/churn-modelling 
* https://kdd.org/kdd-cup/view/kdd-cup-2009/Data
* https://www.kaggle.com/barun2104/telecom-churn?select=telecom_churn.csv 
* https://www.kaggle.com/blastchar/telco-customer-churn 
* https://www.kaggle.com/datasets/mahreen/sato2015 
* https://www.kaggle.com/datasets/jpacse/datasets-for-churn-telecom?select=cell2celltrain.csv
* www.sgi.com/tech/mlc/db

To make sure that everyhting runs smoothly, put the data sets in the same directory as the code file. 

Since the paper benchmarks 33 classifiers across all 8 data sets, the code takes very long to run. Users that want to speed up the running time are advised to parallellise the code with `foreach` or run each data set in a different R window. 

## References

Bogaert, M., & Delaere, L. (2023). Ensemble Methods in Customer Churn Prediction: A Comparative Analysis of the State-of-the-Art. Mathematics, 11(5), 1137.

