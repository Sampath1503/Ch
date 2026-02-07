# 📊 Telecom Customer Churn Analysis & Prediction

**SQL | Power BI | Machine Learning**

---

## 🔍 Project Overview

Customer churn is a major revenue risk for telecom companies.
This project addresses churn from a **business-first perspective**, combining:

1. **Churn analysis & segmentation** (Why customers churn)
2. **Churn prediction using ML** (Who is likely to churn next)

Instead of jumping directly to machine learning, this project follows how **real companies work**:
👉 *Understand the problem → segment customers → then predict churn.*

---

## 🎯 Business Problem

Telecom companies struggle to:

* Identify **early warning signs** of churn
* Understand **which customers are high-value but at risk**
* Decide **where to focus retention efforts**

The goal is not just to predict churn, but to:

* Explain **why churn happens**
* Identify **actionable customer segments**
* Support **data-driven retention strategies**

---

## 🧠 Real-World Approach (Why This Project Is Different)

Most academic projects:

* Jump straight to churn prediction
* Ignore business context
* Produce scores without actions

**This project follows industry practice:**

```
Churn Analysis → Customer Segmentation → Churn Prediction → Business Action
```

---

## 📁 Project Structure

```
Telecom-Churn/
│
├── churn-analysis-dashboard/
│   ├── PowerBI_Dashboard.pbix
│   └── Screenshots/
│
├── churn-prediction-model/
│   ├── data_preprocessing.py
│   ├── model_training.py
│   ├── evaluation.py
│   └── app.py (Streamlit)
│
├── data/
│   └── telecom_data.csv
│
└── README.md
```

---

## 📊 Part 1: Churn Analysis & Segmentation (SQL + Power BI)

### 🔹 Data Understanding

The dataset contains:

* Customer usage (day / evening / night minutes)
* Billing charges (used as **revenue proxy**)
* Customer service calls
* Plan details (international plan)
* Churn flag (0 = retained, 1 = churned)

> **Note:** Revenue is derived using charge variables, which reflects real telecom billing logic.

---

### 📄 Dashboard Structure

#### **Page 1 – Executive Overview**

**Purpose:** Understand churn impact at a glance

* Total Customers
* Churn Rate (~14%)
* Churned vs Retained distribution
* Initial churn signals

👉 Answers: *“Is churn a problem?”*

---

#### **Page 2 – Behavioral & Financial Drivers**

**Purpose:** Explain *why* churn happens

Key insights:

* Churned customers are **high-usage and high-value**
* Churn increases sharply after **4+ customer service calls**
* International plan users show higher churn
* Churn is driven more by **service experience than low usage**

👉 This page forms the **segmentation logic**

---

#### **Page 3 – Business Insights & Recommendations**

**Purpose:** Translate analysis into actions

**Key churn drivers**

* High customer service calls
* High usage & charges
* International calling plans

**High-risk customer profile**

* 4+ service calls
* High total minutes
* Higher average charges
* Active international plan

**Recommended actions**

* Trigger retention workflows after 3 service calls
* Targeted offers for international plan users
* Early-warning churn flags in CRM

---

## 🧩 Customer Segmentation (Business-Driven)

Instead of clustering blindly, segmentation is based on **actionable business rules**:

### 1️⃣ Service-Based Segmentation

* 0–1 calls → Low risk
* 2–3 calls → Medium risk
* 4+ calls → High risk

### 2️⃣ Value-Based Segmentation

* High usage & high charges → High-value customers
* Low usage & low charges → Low-value customers

### 3️⃣ Plan-Based Segmentation

* International plan users vs non-international users

These segments are:

* Easy to explain
* Easy to implement
* Trusted by business teams

---

## 🤖 Part 2: Churn Prediction (Machine Learning)

After identifying churn drivers and segments, a **churn prediction model** was built.

### 🔹 Model Highlights

* Handled class imbalance using **SMOTE**
* Trained models including **XGBoost**
* Achieved high accuracy and recall on churned customers
* Deployed using **Streamlit** for interactive predictions

### 🔹 Why Prediction Comes Second

Segmentation insights were used to:

* Guide feature selection
* Interpret model outputs
* Align predictions with business actions

> *Prediction prioritizes customers within known risk segments.*

---

## 🔗 How Both Parts Work Together

**Churn Analysis & Segmentation**

* Explains *why* customers churn
* Defines high-risk behavioral patterns

**Churn Prediction**

* Identifies *who* will churn next
* Helps prioritize retention efforts

Together, they form a **complete churn management system**.

---

## 🧠 Key Takeaways

* Churn is driven by **customer experience**, not low usage
* High-value customers are at significant churn risk
* Segmentation is more trusted than black-box models
* Prediction works best **after** understanding behavior

---

## 🛠️ Tools Used

* SQL Server
* Power BI
* Python (Pandas, Scikit-learn, XGBoost)
* Streamlit

---

## 📌 Final Note

This project demonstrates:

* Business-first thinking
* End-to-end analytics workflow
* Practical integration of BI and ML
* Decision-oriented data analysis

---

## 📬 Contact

**Sampath**
Aspiring Data Analyst / Data Scientist
📧 Email: *sampath967610@gmail.com*
🔗 LinkedIn: *www.linkedin.com/in/sampath-kumar-panthagani-2147a6250*

---
