# code-you-capstone
August 2024 Capstone Project Repository for Code:You

# Academy Awards Analysis: Project Plan

## **1. Project Overview**
I have been a fan of the Academy Awards for as long as I can remember.

This analysis project investigates trends in Oscar-winning movies to uncover patterns and correlations. The project aims to analyze data on genres, runtimes, box office performance, and other factors to answer questions like:
- What genres dominate the Academy Awards? This will be analyzed using bar charts to visualize genre distributions over time.
- How have winning trends evolved over time? A timeline of winning genres will show shifts in preferences or themes across decades.
- Is there a correlation between box office success and award wins? Scatter plots will be used to examine relationships between box office revenue and award outcomes, providing quantitative insights.

This analysis will provide insights through detailed visualizations and SQL-based queries, offering a comprehensive look at historical Academy Award trends.

### **Proposed Features:**
1. Analyze trends in Best Picture winners by genre and runtime.
2. Examine correlations between box office performance and award wins.
3. Provide visual insights through bar charts, scatter plots, and pivot tables.

---

## **2. Technical Insight**

### **Tools and Technologies:**
- **Python**: Used for data cleaning, analysis, and visualization with libraries such as pandas, matplotlib, and seaborn.
- **SQL**: SQLite database for storing and querying integrated datasets.
- **APIs**:
  - **TMDb API**: To retrieve movie metadata, genres, and box office data.
  - **Optional**: OMDb API or additional CSV datasets for redundancy, which ensures data reliability by cross-referencing sources and filling potential gaps in metadata or box office figures.
- **GitHub**: For version control, with regular commits to track progress.

### **Integration Strategy:**
1. **Data Loading**: Retrieve movie metadata and box office data from the TMDb API and supplement with historical Academy Award data from CSV/Excel files.
2. **Data Cleaning**: Use pandas to handle missing values, standardize columns, and merge datasets.
3. **Data Storage**: Store cleaned and merged data in a SQLite database.
4. **Analysis:**
   - Write SQL queries to explore trends (e.g., genres of Best Picture winners over decades).
   - Use Python for advanced analysis, including correlations and rankings.
5. **Visualization**:
   - Create bar charts for genre distributions and timelines for trends.
   - Use scatter plots to analyze correlations (e.g., runtime vs. box office revenue).
   - Optionally create interactive visualizations using Plotly or Tableau.

---

## **3. Optional Visual Aids**

### **Proposed Visualizations:**
- **Bar Chart**: Number of Best Picture wins by genre.
- **Scatter Plot**: Box office revenue vs. IMDb rating for winners.
- **Timeline**: Trends in winning genres over decades.

### **Flowchart:**
A simple diagram illustrating the flow of data from APIs to analysis and visualization:
1. **Data Sources**: TMDb API, CSV files.
2. **Data Cleaning**: Handle missing values, merge datasets in pandas.
3. **Database**: Store processed data in SQLite.
4. **Analysis**: Python and SQL.
5. **Visualizations**: Generate graphs in Python and optionally Tableau or Plotly.

---

## **4. Mentor Feedback**
To ensure alignment with project requirements, feedback will be requested on:
1. Feasibility of using the TMDb API and datasets.
2. SQL schema design and queries.
3. Clarity of visualizations and insights.

Mentor feedback will guide refinements to the plan and implementation.

---

## **5. Timeline**

### **Week 1-2: Setup and Data Loading**
- Finalize datasets and APIs.
- Set up GitHub repository and virtual environment.
- Load initial datasets from TMDb API and CSV files.

### **Week 3-4: Data Cleaning and Database Setup**
- Clean data using pandas.
- Design and populate SQLite database.
- Begin exploring data with SQL queries.

### **Week 5-6: Analysis and Visualization**
- Perform advanced analysis using Python and SQL.
- Create visualizations (bar charts, scatter plots, timelines).
- Test and refine analysis scripts.

### **Week 7-8: Finalization and Submission**
- Polish visualizations and add annotations.
- Write README and code comments.
- Conduct testing and incorporate mentor feedback.
- Submit the project on GitHub before the deadline.

### **Review and Polishing**
- Include clear data interpretation sections in the Jupyter Notebook and README to ensure accessibility to unfamiliar audiences.
- Annotate code with Markdown cells and detailed comments to enhance clarity and coherence.

---

## **Next Steps**
1. Create wireframes and flowchart to support understanding.
2. Begin Week 1 tasks: setting up APIs and gathering data.
3. Review the plan with a mentor for feedback.

---

This document provides a comprehensive roadmap for completing the Academy Awards Analysis project, ensuring alignment with all requirements.

