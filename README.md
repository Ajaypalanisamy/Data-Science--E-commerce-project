# 📱 E-Commerce Mobile Phone Market Analysis

## Author
**Ajay Palanisamy**

---

## Table of Contents
1. 📝 Introduction – Overview of project goals and dataset  
2. 🔄 Project Flow – Step-by-step project pipeline  
3. 🌐 Web Scraping – Tools and methods for data collection  
4. 🧹 Data Preprocessing – Cleaning and preparing data  
5. 🧪 Data Cleaning: Before & After – Transformation of raw data  
6. 📊 EDA Process & Market Insights – Data exploration and insights  
7. ⭐ Market Insights: Top Models and Brands – Most popular phones and brands  
8. 💾 SQL Connectivity – Database integration for scalability  
9. 🔍 Unsupervised Learning – Clustering market segments  
10. 🤖 Supervised Learning – Brand classification models  
11. ⚙️ Hyperparameter Tuning: Grid Search – Optimizing model performance  
12. 🏁 Conclusion & Future Work – Summary and next steps  
13. ❓ Questions – Open discussion points  

---

## 📝 Introduction
**Objective:** Execute a **complete data pipeline** for e-commerce mobile phones.  

- **Data Collected:** 1,161 mobile phone records via Web Scraping  
- **Data Cleaning:** Removed duplicates, handled missing values, converted data types  
- **EDA:** Explored market trends, pricing patterns, and customer behavior  
- **Machine Learning:** Built **Price Prediction and Brand Classification Models**  

---

## 🔄 Project Flow
The project consisted of **four main phases**:  

1. **Data Scraping & CSV Creation** – Collect raw data from e-commerce sites  
2. **Data Cleaning & Analysis** – Transform and explore the dataset  
3. **Unsupervised & Supervised Learning** – Identify clusters and predict brands  
4. **Hyperparameter Tuning** – Optimize machine learning models  

---

## 🌐 Web Scraping
- **Tools:** Selenium (browser automation), BeautifulSoup (HTML parsing)  
- **Data Points:** Price, Rating, Title, Number of Reviews  
- **Dataset:** 40 pages scraped → 1,161 records  
- **Storage:** CSV file for further processing  

---

## 🧹 Data Preprocessing
Key steps for preparing data:  

1. **Initial Cleanup:** Remove duplicates, handle missing values  
2. **Feature Engineering:** Extract **Brand** and **Model** from titles  
3. **Data Transformation:** Convert **Price, Rating, Reviews** to numeric types  
4. **Quality Control:** Remove price outliers using **IQR method**  

---

## 🧪 Data Cleaning: Before & After
- **Before:** Mixed text and numbers in columns like Price and Reviews  
- **After:** Clean numeric columns; Brand and Model separated into dedicated columns  

---

## 📊 EDA Process & Market Insights
- **Objective:** Understand market structure, pricing, and customer response  
- **Price Distribution:** Most phones are in lower price ranges; expensive devices form a long tail  
- **Price vs Rating Scatter Plot:** High ratings across all price points  

---

## ⭐ Market Insights: Top Models and Brands
- **Top 10 Brands by Number of Models:** realme, Samsung lead  
- **Top 10 Most Reviewed Models:** Apple iPhone 14 dominates, followed by Motorola  
- **Insight:** Certain models drive **higher customer engagement**  

---

## 💾 SQL Connectivity
- **Purpose:** Centralized access and persistent storage  
- **Tools:** SQLAlchemy ORM  
- **Benefit:** Dataset is **queryable** and **scalable**  

---

## 🔍 Unsupervised Learning
- **Task:** Clustering to discover hidden market segments  
- **Features Used:** Price, Rating, Reviews  
- **Result:** 4 optimal clusters identified  
- **Value:** Enables **targeted marketing** and **strategic positioning**  

---

## 🤖 Supervised Learning
- **Task:** Brand Classification  
- **Input Features:** Price, Number of Reviews  
- **Algorithms Tested:** Random Forest, XGBoost, SVM, K-NN, Logistic Regression  
- **Best Model:** Random Forest (**F1-Score:** 0.7486)  

---

## ⚙️ Hyperparameter Tuning: Grid Search
- **Goal:** Maximize Random Forest model accuracy  
- **Method:** GridSearchCV (parameters: max_depth, n_estimators)  
- **Observation:** Accuracy slightly decreased (0.7561 → 0.7252)  
- **Insight:** Default parameters were robust; tuning may cause slight overfitting  

---

## 🏁 Conclusion & Future Work
- **Achievements:** Full data pipeline executed, from scraping to ML model  
- **Key Findings:**  
  - Market dominated by **specific brands**  
  - **Mid-range pricing** is most common  
- **Future Work:**  
  - Include detailed specs (RAM, Processor)  
  - Explore **Time Series Analysis** for trend forecasting  







