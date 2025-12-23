
---

# 📊 Weekly Active Users (WAU) – Growth Accounting Analysis
The analysis applies **Growth Accounting principles** to Weekly Active Users (WAU) data to evaluate user growth health and derive actionable business insights.

---


## 📂 Dataset Overview

* The dataset contains **unique device IDs active in each week**
* Each device can appear in multiple weeks
* Time granularity: **Weekly**
* Objective: Understand *why* WAU grows or declines, not just *whether* it grows

---

## 🧠 Methodology: Growth Accounting

For every week, users are segmented into mutually exclusive buckets:

* **New Users** – First-time active users
* **Retained Users** – Active in both current and previous week
* **Resurrected Users** – Active this week, inactive last week, but active before
* **Churned Users** – Active last week but inactive this week

Growth identity used:

```
WAU(t) = New + Retained + Resurrected
WAU(t-1) = Retained + Churned
```

### Key Metric

* **Quick Ratio = (New + Resurrected) / Churned**

  * Measures whether growth offsets churn

---

## 📈 Analysis & Visualizations

The notebook includes:

* WAU trend over time
* Weekly Growth Accounting bar chart
* Quick Ratio trend
* Retention vs Churn analysis
* Net weekly growth
* Early-life churn analysis
* Contribution analysis (New vs Resurrected)
* Growth health scorecard

All calculations and charts are implemented in a **single Jupyter Notebook**.

---

## 📊 Key Findings (With Numbers)

* **Median Quick Ratio:** ~**0.99** → growth is barely sustainable
* **Median Retention Rate:** ~**72.7%** → core value exists
* **Median Early-Life Churn Ratio:** ~**1.63×** → early churn is high
* **Growth Weeks:** **46.4%** (26 out of 55 weeks)
* **Growth Contribution:**

  * New Users: **63.8%**
  * Resurrected Users: **36.2%**

Nearly **half of all gained users are offset by churn**, creating a leaky growth funnel.

---

## 🏁 Final Conclusion

While the product shows overall growth in Weekly Active Users, Growth Accounting reveals that this growth is **fragile and inefficient**. The business relies heavily on continuous acquisition and resurrection to compensate for persistent churn. Although retention among core users is reasonable (~73%), **early-life churn is the dominant bottleneck**, with the product typically losing **1.6× more users than it gains shortly after onboarding**.

The Quick Ratio hovering around 1 confirms that growth barely offsets losses, and fewer than half of the weeks show net growth. The significant contribution from resurrected users indicates weak habit formation, where users churn before later returning.

**Recommendation:**
The business should prioritize **early retention improvements** over scaling acquisition. Enhancing onboarding, reinforcing first-week value moments, and improving acquisition quality would reduce early churn, lift the Quick Ratio above 1, and enable acquisition and re-engagement efforts to translate into **durable, compounding growth**, signaling stronger product–market fit.

---

## 📎 Repository Contents

* `Rajesh_Kumar_Jena_HealthKart_Assignment.ipynb`
  → Complete analysis with calculations, charts, and insights

---

## 🔗 Submission Links

* **Google Colab:**
  [https://colab.research.google.com/drive/196DcM4hLMDqbgcwTls-QM5l0etimBHRZ?usp=sharing](https://colab.research.google.com/drive/196DcM4hLMDqbgcwTls-QM5l0etimBHRZ?usp=sharing)

* **GitHub Repository:**
  [https://github.com/Rajesh-1234567/Weekly-Active-Users-WAU-Growth-Accounting-Analysis](https://github.com/Rajesh-1234567/Weekly-Active-Users-WAU-Growth-Accounting-Analysis)

---
