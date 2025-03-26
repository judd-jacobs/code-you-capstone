# 🗂️ Data Dictionary

Below is a reference of key data fields used in this project, sourced and constructed from Wikipedia, TMDb API, and OMDb API. These fields are used across core dataframes like `omdb_metadata_clean` and `tmdb_genre_results`, as well as in merged outputs used for analysis.

---

## 📦 `omdb_metadata_clean`

| Column Name       | Type       | Description                                                                 |
|-------------------|------------|-----------------------------------------------------------------------------|
| `film`            | object     | Title of the film                                                           |
| `year`            | int64      | Year of the film's release                                                  |
| `title_api`       | object     | Title as returned by OMDb API                                               |
| `rated`           | object     | MPAA rating (e.g., PG-13, R)                                                |
| `released`        | object     | Official release date                                                       |
| `runtime`         | object     | Raw runtime string from OMDb (e.g., "123 min")                              |
| `director`        | object     | Director(s) of the film                                                     |
| `writer`          | object     | Writer(s) of the film                                                       |
| `actors`          | object     | Primary actors featured                                                     |
| `plot`            | object     | Short plot summary                                                          |
| `language`        | object     | Primary languages spoken in the film                                        |
| `country`         | object     | Countries involved in production                                            |
| `awards`          | object     | Award summary string from OMDb                                              |
| `poster`          | object     | Poster image URL                                                            |
| `ratings`         | object     | List of external rating sources (IMDB, Metacritic, etc.)                    |
| `metascore`       | float64    | Metacritic score                                                            |
| `imdbRating`      | float64    | IMDb rating (0–10 scale)                                                    |
| `imdbVotes`       | Int64      | Number of votes counted on IMDb                                             |
| `imdbID`          | object     | IMDb ID identifier                                                          |
| `type`            | object     | Type of media (e.g., "movie")                                               |
| `boxOffice`       | object     | Raw box office string (e.g., "$123,456,789")                               |
| `response`        | object     | API success indicator                                                       |
| `runtime_mins`    | Int64      | Parsed runtime in minutes                                                   |
| `boxOffice_clean` | float64    | Box office revenue as float (USD)                                           |
| `decade`          | int64      | Decade derived from film release year                                       |
| `winner`          | bool       | `True` if the film won Best Picture, `False` if it was only a nominee       |

---

## 📦 `tmdb_genre_results`

| Column Name | Type     | Description                                |
|-------------|----------|--------------------------------------------|
| `film`      | object   | Title of the film                         |
| `year`      | int64    | Year of the film's release                |
| `genre`     | object   | List of genre(s) returned from TMDb API   |

---

## 🧮 Temporary & Merged Analysis Frames
These datasets are generated for specific visualizations and analysis steps. They often include columns derived from one or more sources:

| Column Name       | Type     | Description                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| `status`          | object   | Either "Winner" or "Nominee" (derived from `winner` boolean)               |
| `formatted`       | object   | Human-readable string of revenue for labeling purposes (e.g., "$140M")     |
| `count`           | int64    | Count of rows when grouping by genre, decade, or status                     |
| `genre_exploded`  | object   | Exploded rows for multi-genre films (used in heatmaps and bar charts)       |

These fields are dynamically generated and do not appear in the persistent database tables.

---

📌 Note: Fields such as `genre`, `boxOffice_clean`, and `runtime_mins` were created or transformed specifically for visualization purposes, and do not appear in the raw API response.
