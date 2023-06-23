# Project-3-H1N1
# Description
  The past few years have shed a light on the effectiveness of vaccines and the reluctance of participants in receiving a vaccine. To help learn which demographics are more likely to get vaccinated and which methods would be best used to increase participation. It is improtant to learn from the past, in particular, to look at the H1n1 crisis from 2009 to 2010. By analyzing this information one can best understand which groups to advertise towards and which advertisements groups would be the least effective. 
# Import of relevants packages
  import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.linear_model import LogisticRegression
from sklearn.linear_model import LinearRegression
from sklearn import preprocessing
from sklearn.preprocessing import OneHotEncoder
from sklearn.preprocessing import OrdinalEncoder
from sklearn.preprocessing import LabelEncoder
from sklearn.preprocessing import StandardScaler, OneHotEncoder, MaxAbsScaler
from sklearn.metrics import roc_curve, auc
from sklearn.metrics import r2_score
from sklearn.metrics import accuracy_score, recall_score, precision_score, f1_score
from sklearn.model_selection import train_test_split
from sklearn.model_selection import cross_val_score, KFold
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.tree import DecisionTreeClassifier
from sklearn.tree import DecisionTreeRegressor
from sklearn.pipeline import Pipeline
from sklearn.neighbors import KNeighborsClassifier
from sklearn.ensemble import BaggingClassifier, RandomForestClassifier,\
ExtraTreesClassifier, VotingClassifier, StackingRegressor
from sklearn.impute import SimpleImputer
from sklearn.neighbors import KNeighborsRegressor
from sklearn.compose import ColumnTransformer
from imblearn.over_sampling import SMOTE
from imblearn.pipeline import Pipeline
# Formation of Pipelines with different classification models
<img width="231" alt="Screen Shot 2023-06-23 at 11 27 38 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/3286e19c-2a7f-48b2-93c1-87f557f5bfec">
Logistic Regression 


<img width="334" alt="Screen Shot 2023-06-23 at 11 27 50 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/969b6326-10b7-4645-a69d-2ba8db622196">
Decision Tree with Bagging 


<img width="324" alt="Screen Shot 2023-06-23 at 11 28 12 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/cf1e263d-8812-4bb7-9bac-1185c269a2ea">
Random Forest Classification 

# Looking at which confusion Matrixes produced the most accurate results
<img width="487" alt="Screen Shot 2023-06-23 at 11 32 32 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/2d0f296a-8d58-46d2-aa1d-d29e10f6da50">
Logistic Regression 


<img width="429" alt="Screen Shot 2023-06-23 at 11 32 39 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/5b6b77dc-09fc-4855-846c-0fb33a3dab38">
Decision Tree


<img width="447" alt="Screen Shot 2023-06-23 at 11 32 45 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/3c92694b-ee1c-408f-96bc-d0452b3db420">
Random Forest Classifier

# Analyzing the results 
The best predictive model was the random forest classifier, using smote and a grid search to find the optimal parameters. In order to further test the effectiveness of this model, it was tested on a ROC curve. 
<img width="443" alt="Screen Shot 2023-06-23 at 11 28 22 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/f4e8662b-52e8-4048-a866-54302b33e759">

# Identifying Feature Importances 
<img width="646" alt="Screen Shot 2023-06-23 at 11 28 06 AM" src="https://github.com/justinlapidus25/Project-3-H1N1/assets/130884190/8674e9dd-8b53-4d40-b686-a56fa3076672">
The most important features are; age, education, and number of children 
The least important features are; race, sex, and income disparity

# Reccomendations 

1) Focus on increasing advertisements towards educational centers, in particular elementary and pre school settings. Push the narrative of protecting the future.
2) Avoid Race and sex-specific advertisements since they are not a good indicator of who is being administered the vaccine. 



