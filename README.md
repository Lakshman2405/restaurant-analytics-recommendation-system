# Restaurant Analytics and Recommendation System

## Overview
The restaurant industry generates large volumes of heterogeneous data including location, pricing, cuisine types, services, and customer feedback. The challenge is to convert this raw data into meaningful insights that help understand restaurant performance and recommend suitable restaurants based on user preferences.

This project presents an end-to-end **Data Science solution** that performs data cleaning, exploratory analysis, predictive modeling, classification, and content-based recommendation using restaurant data.

---

## Objectives
- Clean and normalize raw restaurant data for consistent downstream analysis
- Analyze restaurant patterns across locations, pricing, and services
- Predict restaurant ratings using regression models
- Classify restaurant cuisines using supervised machine learning
- Build a content-based restaurant recommendation system

---

## Dataset Cleaning (Preprocessing Pipeline)
- Removed encoding issues and byte-order marks from column names
- Normalized multilingual categorical text using Unicode normalization
- Removed non-Latin and special characters from text fields
- Generated a reusable cleaned dataset for all modeling tasks

---

## Module 1: Exploratory & Location-Based Analysis
- Analyzed geographical distribution of restaurants across countries and cities
- Studied patterns in ratings, pricing, votes, and service availability
- Identified high-density and high-rating restaurant regions

---

## Module 2: Restaurant Rating Prediction (Regression)
- Built a regression model to predict aggregate restaurant ratings
- Engineered features including votes, pricing, services, cuisine flags, and country information
- Applied target encoding for country to avoid high cardinality
- Evaluated model using RMSE and R² score
- Performed feature influence analysis using model coefficients

**Techniques:** Linear Regression, Feature Engineering, Target Encoding

---

## Module 3: Cuisine Classification (Multi-Class Classification)
- Framed cuisine identification as a multi-class classification problem
- Handled class imbalance by filtering rare cuisines
- Trained a Random Forest classifier with stratified train-test split
- Evaluated performance using accuracy, precision, recall, and F1-score
- Performed hyperparameter tuning using GridSearchCV
- Analyzed model limitations and identified feature coarseness as the root cause

**Key Insight:** Numerical features alone are insufficient for fine-grained cuisine classification

---

## Module 4: Restaurant Recommendation System
- Designed a content-based recommendation system using cosine similarity
- Engineered numerical, binary, and one-hot encoded categorical features
- Applied MinMax scaling prior to similarity computation
- Recommended restaurants based on cuisine, price range, services, ratings, popularity, and location
- Validated recommendations across multiple real-world user preference scenarios

---

## Tools & Technologies
- **Programming:** Python
- **Libraries:** pandas, NumPy, scikit-learn, matplotlib, seaborn
- **Techniques:** Regression, Classification, Feature Engineering, Recommendation Systems

---

## Key Learnings
- Importance of data cleaning and encoding in real-world datasets
- Handling categorical variables and class imbalance
- Avoiding data leakage during feature encoding
- Understanding model limitations and proposing data-driven improvements

---

## Future Improvements
- Apply TF-IDF or word embeddings on cuisine text for improved classification
- Introduce hybrid recommendation (content + popularity-based)
- Deploy the recommendation system as a web application

