# 🏗️ System Architecture Overview

## **1. Data Sources**

The project integrates **two primary data sources**:

- **Wikipedia Scraping**: Extracts Best Picture winners and metadata (title, year, genre).
- **Kaggle Dataset**: Provides structured Oscar award data across multiple categories.

These sources ensure comprehensive coverage of **Oscar-winning movies**, reducing reliance on a single dataset.

---

## **2. Data Collection & Ingestion**

### **Wikipedia Scraping**

- The project uses **BeautifulSoup** to extract structured data from **Wikipedia tables**.
- The scraped data is **cleaned and stored in a CSV file** before merging with Kaggle data.

### **Kaggle Dataset Handling**

- The dataset is loaded into **pandas** for preprocessing.
- Data is validated, and missing fields are handled to ensure consistency.

---

## **3. Data Processing & Storage**

### **Data Cleaning**

- **Standardizing movie titles** across Wikipedia & Kaggle datasets.
- **Handling missing values** (e.g., box office earnings, genres).
- **Ensuring accurate genre classification** for Best Picture winners.

### **Data Storage**

- All processed data is stored in an **SQLite database**.
- The database includes three main tables:
  - **Movies**: Stores title, year, genre, box office data.
  - **Awards**: Tracks award categories and winners.
  - **Speech Data (Stretch Goal)**: If Wikipedia movie summaries are available, this will be used for NLP analysis.

---

## **4. Data Analysis & Querying**

### **SQL Queries**

The project performs **SQL-based analysis** to uncover patterns, such as:

- **Winning movie trends** over different decades.
- **Correlations between box office revenue & awards**.
- **Genre analysis** for Best Picture winners.

### **Python-Based Analysis**

- **Statistical insights** (e.g., average IMDb ratings of winners).
- **Visualization using Matplotlib & Seaborn**.
- **Stretch Goal**: **Word Cloud** based on Wikipedia movie summaries.

---

## **5. Data Visualization**

The project utilizes **various visualizations** to make insights clear:

| Visualization Type | Purpose |
|-------------------|---------|
| **Bar Charts** | Show trends in Best Picture wins by genre |
| **Scatter Plots** | Explore relationships between box office revenue & awards |
| **Timelines** | Track genre trends over decades |
| **Stretch Goal: Word Cloud** | Analyze common themes in Wikipedia movie summaries |

These visualizations help **illustrate historical Oscar-winning trends** in an engaging format.

---

## **6. Deployment & Version Control**

### **GitHub Repository**

- The project is version-controlled using **GitHub**, with structured commits.
- All scripts and datasets are stored in an **organized file structure**.

### **Jupyter Notebook Execution**

- The main analysis is performed in `academy_awards_analysis.ipynb`.
- The notebook is designed for **reproducibility**, ensuring anyone can run it with minimal setup.

---

## **7. Summary**

This **Academy Awards Analysis System** is designed for:

✅ **Reliable data collection** via Wikipedia scraping & Kaggle dataset.  
✅ **Efficient data storage** in an SQLite database.  
✅ **Comprehensive SQL & Python-based analysis** for meaningful insights.  
✅ **Professional data visualizations** to illustrate findings.  

This structure ensures **scalability, reproducibility, and ease of analysis** while providing an engaging exploration of Oscar-winning movies.
