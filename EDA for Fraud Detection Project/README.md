# Exploratory Data Analysis (EDA) for Fraud Detection Project

## 🎯 Goal
The goal of this project is to perform an in-depth exploratory data analysis (EDA) of a transaction dataset to identify potential fraud indicators and uncover trends that can help in detecting fraudulent activities.

## 📌 Overview
This project involves analyzing a dataset containing 10 years of transaction data to perform the following:
1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA) with visualizations
3. High-Risk Client Analysis and Risk Categorization

## 🛠 Tools & Libraries Used
- **Python** – For data cleaning, analysis, and visualization.
- **Pandas** – For data manipulation and cleaning.
- **Matplotlib/Seaborn** – For data visualization and plotting charts.
- **NumPy** – For numerical operations.
- **Jupyter Notebooks** – For performing the analysis and documenting the workflow.

## 📊 Kaggle Dataset
The dataset used for this project can be found at: [Kaggle Transaction Dataset](https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets).

## 🔍 Key Insights & Findings

### 1. Data Understanding & Cleaning
- **Dataset Overview**: The dataset contains 10 years of transaction data, including date, amount, merchant, transaction type, and location.
- **Missing Values**: No missing values were found in the dataset.
- **Duplicates**: No duplicate records were found.
- **Data Type Verification**: 
  - Date column was converted to datetime format.
  - Amount column was converted to float, removing any non-numeric characters.

### 2. Initial Exploratory Data Analysis (EDA)

#### 2.1 Top Merchants by High-Value Transaction Volume
- **Key Observations**:
  - Merchant ID 27092 has the highest transaction volume with a significant $200,000+ gap from others.
  - Other merchants have similar transaction amounts (~$3.5M - $4.5M).
  - Even distribution among the top 10 merchants.

- **Visualization**: Bar chart of top 10 merchants by transaction volume.

#### 2.2 Monthly & Yearly High-Value Transaction Trends
- **Key Observations**:
  - **Monthly**: July has the highest transaction volume, while November & February show major drops in transaction volume.
  - **Yearly**: Transaction volume saw overall growth until 2017, followed by a decline.
  
- **Visualizations**:
  - Line chart showing monthly and yearly trends.

#### 2.3 Merchant-Level Drop Analysis (November & February)
- **Key Observations**:
  - Merchant ID 49637 showed a significant drop in transactions in November & February.
  - Other merchants showed small drops but not as significant.
  
- **Visualization**: Bar chart showing merchant transaction drops.

#### 2.4 Transaction Type Analysis
- **Key Observations**:
  - Swipe and Chip transactions show a decline in November & February.
  - Online transactions remain stable, unaffected by seasonal trends.

- **Visualization**: Stacked bar chart comparing transaction types across months.

#### 2.5 Top Clients by Transaction Volume
- **Key Observations**:
  - Client ID 96 has the highest transaction volume at $3.55M.
  - The top 3 clients significantly outpace others in total transaction value.

- **Visualization**: Bar chart of top 10 clients by transaction volume.

#### 2.6 Unique Cards per Client
- **Key Observations**:
  - Client ID 840 used 6 unique cards, while Client ID 1168 used only 1 card.
  
- **Visualization**: Bar chart showing unique cards per top client.

#### 2.7 Transaction Type Breakdown for Top Clients
- **Key Observations**:
  - Client ID 96 has the highest number of swipe transactions (~23,226).
  - Online transactions are less frequent across all top clients, and chip transactions dominate for some clients.

- **Visualization**: Stacked bar chart comparing transaction type breakdown for top clients.

### 3.0 High-Risk Client Analysis

#### 3.1 High Online Transaction Risk Analysis
- **Key Observations**:
  - 44 clients were identified as high-risk due to an unusually high online transaction ratio.
  - Clients with excessive online transactions could indicate potential fraudulent activities, such as card-not-present fraud.

- **Top 10 High-Risk Clients**:
  - Client IDs 1459, 1812, 1072, and others show high online transaction ratios.
  
- **Visualization**: Bar chart showing high-risk clients based on online transaction ratios.

#### 3.2 Client Risk Categorization
- **Key Observations**:
  - **High-Risk Clients** (70%+ Online Transactions): Client IDs 1558, 1194, and 1684 have high transaction amounts.
  - **Moderate-Risk Clients** (50%-70% Online Transactions): Several clients show moderate amounts, ranging from $26.47 to $55.73.
  - **Low-Risk Clients**: Clients with lower online transaction percentages exhibit lower transaction averages.

- **Visualization**: Bar graph comparing risk categories over distribution of clients.

#### 3.3 Merchant Risk Evaluation
- **Key Observations**:
  - High-Risk Clients buying from the same merchant frequently (e.g., Merchant ID 39021) show high risk exposure.

- **Visualization**: Line chart comparing monthly spending trends for high-risk clients over months.

## 📈 Project Visualizations
- **Top Merchants**: Bar chart of top 10 merchants by transaction volume.
- **Monthly Trends**: Line charts showing high-value transaction trends.
- **Merchant Drop Analysis**: Bar charts showing merchant transaction declines.
- **Risk Analysis**: Visualizations for high-risk client identification and risk categorization.

## 📌 Steps Followed
1. **Data Extraction & Cleaning**: Processed raw transaction data for analysis.
2. **Exploratory Data Analysis**: Uncovered trends, patterns, and anomalies.
3. **Risk Analysis**: Categorized clients and merchants based on transaction behaviors.
4. **Visualization**: Created insights through charts and graphs for better understanding.
