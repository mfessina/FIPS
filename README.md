# FIPS

This repository provides the code implementation for the paper:
> Identifying Key Products to Trigger New Exports: An Explainable Machine Learning Approach https://iopscience.iop.org/article/10.1088/2632-072X/ad3604

that introduces the Feature Importance Product Space.

# Code

The code is organized into three functions: 

- read_csv_from_url(url_files, start_year, last_year): load and clean export data from the repository https://github.com/giamba95/SaplingSimilarity/tree/main/data

- feature_importance(X_train,y_train,X_test,y_test,n_folds,n_rep,n_perm): compute feature importance values and the corresponding null distributions for a Random Forest classifier

- pvalues(gi_imp,gi_perm_imp): compute the p-values to validate feature importance values

Details on the input variables and output of the three functions are reported as comments in the corresponding codes.
