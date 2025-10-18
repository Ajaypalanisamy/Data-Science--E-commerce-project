# E-Commerce Mobile Phone Market Analysis

## Author
**Ajay Palanisamy**

---

## Table of Contents
1. [Introduction]
2. [Project Flow]
3. [Web Scraping]
4. [Data Preprocessing]
5. [Data Cleaning: Before & After]
6. [EDA Process & Market Insights]
7. [Market Insights: Top Models and Brands]
8. [SQL Connectivity]
9. [Unsupervised Learning]
10. [Supervised Learning]
11. [Hyperparameter Tuning: Grid Search]
12. [Conclusion & Future Work]
13. [Questions]

---

## Introduction
The main objective of this project was to execute a **complete data pipeline**.  

- **Data Collected:** 1,161 mobile phone records via Web Scraping  
- **Data Cleaning:** Removed duplicates, handled missing values, converted data types  
- **EDA:** Explored market trends, pricing patterns, and customer behavior  
- **Machine Learning:** Developed a **Price Prediction and Brand Classification Model** optimized via **Hyperparameter Tuning**

---

## Project Flow
The project consisted of **four main phases**:

1. **Data Scraping & CSV Creation**  
2. **Data Cleaning & Analysis**  
3. **Unsupervised & Supervised Learning**  
4. **Hyperparameter Tuning**  

---

## Web Scraping
- Tools: **Selenium** (browser automation), **BeautifulSoup** (HTML parsing)  
- Data Points Collected: **Price, Rating, Title, Number of Reviews**  
- Scraped **40 pages** resulting in **1,161 records**  
- Data stored in a **CSV file** for further processing

---

## Data Preprocessing
Key steps for preparing data:

1. **Initial Cleanup:** Remove duplicates, handle missing values  
2. **Feature Engineering:** Extract **Brand** and **Model** from product titles  
3. **Data Transformation:** Convert **Price, Rating, Reviews** into numeric types  
4. **Quality Control:** Remove price outliers using **IQR method**

---

## Data Cleaning: Before & After
- **Before:** Mixed text and numbers in columns like Price and Reviews; single Title column  
- **After:** Clean numeric columns for Price, Rating, Reviews; Brand and Model separated into dedicated columns  

---

## EDA Process & Market Insights
- **Objective:** Understand market structure, pricing behavior, and customer response  
- **Price Distribution:** Majority of phones in lower price ranges; long tail for expensive devices  
- **Price vs Rating Scatter Plot:** High ratings across all price points; very high prices mostly correspond to high ratings  

---

## Market Insights: Top Models and Brands
- **Top 10 Brands by Number of Models:**  
  - **realme** leads, followed by **Samsung**  
- **Top 10 Most Reviewed Models:**  
  - Dominated by **Apple iPhone 14** and **Motorola models**  
- Insight: Certain models drive **higher customer engagement** in reviews

---

## SQL Connectivity
- **Purpose:** Data persistence and centralized access  
- **Tools:** **SQLAlchemy ORM**  
- Ensures clean dataset is **queryable** and **scalable** for future analyses

---

## Unsupervised Learning
- **Task:** Clustering to discover hidden market segments  
- **Features Used:** Price, Rating, Reviews  
- **Result:** **4 optimal clusters** identified  
- **Value:** Helps in **targeted marketing** and **strategic product positioning**

---

## Supervised Learning
- **Task:** Brand Classification  
- **Input Features:** Price, Number of Reviews  
- **Algorithms Tested:** Random Forest, XGBoost, SVM, K-NN, Logistic Regression  
- **Best Model:** Random Forest  
  - **F1-Score:** 0.7486  

---

## Hyperparameter Tuning: Grid Search
- **Goal:** Maximize accuracy of Random Forest model  
- **Method:** GridSearchCV (parameters tested: max_depth, n_estimators)  
- **Observation:** Accuracy slightly decreased from **0.7561 → 0.7252**  
- **Insight:** Default parameters were robust; tuning may have caused slight overfitting

---

## Conclusion & Future Work
- **Achievements:** Completed full data pipeline from Web Scraping to ML Model optimization  
- **Key Market Findings:**  
  - Mobile market dominated by **specific brands**  
  - **Mid-range pricing** is most common  
- **Future Work:**  
  - Include more detailed specs (RAM, Processor)  
  - Explore **Time Series Analysis** for trend forecasting  




