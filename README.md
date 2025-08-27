# ML--Diamond-Price-Analysis-using-Python
# 💎 Diamond Price Analysis & Prediction

## 📌 Project Overview
Diamonds are among the most expensive stones, and their price depends on multiple factors beyond just size.  
In this project, we explore **diamond price analysis and prediction** using Python.  

We analyze attributes such as **carat, cut, color, clarity, depth, table, and size**, and then build a **machine learning model** to predict diamond prices.

---

## 📊 Dataset
The dataset (sourced from [Kaggle](https://www.kaggle.com/)) contains **53,940 rows × 10 features** about diamonds:

- `carat` – Diamond weight  
- `cut` – Quality of the cut (Ideal, Premium, Good, Very Good, Fair)  
- `color` – Diamond color grading (D–J)  
- `clarity` – Clarity grading  
- `depth` – Total depth %  
- `table` – Width of top facet  
- `price` – Price in USD  
- `x, y, z` – Dimensions (mm)  
- `size` – Derived feature (x × y × z)  

---

## 🔎 Exploratory Data Analysis (EDA)
- **Carat vs Price** → Linear relationship (higher carat = higher price).  
- **Size vs Price** → Strong correlation (larger diamonds are more expensive).  
- **Cut & Color vs Price** → Premium cuts and higher color grades are costlier.  
- **Clarity vs Price** → Higher clarity increases price.  
- **Correlation Matrix** shows strong correlation with:
  - Carat (0.92)  
  - Size (0.90)  
  - Dimensions x, y, z (~0.86–0.88)  

---

## 🤖 Machine Learning Model
We trained a **Random Forest Regressor** to predict diamond prices.

### Features Used
- Carat  
- Cut (converted to numerical scale)  
- Size (x × y × z)  

### Steps
1. Preprocessed categorical features (`cut` mapped to numerical values).  
2. Split dataset into **Train (90%) / Test (10%)**.  
3. Trained a **Random Forest Regressor**.  
4. Predicted diamond prices for unseen data.  

### Example Prediction


