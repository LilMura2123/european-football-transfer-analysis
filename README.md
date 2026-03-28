# ⚽ Why Do Some Football Clubs Make Better Transfers Than Others?

Football clubs spend billions in the transfer market every year.  
Yet some consistently build competitive squads, while others struggle — even with similar budgets.

Is success in the transfer market just about money?  
Or do clubs follow fundamentally different strategies?

In this project, we analyze transfer data from major European leagues to uncover **how clubs actually behave in the market** and identify distinct transfer strategies.

---

# 🧠 The Idea

Instead of simply comparing how much clubs spend, this project focuses on a deeper question:

> **How do clubs structure their transfer activity?**

Do they:
- invest in expensive star players?
- rely on low-cost signings?
- build squads through free transfers?

To answer this, we move beyond raw spending and analyze **transfer behavior, efficiency, and decision patterns**.

---

# 📊 Data & Approach

The analysis is based on football transfer data from top European leagues, focusing on transfers since **2022** — a period representing more stable, post-COVID financial conditions.

The workflow follows a structured pipeline:

- data cleaning and preprocessing  
- feature engineering at the club level  
- exploratory data analysis (EDA)  
- clustering using unsupervised learning  

---

# 🏗 Feature Engineering: From Transfers to Strategy

We transform raw transfer data into club-level indicators that capture different aspects of strategy.

### 💰 Financial (paid transfers only)
- total transfer spending  
- average transfer fee  
- log-transformed financial features  

### ⚖️ Efficiency
- **value_ratio_paid** → how much clubs pay relative to market value  

### 🧠 Behavior
- share of free transfers  
- share of expensive transfers (> €40M)  
- share of low-cost transfers (< €15M)  

This allows us to separate:

👉 **how much clubs spend**  
👉 from  
👉 **how they spend**

---

# 🔍 What the Data Reveals

Exploratory analysis shows that:

- financial data is highly skewed — a few clubs dominate spending  
- most clubs rely heavily on low-cost transfers  
- expensive transfers are rare and concentrated among elite teams  
- free transfers play a major role, especially for smaller clubs  

To properly capture these patterns, financial variables are log-transformed, and redundant features are removed.

---

# 🤖 Clustering Football Clubs

We apply **KMeans clustering** to group clubs based on their transfer behavior.

- Elbow Method → suggests k = 3  
- Silhouette Score → confirms k = 3 as optimal  
- Agglomerative clustering → produces consistent results  

👉 This indicates a stable underlying structure in the data.

---

# 🔥 The Result: 3 Transfer Strategies

The analysis reveals **three distinct types of clubs**.

---

## 🔴 Elite High-Spending Clubs

These are the financial giants of football.

**Examples:** Manchester City, PSG, Real Madrid, Bayern Munich, Chelsea  

Characteristics:
- highest transfer spending  
- frequent participation in expensive transfers  
- strong financial power  

👉 These clubs shape the top end of the transfer market.

---

## 🔵 Balanced / Value-Oriented Clubs

Clubs that focus on efficiency rather than big spending.

**Examples:** AC Milan, Roma, Atlético Madrid, Borussia Dortmund  

Characteristics:
- moderate spending  
- strong reliance on low-cost transfers  
- efficient pricing relative to market value  

👉 These clubs optimize resources instead of competing financially with elite teams.

---

## 🟢 Low-Budget / Free-Transfer-Oriented Clubs

Clubs operating under financial constraints.

**Examples:** Roda JC, Reading, Málaga, Guingamp  

Characteristics:
- minimal spending  
- heavy reliance on free transfers  
- no participation in expensive transfers  

👉 Strategy is driven by necessity rather than choice.

---

# 💡 Key Insights

- Transfer strategy is not defined by spending alone — **behavior matters**.
- Expensive transfers are concentrated in a very small group of elite clubs.
- Most clubs operate in a **low-cost transfer environment**.
- Free transfers are a critical tool, especially for lower-budget teams.
- Even clubs with similar budgets can follow very different strategies.

---

# ⚠️ Limitations

This analysis evaluates transfer efficiency **only at the moment of purchase**.

It does not include:
- post-transfer player value changes  
- player performance  
- outgoing transfers (net spend)  

As a result, the project focuses on **transfer behavior and pricing efficiency**, not long-term transfer success.

---

# 🚀 Future Improvements

The analysis could be extended by:

- incorporating player value evolution after transfer  
- adding player-level features (age, position, performance)  
- analyzing net spending (including outgoing transfers)  
- extending the time horizon  
- applying advanced clustering techniques  

---

# 🛠 Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 👤 Author

**Khadzhimurad Khutraev**  

Student interested in data science, machine learning and neural networks.
