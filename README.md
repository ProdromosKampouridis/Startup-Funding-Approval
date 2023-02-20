# Startup Funding Approval
Binary classification problem in which based on the values of thirty two different attributes/features, we classify Startups Funding Request into one of two categories (0-Approved, 1-Rejected). The following table contains the aforementioned features as well as a basic description for each one of them.

### About Dataset
The attributes have the following meaning:

| # | Attribure       |  Description                         |              
|---|-----------------|--------------------------------------|
| 1 | ID              | Unique ID of representative |
| 2 | Requested Fund        | Fund amount requested   |
| 3 | Approved Fund          | Fund amount approved   |
| 4 | Invested Fund     | Fund ammount invested     |
| 5 | Term         | Term of fund (in months) |
| 6 | Grade    | Grade by the bank |
| 7 | Interest Rate  | Interest rate (%) on fund |
| 8 | Business Residency | Residential status|
| 9 | Business Duration       | Duration of operation of the business |
| 10 | Verification Status              | Verifying the information provided by a company applicant |
| 11 | Debit to Income              | Ratio of representative's total monthly debt repayment divided by self reported monthly revenues excluding mortgage |
| 12 | Delinquency - two years        | number of 30+ days delinquency in past 2 - years   |
| 13 | Inquires - six months          | Total number of inquiries in last 6 months   |
| 14 | Open Account     | number of open credit line in representative's - credit line     |
| 15 | Public Record         | Number of derogatory public records |
| 16 | Revolving Balance    | Total credit revolving balance |
| 17 | Revolving Utilities  | Amount of credit a representative is using - relative to revolving_balance |
| 18 | Total Accounts | Total number of credit lines available in - representatives credit line|
| 19 | Initial List Status       | Unique listing status of the funding: W(Waiting), F(Forwarded) |
| 20 | Total Received Interest              | Total interest received till date |
| 21 | Total Received Late Fee        | Total late fee received till date   |
| 22 | Total Revolving Credit Limit        | Total Revolving Credit Limit   |
| 23 | Recoveries          | Post charge off gross recovery   |
| 24 | Collection Recovery Fee     | Post charge off collection fee     |
| 25 | Collection 12 months Medical         | Total collections in last 12 months - excluding medical collections |
| 26 | Application Type    | Indicates when the representative is an individual or joint |
| 27 | Last week Pay  | Indicates how long (in weeks) a representative has paid EMI after batch enrolled |
| 28 | Accounts Delinquent | Number of accounts on which the representative is delinquent|
| 29 | Total Collection Amount       | Total collection amount ever owed |
| 30 | Total Current Balance              | Total current balance from all accounts |
| 31 | Payment Plan        | Plan of payment   |
| 32 | Fund Status        | 1 = Defaulter, 0 = Non Defaulters   |





## Basic Code Information
The code has been developped in **python 3.9.13**. To run the code, the requirements.txt file must be used in order to load all the needed modules/packages. Then, through Jupyter Notebook and Pycharm IDE, we can run the code by opening and running the main.py file which is located inside the src folder.

## Repository Structure
The repository structure is simple and self-explanatory. It containts the following folders and files:

**Requirements Folder** - Contains the requirments file in .txt format.

**Presentation folder** - Contains the presentation both in .pptx format.

**Report folder** - Contains the report as .pdf file.

**Data folder** - Contains the data that were used to train the models in .csv format.

**Demo folder** - Contains the report as .pdf file.
| Files/Folders    |  Description                         |              
|------------------|--------------------------------------|
| Demo-Menu.ipynb  | Main file for the demo code |
| data_for_demo.csv| A csv file with two examples |
| transformer.sav  | The saved OneHotEncoder |
| scaler.sav       | The saved StandardScaler |
| pca.sav		 | The saved PCA method |
| cat_model.sav    | CatBoosting saved model |
| etc_model.sav    | Extra Tree Classifier saved model |
| knn_model.sav    | KNN saved model |
| rfc_model.sav    | Random Forest Classifier saved model |
| svm_model.sav    | SVM saved model |
| voting_model.sav | Voting saved model |
| xgb_model.sav    | Xtreme Gradient Boosting saved model |

**src folder** - contains the following files and folders
| Files/Folders         |  Description                         |              
|-----------------------|--------------------------------------|
| Funding_Approval.ipynb| Main file of our source code |
|


## Results
Below we can see the results some of our trained models. More details can be found in the report.
| Classifier        | Accuracy | Precision | Recall | f1    |
|-------------------|----------|-----------|--------|-------|
| Decision Trees    | 0.656    | 0.480     | 0.530  | 0.504 |
| Random Forest     | 0.773    | 0.775     | 0.441  | 0.562 |
| KNN	              | 0.690    | 0.529     | 0.549  | 0.539 |
| Voting Classifier | 0.820    | 1.000     | 0.470  | 0.640 |
