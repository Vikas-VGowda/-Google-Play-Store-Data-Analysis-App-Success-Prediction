# Google Play Store Data Analysis & App Success Prediction

##  Project Overview

The Google Play Store contains a vast collection of applications across various categories, making it difficult to identify what drives app success. This project performs an end-to-end data analysis and machine learning workflow to understand app patterns and predict whether an app will achieve high installs.

The project combines data cleaning, exploratory data analysis (EDA), visualization, and machine learning to derive meaningful insights from Play Store data.

##  Objectives

- Understand the distribution of apps across categories  
- Perform exploratory data analysis (EDA) with insights  
- Analyze trends in ratings, installs, pricing, and app size  
- Build and evaluate a machine learning model to predict high-install apps  
- Extract meaningful business insights from the dataset  

## Dataset

- Source: Google Play Store Dataset  
- Records: ~10,000+ apps  
- Features: App, Category, Rating, Reviews, Size, Installs, Price, Genres, Content Rating  
- Target Variable: High_Install (1 if installs ≥ 1M, else 0)  

##  Exploratory Data Analysis (EDA)

### Key insights:

- Most apps have ratings between **4.0–4.5**  
- Categories like **Family, Game, and Tools dominate**  
- Strong correlation between **Reviews and Installs**  
- Majority of apps are **free or low-priced**  
- User sentiment is largely **positive**  

EDA was supported with visualizations and business-focused interpretations.

##  Machine Learning Approach

###  Models Implemented

- Random Forest Classifier  
- Logistic Regression  

###  Key Techniques

- Handling missing values and data cleaning  
- Feature engineering:
  - Size conversion (Size_MB)  
  - Install categorization  
- Feature scaling (StandardScaler)  
- Train-test split with stratification  

##  Model Performance

- Logistic Regression Accuracy: **~81.78%**  
- Random Forest Accuracy: **~95.23%**  
- Random Forest shows better precision, recall, and overall performance  
- Balanced predictions with minimal misclassification  

##  Feature Importance

Key factors influencing app success:

- **Reviews** → Strong indicator of installs  
- **Rating** → Reflects app quality and user satisfaction  
- **Size** → Minor impact on installs  
- **Price** → Limited influence  

These features play a crucial role in predicting high-install apps.

##  Business Usage

This project can help developers and businesses to:

- Predict whether an app will achieve high installs  
- Improve app quality and user engagement  
- Optimize pricing strategies  
- Identify competitive and less saturated categories  

##  Limitations

- Based on a static dataset (not real-time data)  
- Limited features (no user behavior or retention data)  
- Model does not capture external factors like marketing  
- Predictions should assist decisions, not replace them  

##  Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- SciPy (stats)  
- Scikit-learn  

##  Repository Contents

- play_store_Analysis.ipynb → Complete analysis and ML model  
- googleplaystore.csv → Dataset used
- googleplaystore_user_reviews.csv→ Dataset used
- README.md → Project documentation  

##  Author

**Vikas Gowda V**  
Aspiring Data Analyst / Data Scientist  

##  Conclusion

This project demonstrates a complete data analysis and machine learning workflow on Google Play Store data. By combining EDA with predictive modeling, it provides valuable insights into app success factors and supports data-driven decision-making.
