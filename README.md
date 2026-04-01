
#  Bank Marketing Outcome Prediction

##  Project Overview

This project presents an end-to-end **machine learning pipeline**, starting from Exploratory Data Analysis (EDA) to building and optimizing a **Decision Tree Classifier**.

The objective is to predict whether a customer will subscribe to a **term deposit** based on demographic and behavioral data from the **UCI Bank Marketing Dataset**.



##  Objective

The primary goal of this project is to:

* Analyze customer data to identify patterns influencing subscription decisions
* Build a predictive model to classify potential customers
* Help banks optimize marketing strategies and improve conversion rates



##  Tools & Technologies

* **Language:** Python
* **Environment:** Jupyter Notebook / Jupyter Lab

###  Libraries Used

* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn

  * DecisionTreeClassifier
  * LabelEncoder
  * train_test_split



##  Data Cleaning & Preprocessing

The dataset was prepared using the following steps:

* **Exploratory Data Analysis (EDA):**

  * Used histograms for numerical distributions
  * Count plots for categorical variables

* **Missing Values:**

  * Verified that the dataset contains no null values

* **Outlier Detection & Treatment:**

  * Applied **Interquartile Range (IQR)** method
  * Handled outliers in features like *age, duration, campaign*

* **Feature Encoding:**

  * Converted categorical variables using **LabelEncoder**

* **Correlation Analysis:**

  * Generated heatmap to identify relationships between variables



##  Methodology

* **Data Splitting:**

  * Training and testing split (**80:20 ratio**)

* **Model Selection:**

  * Implemented **Decision Tree Classifier**

* **Hyperparameter Tuning:**

  * Compared **Gini vs Entropy**
  * Controlled model complexity using:

    * max_depth
    * min_samples_split

* **Model Evaluation:**

  * Accuracy Score
  * Classification Report:

    * Precision
    * Recall
    * F1-Score
      
  ##  Decision Tree Analysis

This section visualizes the Decision Tree models built using different splitting criteria.

###  Decision Tree (Gini Index)
- Uses Gini impurity to measure node purity
- Faster computation
- Commonly used default criterion

![Decision Tree - Gini]<img width="1455" height="475" alt="Decision_tree1" src="https://github.com/user-attachments/assets/a67683e7-980a-490a-bd89-774dda6e49d7" />


###  Decision Tree (Entropy)
- Uses Information Gain based on entropy
- More informative but computationally intensive

![Decision Tree - Entropy]<img width="1462" height="487" alt="Decision_tree2" src="https://github.com/user-attachments/assets/e817046a-9b11-46dd-bf2b-a54008c7b70d" />



## Key Insights & Conclusions

* **Call Duration Matters:**
  Longer call duration significantly increases the probability of subscription

* **Economic Indicators Influence Decisions:**
  Features like *euribor3m* and *nr.employed* show strong correlation with outcomes

* **Model Performance:**

  * Training Accuracy: ~91%
  * Strong test performance indicates good generalization



##  What I Learned

* Handling **class imbalance** and understanding precision-recall trade-offs
* Importance of **tree pruning** to prevent overfitting
* How to build interpretable models using Decision Trees
* Using visualizations to explain model decisions to stakeholders



##  Repository Structure

```
├── SCT_DS_3.ipynb     # Jupyter Notebook with full pipeline
├── banking+marketing.zip                 # Dataset files 
└── README.md                # Project documentatio
```


##  Future Improvements

* Apply advanced models (Random Forest, Gradient Boosting)
* Perform feature engineering for improved accuracy
* Build an interactive dashboard (Power BI / Tableau)




## 🎥 Project Demo

[Click here to watch the video]https://github.com/user-attachments/assets/3d0a8545-cc04-4e97-adce-630a4a51f3cc




