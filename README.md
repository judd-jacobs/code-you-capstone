# 🎬 Academy Awards Analysis

**Author**: Judd Jacobs

**Project Repository**: <https://github.com/judd-jacobs/code-you-capstone>

## Project Overview

This project analyzes historical trends in **Academy Award-winning movies**, exploring patterns in genres, box office success, and award distribution. Using **Wikipedia web scraping** and **Kaggle datasets**, we collect and process Oscar-related data, store it in an **SQLite database**, and generate insights using **SQL and Python visualizations**.

This project combines **data extraction, SQL querying, data visualization, and natural language processing techniques** (**stretch goal**) to provide an engaging exploration of Oscar history.

## Features & Visualizations

- Genre Trends: Bar charts showing Best Picture winners by genre.
- Box Office & Awards: Scatter plots for revenue vs. award wins.
- Time-Based Analysis: A timeline of winning genres.
- Stretch Goal: Word Cloud from Wikipedia movie summaries (if feasible).

## Data Sources

- **Wikipedia Scraping**: Best Picture winners and movie metadata.
- **Kaggle Dataset**: Oscar awards data from various categories.

## Technologies Used

- **Python** (pandas, BeautifulSoup, NumPy, Matplotlib, Seaborn, WordCloud)
- **SQLite** (SQLAlchemy for structured queries)
- **Jupyter Notebook** (for analysis & visualization)
- **GitHub** (for version control)

## Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/juddjacobs/code-you-capstone.git
```

After you have cloned the repository to your machine, navigate to the project folder in GitBash/Terminal.

```bash
cd [your_project_folder]
```

### 2️⃣ Create a Virtual Environment & Install Dependencies

```bash
python3 -m venv venv
# Mac/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate   

pip install -r requirements.txt
```

### 3️⃣ Run the Jupyter Notebook

```bash
jupyter notebook
```

Open academy_awards_analysis.ipynb and execute cells in order.

### 4️⃣ Deactivate Virtual Environment

When finished working in the repo, deactivate the virtual environment.

```bash
# For Linux/Mac and GitBash
deactivate
```

---

### 5️⃣ Summary of Virtual Environment Commands

| Command | Linux/Mac | GitBash |
| ------- | --------- | ------- |
| Create | `python3 -m venv venv` | `python -m venv venv` |
| Activate | `source venv/bin/activate` | `source venv/Scripts/activate` |
| Install | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| Deactivate | `deactivate` | `deactivate` |

---

## Troubleshooting

If errors occur:

- Ensure all dependencies are installed with pip install -r requirements.txt.
- Run jupyter notebook inside the virtual environment.
- Verify database files exist (academy_awards.db).

---

## License

This project is open-source under the MIT License.

---

## AI Disclaimer

AI tools including Google Gemini and ChatGPT were used as co-intelligence resources when developing this project together.

---

## Additional Documentation

- [Project Plan](project_plan.md)
- [Risk assessment](risk_assessment.md)
- [Timeline](timeline.md)
- [Academy Award Analysis](academy_awards_analysis.ipynb)
