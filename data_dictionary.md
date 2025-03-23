
# 📘 Data Dictionary — `academy_awards.db`

## 🗂️ Table: `movies`

One row per Best Picture–nominated film, including metadata and outcome.

| Column Name       | Type     | Description |
|-------------------|----------|-------------|
| Film              | TEXT     | Title of the film |
| Year              | INTEGER  | Year of nomination or win |
| Status            | TEXT     | Award outcome (`Winner` or `Nominee`) |
| Title             | TEXT     | Official OMDb API title |
| Rated             | TEXT     | Film rating (e.g., PG-13, R) |
| Released          | TEXT     | Release date |
| Runtime (mins)    | INTEGER  | Runtime in minutes |
| Genre             | TEXT     | Raw genre string from OMDb (not normalized) |
| Director          | TEXT     | Director(s) of the film |
| Writer            | TEXT     | Writer(s) of the film |
| Actors            | TEXT     | Main cast |
| Plot              | TEXT     | Short description of the film |
| Language          | TEXT     | Languages used |
| Country           | TEXT     | Country of origin |
| Awards            | TEXT     | Awards summary from OMDb |
| Poster            | TEXT     | URL to poster image |
| Ratings           | TEXT     | Ratings breakdown (e.g., Rotten Tomatoes, Metacritic) |
| Metascore         | INTEGER  | Metacritic score (0–100) |
| imdbRating        | FLOAT    | IMDb rating (0–10) |
| imdbVotes         | INTEGER  | Number of votes on IMDb |
| imdbID            | TEXT     | IMDb ID (e.g., tt1234567) |
| Type              | TEXT     | Content type (`movie`) |
| BoxOffice         | FLOAT    | Box office revenue in USD |
| Response          | TEXT     | OMDb API response status (`True` or `False`) |

---

## 🗂️ Table: `movie_genres`

One row per movie-genre pair.

| Column Name | Type    | Description |
|-------------|---------|-------------|
| Film        | TEXT    | Film title (foreign key to `movies.Film`) |
| Year        | INTEGER | Film year (foreign key to `movies.Year`) |
| Genre       | TEXT    | One genre assigned to the film (e.g., Drama, Comedy) |

---

## 🔗 Notes

- The combination of `Film` and `Year` is used as a composite key for linking tables.
- Genre is **normalized** so you can group, count, and analyze genre trends efficiently.
- If needed, this schema can be expanded to include nominations or categories as a third table.
