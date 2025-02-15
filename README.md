# Academy Awards Analysis

**Author**: Judd Jacobs  
**Date**: 2025-02-12  
**Project Repository**: <https://github.com/judd-jacobs/code-you-capstone>

## Project Overview

The **Academy Awards Analysis** project explores trends in Oscar-winning movies and acceptance speeches (**stretch goal**) to uncover insights into winning genres, box office performance, and recurring themes in speeches. Using data from APIs and historical records, this project provides structured visualizations and analysis of Academy Award winners over time.

### Key Questions Explored

✅ What genres have dominated the Academy Awards over the decades?  
✅ How does box office performance relate to Oscar success?  
✅ What words are most commonly used in acceptance speeches?  

This project combines **data extraction, SQL querying, data visualization, and natural language processing techniques** (**stretch goal**) to provide an engaging exploration of Oscar history.

## System Architecture

The project follows a structured data pipeline:

1. **Data Collection**
   - **TMDb API**: Retrieves movie metadata, genres, and box office earnings.  
   - **OMDb API**: Supplements TMDb data with additional details like director, writer, and critical ratings.  
   - **CSV Files**: Provides historical Oscar winners and acceptance speech transcripts (*stretch goal*).  

2. **Data Processing & Cleaning**
   - Handling missing values and standardizing data formats using **pandas**.  
   - Preprocessing speech text using **NLTK** for word frequency analysis. (*stretch goal*)

3. **Data Storage**
   - **SQLite Database** with structured tables for movies, awards, and speeches.  

4. **Analysis & Visualization**
   - **SQL queries** to extract trends in winning movies and speeches.  
   - **Python visualizations** (Matplotlib, Seaborn) to generate bar charts, scatter plots, timelines, and word clouds.  

5. **Deployment & Version Control**
   - All code is version-controlled using **GitHub** for reproducibility.

## Technologies Used

- **Python** – Data processing, analysis, and visualization  
- **Pandas, NumPy** – Data manipulation and cleaning  
- **Matplotlib, Seaborn, WordCloud** – Data visualization
- **NLTK** – Natural language processing for speech analysis (*stretch goal*)
- **SQLite** – Database for structured data storage  
- **SQL** – Querying award and movie data  
- **TMDb & OMDb APIs** – Data retrieval for movie details  
- **GitHub** – Version control and project tracking

## Project Requirements

This project was created to fulfill the requirements of Code Louisville’s Python Data Analytics 2 class. The project had four requirements as follows:

1. Read in two data sets.
2. Make 3 plots
3. Make a virtual environment for the project
4. Annotate our code

## Project Features

- Feature 1 - Read data from 2 data sources
  - This was accomplished by...(e.g., reading in 3 csv files)

- Feature 2 - Manipulate and clean your data
  - The data was cleaned by... (e.g., removing missing data and dropping data that was not needed, and mapping values)

- Feature 3 - Visualize data
  - By utilizing the ... (e.g. `groupby`) method...(e.g. sub plots where made to reveal a gender and racial bias on citations).

- Feature 4 - Utilized a virtual environment and include instructions in the README on how the user should run the project.

- Feature 5 - Interpreted the data by annotating the code via markdown cells.

## Installation & Setup Requirements

### 1. Clone the Repository

```bash
git clone https://github.com/judd-jacobs/code-you-capstone.git
```

After you have cloned the repo to your machine, navigate to the project folder in GitBash/Terminal.

```bash
cd [your_project_folder]
```

### 2. Create Virtual Environment

```bash
# For Linux/Mac
python3 -m venv venv

# For GitBash
python -m venv venv
```

### 3. Activate the Virtual Environment

```bash
# For Mac/Linux
source venv/bin/activate   

# For GitBash
source venv/Scripts/activate      
```

### 4. Install Requried Packages

From the directory pip install the "requirements.txt" file.

```bash
# For Linux/Mac and GitBash
pip install -r requirements.txt
```

### 5. Deactivate Virtual Environment

When finished working in the repo, deactivate the virtual environment.

```bash
# For Linux/Mac and GitBash
deactivate
```

### Summary of Virtual Environment Commands

| Command | Linux/Mac | GitBash |
| ------- | --------- | ------- |
| Create | `python3 -m venv venv` | `python -m venv venv` |
| Activate | `source venv/bin/activate` | `source venv/Scripts/activate` |
| Install | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| Deactivate | `deactivate` | `deactivate` |

### 6. Set up API Keys

- Obtain API keys from TMDb and OMDb.
- Create a .env file and add your API keys:

```python
TMDB_API_KEY = "your_tmdb_api_key"
OMDB_API_KEY = "your_omdb_api_key"
```

### 7. Run the Jupyter Notebook

---

## Additional Documentation

[Risk assessment](risk_assessment.md)

[Timeline](timeline.md)
