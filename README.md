# Premier-League-Match-Prediction-Project

**Premier League 2024-25 Season : Match Outcome Prediction**

A comprehensive machine learning project that predicts Premier League match outcomes using multiple classification algorithms. This project demonstrates the complete ML pipeline from data preprocessing to model development.

**Overview** : This project tackles the challenging Premier League match outcomes (Win/Draw/Loss) using team performance statistics. The project implements and compares five machine learning algorithms:

**> Logistic Regression** - Linear probabilistic classifier

**> Decision Tree** - Rule-based classifier

**> Random Forest** - Ensemble of decision trees

**> Support Vector Machine** - Margin-based classifier

**> Voting Classifier** - Ensemble of multiple diverse models



**Key Features** 

~ Complete data preprocessing

~ Comprehensive exploratory data analysis (EDA)

~ Advanced feature engineering

~Multiple ML model implementation 

~ Hypererparameter tuning with GridSearchCV

~ Feature importance analysis

~ Professional visualization



**Dataset Information** : The dataset contains Premier League 2024-25 season match data with the features such as 
HomeTeam/AwayTeam

~ full-time home/away goals (FTHG/FTAG)

~full-time result (H/D/A)

 and the performance metrics are such as

~ home/away shots (HS/AS)

~ home/away shots on target (HST/AST)

~ home/away corners (HC/AC)

~ home/away fouls (HF/AF)

~ home/away yellow cards (HY,RY)

~ home/away red cards (HR/AR)





**Engineered Features** : 

~ Shooting Accuracy Metrics

~ Dominance Indicators

~ Shot Efficiency

~ Discipline Metrics

~ Foul Balance





**Methodology** 

 **- Data Preprocessing**
1. Missing value handling with median imputation
2. Duplicate removal and data type correction
3. Outlier detection and treatment with log transformation

**- Feature Engineering**
1. Created 16 features from raw statistics
2. Shot-based features (accuracy, efficiency)
3. Dominance indicators (shots,corners)
4. Discipline metrics (cards, fouls)


**- Multicollinearity Handling**
~ Correlation analysis to check if if there is correlation of features with |r| > 0.8
but there is no multicollinearity.

**- Model Training & Evaluation**
1. 70-30 train-test split with stratification
2. 5-fold cross-validation for robust evaluation
3. StandardScaler for linear models (LR, SVM)
4. Hyperparameter tuning potential for future work






**Key Insights**

1. Random Forest achieved the best performance with 61% accuracy
2. Home advantage is significant (40.7% homw wins vs 34.73% away wins)
3. Shooting accuracy and shot aefficiency are the most predictive features
4. Total shots and total goals show strong correlation with match outcomes







**Technology Stack**

Python 3.13.7

pandas - Data manipulation

numpy - Numerical computing

matplotlib/seaborn - Data visualization

scikit-learn - Machine learning




**Visualizations**

This project generates comprehensive visualizations including:

1. Match results distribution
2. Home vs away goals kernel density estimation
3. Home advantage analysis
4. Shots and goals correlation scatter plots
5. Corner Distribution
6. Cards distribution
7. Correlation heatmap
8. Boxplot for extreme values
9. Log-transformed distribution
10. Confusion matrices for best models
11. Feature importance rankings
12. Model performance comparison bar charts


**Key Learnings**

1. Domain Knowledge - Understanding football statistics significantly improves feature engineering.
2. Feature Engineering - Created features often outperform raw statistics.
3. Class Imbalance - Football match outcomes are naturally imbalanced (more home wins).
4. Model Selection - Ensemble methods (Random Forest, following with voting classifier with 58% accuracy) perform best for this type of data.
5. Evaluation - Cross-validation is crucial for reliable performance estimates



