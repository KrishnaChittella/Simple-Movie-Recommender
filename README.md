Movie Recommender System

This is a Movie Recommender System built using Python, Streamlit, and TMDb API. The system recommends movies to users based on their selected choice and displays the posters of recommended movies.

Features

Recommends movies similar to the selected movie.

Fetches movie posters using the TMDb API.

Interactive and user-friendly interface built with Streamlit.


Project Structure

Movies-Recommendor/
│
├── app/
│   ├── app.py                   # Main Streamlit app file
│   └── requirements.txt         # Python dependencies
│
├── models/
│   ├── movies_dict.pkl          # Serialized movie data
│   ├── similarity.pkl           # Precomputed similarity matrix
│
├── README.md                    # Project documentation
└── .gitignore                   # Ignored files and folders

How It Works

The system uses a precomputed similarity matrix (similarity.pkl) to find movies similar to the selected movie.

Movie details (e.g., title, poster) are fetched using the TMDb API.

The Streamlit interface allows users to interact with the app seamlessly.

Installation

Prerequisites

Python 3.7+

A TMDb API key (Get yours from here)

Steps

Clone the repository:

git clone https://github.com/yourusername/Movies-Recommendor.git
cd Movies-Recommendor

Install dependencies:

pip install -r app/requirements.txt

Add your TMDb API key:

Replace {YOUR API KEY} in app.py with your actual API key.

Run the app:

streamlit run app/app.py

Open the app in your browser at http://localhost:8501.

Usage

Select a movie from the dropdown menu.

Click "Show Recommendation" to view the recommended movies and their posters.

Example Screenshot

[Insert a screenshot of your app interface here]

Technologies Used

Python

Streamlit for building the web app

pandas for data manipulation

pickle for loading precomputed data

requests for TMDb API integration

Future Enhancements

Add multiple recommendation algorithms (e.g., content-based and collaborative filtering).

Deploy the app online (e.g., Streamlit Cloud or Heroku).

Improve the user interface and responsiveness.

Handle edge cases for movies without posters or data.

Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

License

This project is licensed under the MIT License.

Acknowledgments

The Movie Database (TMDb) for the API and data.

Streamlit for the interactive interface.

