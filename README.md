# ⚽ Football Transfer Market Analysis

This project analyzes **football transfer strategies across major European leagues** using Python and machine learning techniques.

The goal of the analysis is to understand **how clubs behave in the transfer market** and identify different strategic patterns in player acquisitions.

The study focuses on transfers starting from **2022**, representing the post-COVID period when football clubs returned to more stable financial conditions.

---

# 🎯 Project Goal

The main objective of this project is to explore patterns in football transfers and analyze how clubs approach the transfer market.

Key questions addressed in this analysis:

- Which clubs spend the most on transfers?
- How many players do clubs typically sign?
- Do clubs tend to overpay relative to market value?
- What different transfer strategies exist across clubs?

To answer these questions, the project applies **data analysis and unsupervised machine learning techniques**.

---

# 📊 Methodology

The analysis includes several steps:

### Data Processing
- cleaning the dataset
- handling missing values
- filtering leagues and time periods

### Feature Engineering
Several indicators describing transfer strategies were created:

- total transfer spending
- number of signed players
- average transfer fee
- total market value of players
- difference between market value and transfer spending

### Exploratory Data Analysis (EDA)

Visualizations were used to explore the dataset:

- transfer spending distribution
- top spending clubs
- average transfer fees
- feature distributions

### Clustering Analysis

Unsupervised machine learning was used to identify **groups of clubs with similar transfer strategies**.

The following models were tested:

- **KMeans**
- **Agglomerative Clustering**
- **DBSCAN**

The optimal number of clusters was determined using:

- Elbow Method
- Silhouette Score

---

# 🧠 Key Findings

The analysis reveals that football clubs follow **distinct transfer market strategies**.

Some clubs spend aggressively and frequently sign expensive players, while others rely on **efficient scouting and player development**.

Clustering analysis shows that clubs can be grouped into different strategic categories based on their spending behavior and transfer efficiency.

---

# 🛠 Technologies Used

The project was implemented using the following tools:

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Joblib**

---

# 📁 Project Structure

project/
│
├── notebooks/
│ └── transfer_market_analysis.ipynb
│
├── data/
│ └── dataset description
│
├── images/
│ └── visualizations
│
└── README.md


---

# 🚀 Possible Improvements

Future extensions of the project may include:

- incorporating more seasons of transfer data
- adding player performance metrics
- analyzing club financial indicators
- applying more advanced clustering techniques
- building predictive models for transfer success

---

# 👤 Author

**Khadzhimurad Khutraev**

Data analysis and machine learning project focused on **football analytics and transfer market behavior**.
