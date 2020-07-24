# Neuro Trends

This project covers assessment of Age and a few other features from static FNC correlation features and sMRI SBM loadings for around 5000
subjects.
This involved understanding the anonymized data using extensive EDA. Once the abnormalities of the data were found, various models were
deployed to assess the desired values.
The variety of models used were:

a. Linear Models (Ridge, Lasso, ElasticNet, Linear Regression)
b. Support Vector Machines ( SVR )
c. Tree Models ( Random Forest )
d. Gradient Boosting ( XGBoost, CatBoost, LightGBM )

Out of these, support vector models and gradient boosting models were trained on an online GPU using Nvidia's Rapids, cudf, cuml etc.
After these rigourous stacking and ensembling of the predictions given by these models was done to achieve competitive results.

This is a mini-project to predict age and other assessment features(d1v1, d1v2, d2v1, d2v2) from the sbm_loadings and fnc_mappings in tabular form.
It can be categorized into:

a. basic_eda

b. experiments

c. stacking_individual ( which contains stacking_tree_models.ipynb, stacking_gbt_models.ipynb, stacking_linear_models.ipynb, stacking_svr_models.ipynb )

d. final_stacking

PS : There are many stacking softwares available like Stacknet, but the stacking had to be done separately for linear models and others because of the gpu requirements.

Also, the data is kept private because of organisation's code of conduct.
