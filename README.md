# SpaceX Falcon 9 Landing Prediction & Launch Analysis

## Overview

This project is the IBM Applied Data Science Capstone project, focused on analyzing SpaceX Falcon 9 launch data to predict first-stage landing success.

It implements a complete end-to-end data science pipeline, including data collection, wrangling, exploratory analysis, machine learning modeling, and interactive visualization.

---

## Problem Statement

SpaceX reduces launch costs by reusing the Falcon 9 first-stage booster. Predicting whether the booster will land successfully is critical for estimating mission cost and reliability.

This project aims to:

* Analyze historical launch data
* Identify key factors influencing landing success
* Build machine learning models to predict landing outcomes
* Enable interactive exploration of launch performance

---

## Project Workflow

### 1. Data Collection

* Extracted data from SpaceX REST API
* Performed web scraping to gather additional information
* Combined multiple sources into a structured dataset

---

### 2. Data Wrangling

* Cleaned missing and inconsistent data
* Engineered features such as payload mass, orbit type, and booster characteristics
* Prepared dataset for analysis and modeling

---

### 3. Exploratory Data Analysis (EDA)

* Analyzed relationships between:

  * Launch site
  * Payload mass
  * Booster version
  * Orbit type
* Identified patterns affecting landing success

---

### 4. Data Visualization

* Used Matplotlib and Seaborn for statistical plots
* Used Folium for geospatial visualization of launch sites
* Identified location-based performance trends

---

### 5. Machine Learning Modeling

Built and evaluated multiple classification models to predict landing success.

#### Approach:

* Standardized features using `StandardScaler`
* Split data into training and testing sets (80/20)
* Performed hyperparameter tuning using `GridSearchCV`

#### Models Implemented:

* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree
* K-Nearest Neighbors (KNN)

#### Results:

* All models achieved ~83% test accuracy
* Decision Tree achieved highest validation accuracy (~89%)
* Models were able to distinguish landing outcomes effectively

#### Evaluation:

* Confusion matrix analysis revealed some false positives
* Compared model performance to select best approach

---

### 6. Interactive Dashboard

Developed an interactive dashboard using Plotly Dash for dynamic exploration of launch data.

#### Features:

* Filter by launch site and payload range
* Visualize success rates across launch sites
* Compare successful vs failed launches
* Analyze payload mass vs mission outcome
* View booster version performance

---

## Key Insights

* Launch site significantly impacts success probability
* Payload mass influences landing success
* Booster reuse and version affect reliability
* Success rates improve over time with operational experience

---

## Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Folium
* Scikit-learn
* Plotly & Dash

---

## How to Run the Dashboard

```
pip install pandas dash plotly
python spacex_dash_app.py
```

Open in browser:

```
http://127.0.0.1:8050/
```

---

## Future Improvements

* Deploy the dashboard for public access
* Improve model performance with advanced techniques
* Add time-series analysis of launch trends
* Enhance UI/UX for better interactivity

---

## Conclusion

This project demonstrates a complete data science workflow, from raw data acquisition to machine learning modeling and interactive visualization. It highlights the use of data-driven techniques to solve real-world prediction problems.

---
