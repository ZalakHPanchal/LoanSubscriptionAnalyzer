# LoanSubscriptionAnalyzer

This project basically uses a banking dataset and it helps us to estimate the success of marketing phone calls for selling long-term bank deposits.


Datasource:

https://archive.ics.uci.edu/ml/datasets/bank+marketing


# The dataset has the following features:
 - age (numeric)
 - job : type of job (categorical: "admin.","blue-collar","entrepreneur","housemaid","management","retired","self-employed","services","student","technician","unemployed","unknown")
 - marital : marital status (categorical: "divorced","married","single","unknown"; note: "divorced" means divorced or widowed)
 - education (categorical: "basic.4y","basic.6y","basic.9y","high.school","illiterate","professional.course","university.degree","unknown")
 - default: has credit in default? (categorical: "no","yes","unknown")
 - housing: has housing loan? (categorical: "no","yes","unknown")
 - loan: has personal loan? (categorical: "no","yes","unknown")
 - contact: contact communication type (categorical: "cellular","telephone") 
 - month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
 - day_of_week: last contact day of the week (categorical: "mon","tue","wed","thu","fri")
 - duration: last contact duration, in seconds (numeric). Important note:  this attribute highly affects the output target (e.g., if duration=0 then y="no"). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
 - previous: number of contacts performed before this campaign and for this client (numeric)
 - poutcome: outcome of the previous marketing campaign (categorical: "failure","nonexistent","success")
 - emp.var.rate: employment variation rate - quarterly indicator (numeric)
 - cons.price.idx: consumer price index - monthly indicator (numeric)     
 - cons.conf.idx: consumer confidence index - monthly indicator (numeric)     
 - euribor3m: euribor 3 month rate - daily indicator (numeric)
 - nr.employed: number of employees - quarterly indicator (numeric)

 Output variable (desired target):
 - y - has the client subscribed a term deposit? (binary: "yes","no")


# Operations:
    - Some of the feature have missing values;it is handling by the dropping missing values with a rows(dropna).
    
    - splitting the dataset(70:30;70% in train and 30% in test)
    
    - For the binary classification, the following linear and non-linear machine learning approaches were attempted: Decision Tree Classification, Logistic regression, Linear   Discriminative Analysis, K-nearest neighbor, Support Vector Machine(SVM and kernel-SVM).
    
    
