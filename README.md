# Mall Customer Segmentation using K-Means Clustering

An end-to-end data science project utilizing unsupervised machine learning to segment retail mall customers based on their demographic and spending behaviors. This project transitions through data exploration, visual analysis, and multi-dimensional clustering using the K-Means algorithm.

## 📊 Dataset Overview
The dataset used is the popular **Mall Customers Dataset**, which contains target market data gathered through loyalty cards. It includes the following attributes:
*   **CustomerID:** Unique ID assigned to the customer
*   **Gender:** Gender of the customer (Male/Female)
*   **Age:** Age of the customer
*   **Annual Income (k$):** Annual income of the customer in thousands of dollars
*   **Spending Score (1-100):** Score assigned by the mall based on customer behavior and spending nature

## 🛠️ Tech Stack & Dependencies
The analysis was performed entirely inside a Jupyter Notebook environment using the core Python data science stack:
*   **Data Manipulation:** `pandas`
*   **Data Visualization:** `matplotlib`, `seaborn`
*   **Machine Learning:** `scikit-learn` (KMeans, StandardScaler)

## 📈 Key Analysis Phases

### 1. Exploratory Data Analysis (EDA)
*   **Univariate Analysis:** Explored distributions, density profiles (KDE), and outliers via boxplots across `Age`, `Annual Income`, and `Spending Score`.
*   **Bivariate Analysis:** Evaluated the relationship between attributes, isolated correlation statistics through heatmaps, and assessed gender-specific variance across income and spending metrics.

### 2. Machine Learning & Cluster Execution
*   **Univariate Clustering:** Built an introductory 3-cluster model strictly around `Annual Income` zones.
*   **Bivariate Clustering:** Utilized the **Elbow Method** (Inertia minimization curve) to find the mathematical inflection point at **5 optimal clusters** pairing `Annual Income` and `Spending Score`.
*   **Multivariate Clustering:** Explored scaling and dummy encoding categorical variables (`Gender`) using `StandardScaler` for total high-dimensional cluster segmentation.

## 📌 Clustering Insights
The 5 distinct customer groups identified from the primary bivariate analysis include:
1.  **High Income, High Spending (Target Group):** High annual income and high spending parameters.
2.  **High Income, Low Spending (Careful):** High annual income but conservative spending behavior.
3.  **Average Income, Average Spending (Standard):** Middle-class income bracket with moderate spending scores.
4.  **Low Income, High Spending (Careless):** Lower annual income but high propensity to spend.
5.  **Low Income, Low Spending (Sensible):** Lower annual income paired with low spending habits.

## 🚀 Getting Started

### Execution
Launch the Jupyter framework to interact with the code:
```bash
jupyter notebook
```
Open the source notebook file to step through the code execution blocks sequentially. The final output partitions will automatically export into a newly created `Clustering.csv` spreadsheet within your root folder.
