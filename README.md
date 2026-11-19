# Team 6 Movie Search

An interactive demonstration of our Johns Hopkins University movie data project.

## Use the demo

Open the GitHub Pages site to search movies by genre, minimum average rating, minimum rating count, and TMDb popularity. Results can be paginated and exported as CSV.

This site preserves the original search interface by **Nelson Yanes-Nunez**. The public demonstration runs in the browser against the submitted dataset. It needs no account, API key, Docker installation, or external query service.

## Dataset

- 9,742 movies and 100,836 historical MovieLens ratings, aggregated per movie.
- TMDb popularity snapshot dated October 25, 2026.
- Wikidata director information.
- No individual user rating records are included in this public demo.

The browser adapter preserves the original search parameters and result formatting. The submitted course project uses FastAPI, PostgreSQL, Docker, and an automated refresh pipeline. Those services are not run by GitHub Pages; this is a fixed snapshot demo.

## Team contributions

- **Haiyang Wu:** Part I data collection and validation, documentation, integrated testing, and final submission checks.
- **Chenye Shen:** Part II cleaning, PostgreSQL schema and loading, mapping review, and database documentation.
- **Nelson Yanes-Nunez:** Part III automation, API and original web interface, Docker integration, ERD redraw, and final packaging.

## Data credits

- MovieLens: F. Maxwell Harper and Joseph A. Konstan (2015), *The MovieLens Datasets: History and Context*. https://grouplens.org/datasets/movielens/
- This product uses TMDb data but is not endorsed or certified by TMDb. https://developer.themoviedb.org/docs/daily-id-exports
- Wikidata is available under CC0. https://www.wikidata.org/

## Local preview

Serve the repository with a local HTTP server, for example `python -m http.server 8080`, then open `http://localhost:8080`. Opening HTML files directly via `file://` will not load the dataset.
