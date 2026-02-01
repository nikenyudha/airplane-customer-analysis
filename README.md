# Airplane Customer Value Analysis

## 📌 Project Overview

This project aims to analyze and segment airline customers to understand their behavior and value. By identifying different customer groups, the airline can develop targeted marketing strategies, improve loyalty programs, and optimize resource allocation.

The analysis uses the **LRFMC Model**, a variation of the traditional RFM (Recency, Frequency, Monetary) model tailored specifically for the aviation industry.

## 📊 Dataset Description

The dataset contains airline customer information including membership details, flight history, and mileage. Key features used for the LRFMC model include:

* **L (Length of Relationship):** `LOAD_TIME` - `FFP_DATE` (How long they have been a member).
* **R (Recency):** `LAST_TO_END` (Days since the last flight).
* **F (Frequency):** `FLIGHT_COUNT` (Total number of flights).
* **M (Mileage):** `SEG_KM_SUM` (Total flight distance).
* **C (Coefficient of Discount):** `avg_discount` (Average discount rate used by the customer).

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** - `Pandas` & `NumPy` for data manipulation.
* `Matplotlib` & `Seaborn` for data visualization.
* `Scikit-learn` for data scaling and K-Means Clustering.



## 🚀 Workflow

1. **Data Cleaning:** Handling missing values, removing duplicate records, and filtering out invalid data (e.g., zero flight distance but non-zero fare).
2. **Feature Engineering:** Creating the L, R, F, M, and C features from the raw data.
3. **Data Transformation:** Standardizing features using `StandardScaler` to ensure all variables contribute equally to the distance calculations.
4. **Modeling:** Applying the **K-Means Clustering** algorithm.
5. **Evaluation:** Using the **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters.
6. **Visualization:** Creating Radar Charts (Spider Plots) to compare the characteristics of each cluster.

## 📈 Key Findings

*(Note: Adjust the number of clusters below based on your specific notebook results)*

* **Cluster 1 (Loyal VIPs):** High frequency, high mileage, and long relationship length.
* **Cluster 2 (New High-Value):** High mileage but relatively new members.
* **Cluster 3 (At-Risk):** High historical value but haven't flown recently (High Recency).
* **Cluster 4 (Low-Value/Occasional):** Low frequency and mileage.

## 💡 Business Recommendations

* **Retain VIPs:** Provide exclusive lounge access and priority boarding.
* **Re-engage At-Risk:** Send personalized "we miss you" emails with discount vouchers for their next flight.
* **Cross-sell to New Members:** Offer bonus points for reaching the next membership tier.


## 👩‍💻 Author
**Niken Larasati**
**(Data Scientist & Writer)**

* [GitHub](https://www.google.com/search?q=https://github.com/nikenyudha)
* [LinkedIn](https://www.google.com/search?q=INSERT_YOUR_LINKEDIN_HERE)
