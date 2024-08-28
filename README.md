# Movie Recommender System
A content based movie recommender system using cosine similarity.

This project is a Movie Recommender System that suggests movies similar to the user's input. The system uses the [TMDb API](https://www.themoviedb.org/documentation/api) to fetch movie posters and is built using Streamlit for the web interface.

## Features

- Recommends movies based on similarity to a selected movie.
- Fetches movie posters dynamically using the TMDb API.
- User-friendly interface with movie selection from a dropdown.

## Prerequisites

To run this project, you need the following installed:
- Google Collab/Jupyter Notebook
- Python 3.x
- Streamlit
- Requests
- Pickle

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/movie-recommender-system.git
   cd movie-recommender-system
   ```

2. **Install the required packages:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Obtain TMDb API Key:**

   - Visit [TMDb API](https://www.themoviedb.org/documentation/api) and sign up for an API key.
   - Replace the API key in the script with your key:  
     ```python
     api_key = "your_api_key"
     ```

4. **Prepare the data:**

   - Ensure you have the required pickled files (`movie_list.pkl` and `similarity.pkl`) in the `model/` directory.

## Usage

1. **Run the Streamlit app:**

   ```bash
   streamlit run app.py
   ```

2. **Select a movie:**
   - Type or select a movie from the dropdown.

3. **Get recommendations:**
   - Click on the "Show Recommendation" button to display similar movies along with their posters.

## Project Structure

- `app.py`: Main application script.
- `model/movie_list.pkl`: Pickle file containing the list of movies.
- `model/similarity.pkl`: Pickle file containing the similarity matrix.
- `requirements.txt`: Contains all the required dependencies.

## Example

![Example](path/to/example_image.png)

## Acknowledgments

- This project uses data from [TMDb](https://www.themoviedb.org/).

## License

This project is licensed under the MIT License.

