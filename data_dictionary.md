# 🗂️ Data Dictionary

This data dictionary provides a reference for the structured fields used across key dataframes in this project. Data was collected from Wikipedia, TMDb API, and OMDb API, then cleaned and enriched for analysis.

---

## 📦 `omdb_metadata_clean`

| Column Name       | Type       | Description                                                   | Example               |
|-------------------|------------|---------------------------------------------------------------|------------------------|
| `film`            | object     | Title of the film                                             | `The Godfather`        |
| `year`            | int64      | Year of the film's release                                    | `1972`                 |
| `title_api`       | object     | Title returned by OMDb API                                    | `The Godfather`        |
| `rated`           | object     | MPAA rating                                                   | `R`                    |
| `released`        | object     | Official release date                                         | `24 Mar 1972`          |
| `runtime`         | object     | Raw runtime string from OMDb                                  | `175 min`              |
| `director`        | object     | Director(s) of the film                                       | `Francis Ford Coppola` |
| `writer`          | object     | Writer(s) of the film                                         | `Mario Puzo`           |
| `actors`          | object     | Featured actors                                               | `Marlon Brando, Al Pacino` |
| `plot`            | object     | Short plot description                                        | `The aging patriarch...`|
| `language`        | object     | Primary spoken languages                                      | `English`              |
| `country`         | object     | Producing countries                                           | `USA`                  |
| `awards`          | object     | Awards summary from OMDb                                      | `Won 3 Oscars`         |
| `poster`          | object     | URL of the poster image                                       | `https://...jpg`       |
| `ratings`         | object     | List of external rating sources                               | `[{"Source": "IMDB", ...}]` |
| `metascore`       | float64    | Metacritic score                                              | `100.0`                |
| `imdbRating`      | float64    | IMDb rating (0–10 scale)                                      | `9.2`                  |
| `imdbVotes`       | Int64      | IMDb vote count                                               | `1,600,000`            |
| `imdbID`          | object     | IMDb identifier                                                | `tt0068646`            |
| `type`            | object     | Type of media                                                 | `movie`                |
| `boxOffice`       | object     | Raw box office string                                         | `$134,966,411`         |
| `response`        | object     | API success indicator                                         | `True`                 |
| `runtime_mins`    | Int64      | Runtime converted to minutes                                  | `175`                  |
| `boxOffice_clean` | float64    | Cleaned box office as float (USD)                             | `134966411.0`          |
| `decade`          | int64      | Film’s release decade                                         | `1970`                 |
| `winner`          | bool       | `True` if the film won Best Picture                           | `True`                 |

---

## 📦 `best_picture_wikipedia`

| Column Name   | Type     | Description                                      | Example                                 |
|----------------|----------|--------------------------------------------------|------------------------------------------|
| `film`         | object   | Title of the nominated or winning film           | `Everything Everywhere All at Once`      |
| `year`         | float64  | Year the film was eligible or released           | `2022.0`                                 |
| `awards`       | object   | Number of Oscars won                             | `7`                                      |
| `nominations`  | object   | Total number of nominations received             | `11`                                     |
| `status`       | object   | Whether the film was a `Winner` or `Nominee`     | `Winner`                                 |

---

## 📦 `tmdb_genre_results`

| Column Name | Type     | Description                                 | Example               |
|-------------|----------|---------------------------------------------|------------------------|
| `film`      | object   | Title of the film                          | `The Godfather`        |
| `year`      | int64    | Year of the film's release                 | `1972`                 |
| `genre`     | object   | List of genre(s) from TMDb API             | `['Crime', 'Drama']`   |

---

### 🧮 Temporary & Merged Analysis Frames

These are intermediate datasets created during cleaning, transformation, and visualization steps.

| Column Name       | Type     | Description                                                    | Example         |
|-------------------|----------|----------------------------------------------------------------|------------------|
| `status`          | object   | Winner/Nominee status derived from `winner`                   | `Winner`         |
| `formatted`       | object   | Formatted revenue string for labels                           | `$140M`          |
| `count`           | int64    | Count of grouped items (e.g., genre or decade frequency)       | `43`             |
| `genre_exploded`  | object   | Single genre per row from exploded genre lists                | `Drama`          |

These are generated temporarily and are not stored in the final SQLite database.

---

📌 Note: Fields such as `genre`, `boxOffice_clean`, and `runtime_mins` were created or transformed specifically for visualization purposes and do not appear in raw API outputs.

- [README](README.md)
