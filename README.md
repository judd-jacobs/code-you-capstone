# code-you-capstone

# Academy Awards Analysis: Project Plan

## **1. Project Overview**

The Academy Awards Analysis project investigates trends in Oscar-winning movies to uncover patterns and correlations. The project aims to analyze data on genres, runtimes, and box office performance, exploring how these factors interrelate to influence Academy Award outcomes. By examining their connections, we can identify patterns in winning films, such as whether certain genres are more likely to be associated with higher box office earnings or if runtime impacts critical reception.

- What genres dominate the Academy Awards? This will be analyzed using bar charts to visualize genre distributions over time.
- How have winning trends evolved over time? A timeline of winning genres will show shifts in preferences or themes across decades.
- Is there a correlation between box office success and award wins? Scatter plots will be used to examine relationships between box office revenue and award outcomes, providing quantitative insights.

This analysis will provide insights through detailed visualizations and SQL-based queries, offering a comprehensive look at historical Academy Award trends.

### **Proposed Features:**

1. Analyze trends in Best Picture winners by genre and runtime.

2. Examine correlations between box office performance and award wins.

3. Provide visual insights through bar charts, scatter plots, pivot tables, and word clouds.

## **2. Background**

My love for movies began with Disney’s animated classics, where magical stories and unforgettable music captivated me. As I became more immersed in these films, I discovered the Academy Awards through Disney’s many wins and nominations. Watching my favorite movies receive Oscars sparked my curiosity about what made a film award-worthy.

Over time, my interest expanded beyond animation, and the Oscars became an annual tradition for me. I was drawn to the excitement of seeing which films would take home the top honors and how cinematic trends evolved over the years. This project is an exploration of the patterns behind Oscar-winning movies, blending data analysis with my lifelong love for the movies.

This project is a reflection of that early enthusiasm—a fun and insightful exploration of the trends and patterns behind Oscar-winning movies. By analyzing the data behind the Academy Awards, I hope to uncover fascinating insights while recapturing some of the wonder and joy that these films have brought me over the years.

## **3. Technical Insight**

This section outlines the key technologies, data sources, and methods used to analyze Academy Award-winning movies and acceptance speeches.

### **Tools and Technologies:**

- **Python**: Used for data cleaning, analysis, and visualization with libraries such as pandas, matplotlib, or others.
- **SQL**: SQLite database for storing and querying integrated datasets.
- **APIs**:
  - **TMDb API**: To retrieve movie metadata, genres, and box office data.
  - **OMDb API**: To supplement TMDb data, particularly for additional movie details such as director, writer, and ratings from multiple sources.
- **CSV Datasets**: Supplementary datasets to provide redundancy and ensure data reliability by cross-referencing sources and filling potential gaps in metadata or box office figures. These additional sources will be used in cases where TMDb or OMDb data is incomplete or inconsistent, ensuring comprehensive and accurate analysis without excessive duplication.
- **GitHub**: For version control, with regular commits to track progress.

### **Integration Strategy:**

The data pipeline follows a structured process to ensure clean and meaningful insights.

1. **Data Loading**: Collect movie metadata, genres, and box office data from the TMDb and OMDb APIs. Supplement with CSV datasets containing historical Academy Award winners. Gather transcripts from the Academy Awards Speech Database to analyze word frequency trends in speeches. Additionally, collect acceptance speech transcripts from the Academy Awards Acceptance Speech Database.

2. **Data Cleaning**: Use pandas to manage missing values, ensure consistency across sources, and preprocess text data by tokenizing, removing stopwords, and normalizing words for word cloud generation.

3. **Data Storage**: Store cleaned and merged data in an SQLite database, including structured tables for movies, awards, and speeches.

4. **Analysis**:

   - Write SQL queries to explore trends such as the evolution of Best Picture genres and word usage in acceptance speeches over time.

   - Use Python to conduct correlation analysis on box office revenue and Oscar wins.

   - Generate word clouds from acceptance speeches to highlight commonly used words across different decades.

   - Write SQL queries to explore trends (e.g., genres of Best Picture winners over decades, word frequency trends in speeches).

   - Use Python for advanced analysis, including correlations, rankings, and word frequency analysis of speech transcripts to generate word clouds.

5. **Visualization**:

   - Bar charts for genre distributions to analyze how different genres have performed over time.
   - Timelines for trends to visualize how winning movie characteristics and speech themes have evolved.
   - Scatter plots to examine correlations (e.g., runtime vs. box office revenue) and determine patterns in award-winning films.
   - Word clouds and frequency analysis of common speech phrases over time.

