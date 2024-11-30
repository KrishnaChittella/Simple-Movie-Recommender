# Movie Recommender System 🎥🍿

This is a **Movie Recommender System** built using **Python**, **Streamlit**, and **TMDb API**. The system recommends movies to users based on their selected choice and displays the posters of recommended movies.

## Features 🚀

- Recommends movies similar to the selected movie.
- Fetches movie posters using the [TMDb API](https://www.themoviedb.org/).
- Interactive and user-friendly interface built with Streamlit.

## Demo 🎬

[Add a link to a deployed version of your app (e.g., Streamlit Cloud, Heroku, etc.)]

## Project Structure 📂
```
Movies-Recommendor/ 
│  
├── requirements.txt 
│ 
├── app/ 
|   │ 
|   └── app.py 
│ 
└── models/ 
|   │ 
|   ├── movies_dict.pkl 
|   │ 
|   └── similarity.pkl 
│ 
└── README.md
```

## How It Works 🛠️

1. The system uses a precomputed similarity matrix (`similarity.pkl`) to find movies similar to the selected movie.
2. Movie details (e.g., title, poster) are fetched using the TMDb API.
3. The Streamlit interface allows users to interact with the app seamlessly.

## Installation 📥

### Prerequisites

- Python 3.7+
- A TMDb API key (Get yours from [here](https://developers.themoviedb.org/3/getting-started/introduction))

### Steps

1. Clone the repository:
   ```git clone https://github.com/yourusername/Movies-Recommendor.git```
   ```cd Movies-Recommendor```
2. Install dependancies:
    ```pip install -r requirements.txt```
3. Add your TMDb API:
    Replace {YOUR API KEY} in app.py with your actual API key.
4. Run the app:
    ```streamlit run app/app.py```
5. Open the app in your browser at http://localhost:8501

### Usage
1. Select a movie from the dropdown menu
2. Click "Show Recommendation" to view the recommended movies and their posters

### Technologies Used
-  Python

-  Streamlit for building the web app

-  pandas for data manipulation

-  pickle for loading precomputed data

-  requests for TMDb API integration

### Future Enhancements
-  Add multiple recommendation algorithms (e.g., content-based and collaborative filtering).

-  Deploy the app online (e.g., Streamlit Cloud or Heroku).

-  Improve the user interface and responsiveness.

-  Handle edge cases for movies without posters or data.
