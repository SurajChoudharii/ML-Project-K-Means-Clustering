## ✈️ Airlines Customer Segmentation - K-Means Clustering Project

This project applies **K-Means Clustering** to segment airline customers based on their mileage and transaction history. The goal is to help the airline **identify customer groups** for targeted marketing, loyalty programs, and strategic decision-making.

---

### 📁 Dataset Overview

The dataset `EastWestAirlines.csv` contains frequent flier data, with features like:

* **Balance**: Miles eligible for award travel
* **Qual\_mile**: Qualifying miles for elite status
* **cc1\_miles / cc2\_miles / cc3\_miles**: Miles earned from different credit cards
* **Bonus\_miles / Bonus\_trans**: Non-flight bonuses and transactions
* **Flight\_miles\_12mo / Flight\_trans\_12**: Flight activity in the last year
* **Days\_since\_enrolled**: Loyalty duration
* **Award**: Indicates if the user received a free flight

---

### 🎯 Objective

* Find the **optimal number of customer clusters**
* Segment customers into meaningful groups
* Analyze behavioral patterns in each group
* Recommend **data-driven strategies** for each segment

---

### 🛠️ Tools & Libraries

* **Python**, **Pandas**, **NumPy**
* **Scikit-learn** (KMeans, PCA, StandardScaler)
* **Matplotlib**, **Seaborn**

---

### 🧪 Steps Performed

1. **Data Preprocessing**

   * Removed irrelevant columns (like ID)
   * Scaled data using `StandardScaler`

2. **Finding Optimal Clusters**

   * Applied the **Elbow Method** using WCSS

3. **Modeling**

   * Used **KMeans Clustering** to segment data
   * Tested for multiple cluster counts (e.g., k=3 to k=6)

4. **Cluster Analysis**

   * Grouped data by clusters
   * Analyzed `Bonus_trans`, `Flight_miles_12mo`, `Flight_trans_12`, `Days_since_enrolled`, and `Award`
   * Created PCA plot to visualize clusters

5. **Business Inference**

   * Identified loyal customers, new members, and high-spenders

---

### 📊 Cluster Insights 

| Cluster | Behavior                      | Award Ratio | Strategy                    |
| ------- | ----------------------------- | ----------- | --------------------------- |
| 0       | Loyal customers, high mileage | High        | Maintain with rewards       |
| 1       | New customers, low activity   | Low         | Offer incentives & bonuses  |
| 2       | Mid-tier, moderate engagement | Medium      | Target with upgrade options |

---

### 📌 How to Run

1. Install dependencies:

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

2. Open the notebook:

   ```
   ML-Project-K-Means-Clustering.ipynb
   ```

3. Run all cells and observe the summary, visualizations, and final inferences.

---

### ✅ Deliverables

* ✅ Cleaned Dataset
* ✅ Elbow plot to select `k`
* ✅ KMeans clustering model
* ✅ PCA visualization
* ✅ Business inferences for each cluster

---

### 🧠 Conclusion

This project demonstrates how clustering techniques can be used to uncover hidden patterns in customer behavior, enabling more personalized and profitable airline services.
