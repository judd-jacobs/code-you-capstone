# 📝 Academy Awards Data Analysis Project Plan

---

## 1. 🎯 Project Overview

This project explores trends among Academy Award-nominated and winning films, with a focus on Best Picture contenders. Using publicly available data from Wikipedia and APIs, we examine how genre, critical acclaim, box office performance, and runtime relate to Oscar recognition. The goal is to uncover meaningful storytelling and industry insights through a combination of data wrangling, visualization, and interpretation.

---

## 2. 🎬 Background

My love for movies began with Disney’s animated classics — colorful, musical stories that lit up my childhood. As I grew older, I became fascinated with the Oscars, curious about what makes a film worthy of such recognition. This project blends my passion for storytelling with my skills as a budding data analyst. It’s a personal and technical journey into the patterns behind Hollywood’s most celebrated films.

---

## 3. ❓ Research Question

What trends and patterns can be identified among Oscar-nominated and winning films in terms of:

- Genre frequency and shifts over time
- Box office success
- IMDb ratings and critical reception
- Runtime and its impact on revenue or awards

---

## 4. 📚 Data Sources

- **Wikipedia**: Scraped using `pandas.read_html()` and `BeautifulSoup` for Best Picture nominees and winners
- **TMDb API**: Used to enrich films with genre information
- **OMDb API**: Used to retrieve metadata like IMDb ratings, box office revenue, and runtime

---

## 5. 🧰 Tools & Technologies

- **Version Control**: Git and GitHub were used throughout the project for version control, progress tracking, and easy sharing with collaborators or prospective employers.
- **Languages**: Python (Jupyter Notebook)
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Requests, SQLite, SQLAlchemy
- **APIs**: TMDb, OMDb
- **Database**: SQLite for structured storage and queries
- **Documentation**: Markdown-based inline commentary

---

## 6. 📦 Feature Selection

This project includes:

- ✅ Use of at least 2 external data sources (Wikipedia, TMDb, OMDb)
- ✅ Data ingestion, cleaning, and transformation using pandas
- ✅ Database integration via SQLite with structured tables
- ✅ Use of Matplotlib and Seaborn for static visualizations
- ✅ Feature selection across multiple categories: genre, revenue, ratings, runtime, and decade
- ✅ Initiation of a virtual environment

---

## 7. 🧹 Data Cleaning & Transformation

- Parsed and merged scraped HTML tables with API results
- Converted currency, ratings, and runtime fields to numeric formats
- Exploded multi-genre fields for cleaner analysis
- Filtered outlier values to improve visualization clarity
- Stored cleaned datasets in SQLite tables for query support

---

## 8. 📊 Implementation & Visualizations

- **Notebook Structure**: Each visualization is implemented in a clean, modular format with a markdown introduction, well-labeled code cell, and a human-readable summary of results. This structure supports both learning and storytelling.
- **Bar Charts**: Highest-grossing films, genre revenue, and ratings by decade
- **Heatmaps**: Genre frequency over time
- **Scatterplots**: Runtime vs. revenue, IMDb rating vs. box office
- **Labeling & Styling**: Thoughtfully styled with professional fonts, formatting, and consistent visual theming
- **Target Audience**: Movie lovers and aspiring analysts

---

## 9. ✨ Stretch Goals

- **Word Cloud**: Originally intended to visualize film summaries — deferred due to limited plot data availability
- **Tableau Dashboard**: Potential future feature for interactive drill-down

---

## 10. 🚧 Risk Assessment

- **API Rate Limits**: Required retries and lightweight caching
- **Data Gaps**: Some films lacked complete metadata and were filtered
- **Outliers**: Extremely long runtimes or high/low box office removed to enhance readability
- **Genre Variability**: Multi-genre films required parsing and careful grouping

---

## 11. 🧠 Review & Interpretation

- *Drama* dominates across decades but newer genres like *Fantasy* and *Adventure* are on the rise
- Box office revenue doesn’t guarantee Oscar wins — and IMDb ratings don’t guarantee revenue
- The Academy’s tastes have broadened over time, reflecting cultural, economic, and artistic shifts

---

## 12. ✅ Final Status & Next Steps

- All visualizations and documentation complete
- Final cleaning and markdown alignment finished
- Ready for review and publishing

📅 **Submitted:** March 28, 2025  
🧠 **Reflects:** Analytical growth, storytelling precision, and a lifelong love for film 🍿
