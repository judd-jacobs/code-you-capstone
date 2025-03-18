# 📜 Academy Awards Analysis: Project Plan

## **1. Project Overview**

This project investigates trends in **Oscar-winning movies** to uncover patterns in **genres, box office performance, and award distribution**. The analysis explores:

- 🎬 **What genres dominate the Academy Awards?** (Visualized through bar charts)
- 💰 **Is there a correlation between box office revenue and award wins?** (Scatter plot analysis)
- 📈 **How have winning trends evolved over time?** (Timelines of winning genres)
- ☁️ **Stretch Goal**: **Word Cloud** analysis from Wikipedia movie summaries (*if feasible*).

This project integrates **data collection, SQL querying, and data visualization** to provide meaningful insights into the **history of the Academy Awards**.

---

## **2. Background**

My love for movies began with **Disney’s animated classics**, where magical stories and unforgettable music shaped my childhood. Watching my favorite movies receive Oscars **sparked my curiosity** about what made a film award-worthy.

Over time, my interest expanded beyond animation, and the **Oscars became an annual tradition**. This project is a reflection of that early enthusiasm—**a fun and insightful exploration of Oscar-winning movie trends**.

---

## **3. Technical Insight**

### **Data Sources**

- **Wikipedia Scraping**: Extracts Best Picture winners and metadata.
- **Kaggle Dataset**: Provides structured Oscar award data.

### **Processing & Storage**

- **BeautifulSoup** scrapes Wikipedia data.
- **Pandas** cleans and structures datasets.
- **SQLite Database** stores award & genre trends.

### **Data Analysis & Visualization**

- **SQL Queries** identify patterns in Oscar winners.
- **Matplotlib & Seaborn** generate visual insights.
- **Stretch Goal**: **Word Cloud** using Wikipedia movie summaries (*if feasible*).

---

## **4. Project Requirements & Features**

### **Core Requirements**

✅ **Data Collection**

- Scrape **Best Picture winners** and metadata from **Wikipedia**.
- Integrate **Kaggle Oscar Award dataset** for structured award data.
- Store data in an **SQLite database**.

✅ **Data Analysis & SQL Queries**

- Extract trends in **Best Picture winners** over the decades.
- Analyze **genre distribution** and award patterns.
- Investigate **box office revenue vs. awards**.

✅ **Data Visualization**

- **Bar Charts**: Best Picture wins by genre.
- **Scatter Plots**: Box office revenue vs. IMDb ratings.
- **Timelines**: Trends in winning genres over time.

✅ **Project Structure & Deployment**

- Maintain a **clean and structured GitHub repository**.
- Ensure **README.md** includes setup instructions and troubleshooting.
- Document the **data pipeline** in [`system_architecture.md`](system_architecture.md).

### **Stretch Goals**

🔹 **☁️ NLP Word Cloud**  

- If Wikipedia movie summaries are accessible, generate a **word cloud** from common words in descriptions.

🔹 **☁️ OMDb API**  

- For possible future development, incorporate additional data from the Online Movie Database (OMDb).

🔹 **📊 Interactive Visualizations**  

- If time permits, explore **Plotly or Tableau** for enhanced interactivity.

---

## **5. Risk Assessment & Mitigation**

- **Web Scraping Risks**: Wikipedia structure may change → Implement error handling.
- **Data Quality Issues**: Movie title mismatches → Use **fuzzy matching**.
- **Stretch Goal Feasibility**: If Wikipedia summaries aren’t accessible, omit Word Cloud.

---

## **6. Project Evaluation Criteria**

✅ **Data Completeness**: Properly scraped Wikipedia & Kaggle data.  
✅ **Query Performance**: SQL queries return expected results efficiently.  
✅ **Visualization Clarity**: Graphs are well-annotated and easy to interpret.  
✅ **GitHub Organization**: Repository is structured, with clear documentation.  

---

## **7. Deployment & Version Control**

- **GitHub repository** with structured commits.
- **Jupyter Notebook** as the primary analysis tool.
