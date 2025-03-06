# **Flowchart:**

This flowchart outlines the data analysis pipeline for the Academy Awards Analysis project:

1. **Data Sources:**

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

   - Bar charts, scatter plots, timelines, and word clouds using Python libraries (matplotlib, seaborn, and NLTK for NLP visualizations).
   - Optionally: Use Tableau or Plotly to develop interactive dashboards for enhanced insights.