6. **Optional Enhancements:**

   - Interactive visualizations for deeper user engagement and dynamic data exploration.

## **4. Optional Visual Aids**

### **Proposed Visualizations:**

**Bar Chart:** Number of Best Picture wins by genre.

This visualization will feature:

- **X-Axis**: Genres (e.g., Drama, Comedy, Action).
- **Y-Axis**: Number of wins.
- **Additional Details**:
  - Group bars by decade to illustrate how genre popularity has shifted over time.
  - Color-code bars by decade for better readability.
  - Include a legend to explain the color scheme and highlight the most frequent genres in each era.

**Scatter Plot:** Box office revenue vs. IMDb rating for winners.

IMDb ratings serve as a widely accepted measure of audience reception and critical acclaim, making them a useful metric for evaluating award-winning films.&#x20;

This visualization will feature:

- **X-Axis**: Box office revenue (in millions).
- **Y-Axis**: IMDb rating (scale of 1-10).
- **Additional Details**:
  - Points will be color-coded to represent the decade of release, aiding in identifying patterns over time.
  - Include a legend to explain the color scheme.
  - Add trend lines or annotations to highlight notable clusters or outliers, such as high-grossing films with lower ratings.

**Timeline:** Trends in winning genres over decades.

This visualization will feature:

- **X-Axis**: Decades (e.g., 1920s, 1930s, ..., 2020s).
- **Y-Axis**: Number of wins per genre.
- **Additional Details**:
  - Each decade will have stacked bars representing different genres, illustrating shifts in dominant genres over time.
  - Color-code genres for easy differentiation, with a legend explaining the color assignments.
  - Annotations to highlight significant trends, such as the rise of sci-fi films in recent decades or the historical dominance of drama films.

### **Flowchart:**

This flowchart outlines the data analysis pipeline for the Academy Awards Analysis project:

1. **Data Sources:**

   - **TMDb API**: Retrieve data such as movie titles, genres, release years, box office revenue, and IMDb ratings.
   - **CSV Files**: Supplementary datasets containing historical Academy Award winners.
   - **Academy Awards Speech Database**: Collect transcripts of acceptance speeches for linguistic analysis.

2. **Data Cleaning:**

   - Handle missing values (e.g., filling gaps in box office data, ensuring complete speech transcripts).
   - Standardize formats (e.g., consistent genre naming, normalizing text for NLP analysis).
   - Merge datasets on common keys, such as movie titles and years, using pandas.

3. **Database:**

   - Store processed and cleaned data in an SQLite database.
   - Create structured tables for movies, awards, and speech transcripts to enable efficient querying.

4. **Analysis:**

   - Use SQL queries to identify trends (e.g., genres of Best Picture winners over decades, word frequency trends in speeches).
   - Leverage Python for deeper analysis, including correlations, rankings, and word frequency analysis to generate word clouds.

5. **Visualizations:**

   - Create bar charts, scatter plots, timelines, and word clouds using Python libraries (matplotlib, seaborn, and NLTK for NLP visualizations).
   - Optionally use Tableau or Plotly to develop interactive dashboards for enhanced insights.

## **5. Mentor Feedback**

To ensure alignment with project requirements, feedback will be requested on:

1. Feasibility of using the TMDb API and datasets.
2. SQL schema design and queries.
3. Clarity of visualizations and insights

## **6. Timeline**

### **Week 1-2: Setup and Data Loading**

- Finalize datasets and APIs.
- Set up GitHub repository and virtual environment.
- Load initial datasets from TMDb API and CSV files.
- Confirm data quality by verifying completeness, checking for missing values, and ensuring consistency in key fields such as movie titles and years across datasets.

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
- Perform final validation steps, including verifying data integrity, testing all SQL queries and visualizations, reviewing code annotations, and ensuring all documentation is complete and accurate.

### **Review and Polishing**

- Include clear data interpretation sections in the Jupyter Notebook and README to ensure accessibility to unfamiliar audiences. For example, explain how genre distributions reflect historical trends or how correlations between box office revenue and award wins provide actionable insights.
- Annotate code with Markdown cells and detailed comments to enhance clarity and coherence. Provide clear explanations for each step, such as data cleaning, SQL queries, and visualization choices, ensuring that all logic is transparent and easy to follow.