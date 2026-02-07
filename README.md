# End-to-End Movie Recommender System

A content-based movie recommender system that suggests movies similar to the one selected by the user. The application utilizes Natural Language Processing (NLP) techniques and Cosine Similarity to recommend movies based on their plot, cast, genres, and other metadata.

## Features

- **Movie Recommendation**: Recommend top movies based on similarity.
- **Search Functionality**: Search for movies from a large database.
- **Detailed Movie Info**: Display cast, genres, rating, and runtime.
- **Sentiment Analysis**: Analyze user reviews from IMDb to categorize them as 'Good' or 'Bad' using a trained NLP model.
- **Web Interface**: Built with Flask for a responsive and interactive user experience.

## Tech Stack

- **Python**: Core programming language.
- **Flask**: Web framework for the backend.
- **Pandas & NumPy**: Data manipulation and numerical operations.
- **Scikit-learn**: Machine learning library for vectorization and similarity calculation.
- **BeautifulSoup**: Web scraping for fetching reviews.
- **NLTK**: Natural Language Toolkit for text processing.
- **HTML/CSS/Bootstrap**: Frontend for the user interface.

## Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/yourusername/End_to_End_Movie_Recommendation_System.git
    cd End_to_End_Movie_Recommendation_System
    ```

2.  Create a virtual environment (optional but recommended):
    # if going to use uv.lock file (more convenient)
    first install uv using pip or visit uv site: [uv package guide](https://docs.astral.sh/uv/)
    ```bash
    # Using uv
    There is pyproject.toml file, you can directly run
    check: uv --version
    uv venv .venv
    uv sync (install required packages and dependencies)
    
    # Or using python
    python -m venv .venv
    # Windows
    .venv\Scripts\activate
    # macOS/Linux
    source .venv/bin/activate
    ```

4.  Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  Run the application:
    ```bash
    python app.py
    ```

2.  Open your browser and navigate to `http://localhost:5000` to access the application.

## Project Structure

- `app.py`: Main Flask application file containing routes and logic.
- `templates/`: HTML templates for the web interface.
- `static/`: Static assets (CSS, JS, images).
- `Artifacts/`: Contains the dataset (`main_data.csv`) and trained models (`nlp_model.pkl`, `tranform.pkl`).
- `requirements.txt`: List of Python dependencies.

## Contributing

Contributions are welcome! Please check the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## Data Sources & Attribution

This project uses data from [IMDb](https://www.imdb.com/) and [The Movie Database (TMDB)](https://www.themoviedb.org/).
This product uses the TMDB API but is not endorsed or certified by TMDB.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
