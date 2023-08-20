# Portuguese banking institution
### **Task:** Examples represent yes and no instances of Portugese customers who converted and not  after a marketing campaign of phone calls.
### **Trained Model:** 
[Model](https://github.com/Kmohamedalie/Bank-Marketing_Portuguese_Customers/tree/master/Trained%20Model), Training Time: 4h 35min 53s,  Accuracy: 92% but note that 88.7% of the customers never sign up after the phone calls, in marketing terms the conversion/acquisiton rate was very low. So it is better we focus on other metrics such as f1-score, precision and recall since the dataset is imbalanced (88.7 to 11.2).

### **Dataset available on:** [UCI Machine Learning Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing) , [Kaggle](https://www.kaggle.com/datasets/impapan/credit-approval-data-set)

**Developers' Guide:** [Amazon Machine Learning](https://docs.aws.amazon.com/pdfs/machine-learning/latest/dg/machinelearning-dg.pdf#cross-validation)     

**Completed jupyternotebook:** [Bank Marketing Xgboost](https://github.com/Kmohamedalie/Bank-Marketing_Portuguese_Customers-XGBOOST/blob/master/Notebook/Bank_Marketing_Portuguese_Customers_Xgboost.ipynb)



**Metrics:**

| Algorithm | Precision | Recall | F1-score | Accuracy |
|-----------|-----------|--------|----------|----------|
| Xgboost (GridSearchCV)  | 92%       |  92%   | 92%      | 92%    |




![image](https://github.com/Kmohamedalie/Bank-Marketing_Portuguese_Customers/assets/63104472/9dc0797f-60e8-463d-bcf0-1341ad1bc0b9)




## Additional information


- Title: Bank Marketing

- Sources
   Created by: Paulo Cortez (Univ. Minho) and Sérgio Moro (ISCTE-IUL) @ 2012
   
- Past Usage:

  The full dataset was described and analyzed in:

  S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. 
  In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimarães, 
  Portugal, October, 2011. EUROSIS.

- Relevant Information:

   The data is related with direct marketing campaigns of a Portuguese banking institution. 
   The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, 
   in order to access if the product (bank term deposit) would be (or not) subscribed. 

   There are two datasets: 
      1) bank-full.csv with all examples, ordered by date (from May 2008 to November 2010).
      2) bank.csv with 10% of the examples (4521), randomly selected from bank-full.csv.
   The smallest dataset is provided to test more computationally demanding machine learning algorithms (e.g. SVM).

   The classification goal is to predict if the client will subscribe a term deposit (variable y).

- Number of Instances: 45211 for bank-full.csv (4521 for bank.csv)

- Number of Attributes: 16 + output attribute.

- Attribute information:

 -  For more information, read [Moro et al., 2011].

   ## Input variables:
   ### bank client data:<br>
   1 - age (numeric) <br>
   2 - job : type of job (categorical: "admin.","unknown","unemployed","management","housemaid","entrepreneur","student",
                                       "blue-collar","self-employed","retired","technician","services") <br>
   3 - marital : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed) <br>
   4 - education (categorical: "unknown","secondary","primary","tertiary") <br>
   5 - default: has credit in default? (binary: "yes","no") <br>
   6 - balance: average yearly balance, in euros (numeric)  <br>
   7 - housing: has housing loan? (binary: "yes","no")  <br>
   8 - loan: has personal loan? (binary: "yes","no")  <br>
   ### related with the last contact of the current campaign: <br>
   9 - contact: contact communication type (categorical: "unknown","telephone","cellular")  <br>
  10 - day: last contact day of the month (numeric)  <br>
  11 - month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec") <br>
  12 - duration: last contact duration, in seconds (numeric) <br>
   ### other attributes: <br>
  13 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
  14 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted) <br>
  15 - previous: number of contacts performed before this campaign and for this client (numeric) <br>
  16 - poutcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success") <br>

### Output variable (desired target): <br>
  17 - y - has the client subscribed a term deposit? (binary: "yes","no") <br>
- Missing Attribute Values: None
