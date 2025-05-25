# 🛍️ Mall Customer Segmentation using K-Means Clustering

This project uses K-Means clustering to segment mall customers into distinct groups based on their **spending behavior**, **income**, and **demographic** features. It helps businesses understand customer types for personalized marketing strategies.

---

## 📌 Objective

To segment customers into distinct groups using **unsupervised learning (K-Means)** based on:
- Annual Income
- Spending Score
- Age
- Gender

---

## 📊 Dataset

- **Source**: [Mall Customer Segmentation Dataset on Kaggle](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Columns**:
  - `CustomerID`: Unique ID for each customer
  - `Gender`: Male or Female
  - `Age`: Age of the customer
  - `Annual Income (k$)`: Income in thousands of dollars
  - `Spending Score (1-100)`: Score assigned by the mall based on customer spending behavior

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (KMeans, StandardScaler)

---

## 🧠 Methodology

1. **Data Loading & Cleaning**:
   - Removed `CustomerID`
   - Converted `Gender` to numerical
   - Created new columns: `Annual Income ($)` and `Spender Category`

2. **Feature Scaling**:
   - Standardized features using `StandardScaler`

3. **Elbow Method**:
   - Used to determine the optimal number of clusters (K)

4. **K-Means Clustering**:
   - Applied K-Means with the chosen K (e.g., 5)

5. **Cluster Profiling**:
   - Labeled and interpreted each customer group
   - Added a column for `Segment Name`

6. **Visualization**:
   - Scatter plots for Income vs Spending Score
   - Elbow curve for K selection

---

## 📈 Results

Identified 5 meaningful customer clusters:

| Cluster | Description            | Strategy                             |
|---------|------------------------|--------------------------------------|
| 0       | VIP Customers           | Loyalty rewards, exclusive offers   |
| 1       | Low Value               | Budget deals, reduce ad spend       |
| 2       | Impulsive Buyers        | Flash sales, trending products      |
| 3       | Potential Customers     | Educate, upsell, recommend          |
| 4       | Regular Customers       | Retention offers, engagement emails |

---

## 📷 Visualizations

- 📌 Elbow Method to choose K  
- 📌 Scatter plot (Income vs Spending Score)  
- 📌 Cluster-wise spending behavior  

---

## 📁 Project Structure

