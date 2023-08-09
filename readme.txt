Bank data used 
Data Analysis
EDA

Fraud detection is a binary classification task in which any transaction will be predicted and labeled as a fraud or legit. In this Notebook state of the art classification techniques were tried for this task and their performances were compared. :
LogisticRegression()
LinearDiscriminantAnalysis()
KNeighborsClassifier()
RandomForestClassifier()
DecisionTreeClassifier()
XGBClassifier()
GaussianNB()
GradientBoostingClassifier()
LGBMClassifier()
Handled imbalance data with SMOTE
Split 50% data for train and 50 % for test


Adaptive Synthetic Sampling (ADASYN)
Another approach involves generating synthetic samples inversely proportional to the density of the examples in the minority class.
That is, generate more synthetic examples in regions of the feature space where the density of minority examples is low, and fewer or none where the density is high.
This modification to SMOTE is referred to as the Adaptive Synthetic Sampling Method, or ADASYN, and was proposed to Haibo He, et al. in their 2008 paper named for the method titled “ADASYN: Adaptive Synthetic Sampling Approach For Imbalanced Learning.”
ML model
A number of performance metrics could be used to report the performance of the fraud detection classifiers including the confusion matrix, Sensitivity, Specificity, false positive rate, balanced classification Rate and Matthews correlation coefficient.
We just used each algorithm with two approaches of SMOTE
 Simple SMOTE
ADASYN SMOTE
Result : 
Algorithms which  outperformed in term of accuracy
RandomForestClassifier using the SMOTE
RandomForestClassifier using the ADASYN
XGBClassifier using the SMOTE
XGBClassifier using the ADASYN
