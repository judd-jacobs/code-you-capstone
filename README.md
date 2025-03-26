# 🎬 Academy Awards Analysis

**Author**: Judd Jacobs  
**Project Repository**: [GitHub Repo](https://github.com/judd-jacobs/code-you-capstone)

---

## 📣 Project Summary

This project offers a fun and data-driven deep dive into **Academy Award-nominated and winning films**, with a spotlight on the **Best Picture** category.

Combining **web scraping**, **API integration**, **data cleaning**, and **visual storytelling**, this project explores:

- 🎭 Genre trends across decades
- 💵 Box office performance vs. critical acclaim
- 📊 Runtime, ratings, and revenue relationships

Built in **Python** with `pandas`, `BeautifulSoup`, `matplotlib`, and **SQLite**, it features:

- Heatmaps, scatterplots, and bar charts
- Custom formatting for readability
- A clean, modular Jupyter Notebook structure

Whether you're a **movie buff**, **data scientist in training**, or just curious about what makes a film "Oscar-worthy," this project offers both insight and entertainment. 🍿

➡️ [Explore the notebook](academy_awards_analysis.ipynb)  
➡️ [Read the full project plan](project_plan.md)

## 📌 Project Overview

This project analyzes historical trends among **Academy Award-nominated and winning films**, with a special focus on the **Best Picture** category. Using web scraping, API calls, SQL database storage, and a range of visualizations, it explores:

- How genres have evolved over time
- Relationships between IMDb ratings and box office performance
- Patterns of award recognition versus commercial success

By combining storytelling with data, this project offers a fun and analytical look at Oscar trends — made for movie lovers and aspiring data scientists alike.

---

## 🎯 Features & Visualizations

- **Genre Trends**: Heatmaps and bar charts by decade
- **Box Office vs. IMDb Ratings**: Scatterplots showing correlation
- **Top-Grossing Oscar Films**: Horizontal bar charts
- **Revenue by Genre**: Box office averages and totals per genre
- **Runtime vs. Revenue**: Scatterplots with outlier handling
- **Stretch Goal (Deferred)**: Word cloud from movie plot summaries

Each visualization includes clean formatting, summary text, and audience-friendly labels.

---

## 🔎 Data Sources

- 📄 **Wikipedia** – Scraped Best Picture nominees and winners
- 🎬 **TMDb API** – Genre classification
- 🎥 **OMDb API** – IMDb ratings, box office, and metadata

---

## 🧰 Technologies Used

- **Python**: `pandas`, `requests`, `beautifulsoup4`, `matplotlib`, `seaborn`, `sqlite3`, `sqlalchemy`
- **Data Storage**: SQLite relational database
- **IDE**: Jupyter Notebook (run with virtual environment)
- **Version Control**: GitHub for documentation and collaboration

---

## ⚙️ Setup Instructions

### 💻 Virtual Environment Commands (Quick Reference)

| Action          | Mac/Linux Command           | Windows Command            |
|----------------|------------------------------|-----------------------------|
| Create venv     | `python3 -m venv venv`       | `python -m venv venv`       |
| Activate venv   | `source venv/bin/activate`   | `venv\Scripts\activate`     |
| Deactivate venv | `deactivate`                 | `deactivate`                |

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/judd-jacobs/code-you-capstone.git
cd code-you-capstone
```

### 2️⃣ Create Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate   # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Project

```bash
jupyter notebook
```

Open `academy_awards_analysis.ipynb` and execute the cells in order.

### 5️⃣ Deactivate Environment

```bash
deactivate
```

---

## 🛠 Troubleshooting

- Ensure all dependencies are installed via `pip install -r requirements.txt`
- Make sure `.env` file with API keys is set locally
- Run inside the virtual environment
- If database errors occur, verify SQLite files are in place

---

## 📄 License

This project is open-source under the **MIT License**.

---

## 🤖 AI Disclaimer

AI tools including ChatGPT and Google Gemini were used to support brainstorming, troubleshooting, and documentation during development.

---

## 📎 Additional Documentation

- [Project Plan](project_plan.md)
- [Data Dictionary](data_dictionary.md)
- [Jupyter Notebook](academy_awards_analysis.ipynb)
