
# Movie Watchlist React

This app helps you search any movie from the web any helps you keep track of your "Watchlist", "Watched".

You can remove any movie,move your movies from "Watched" to "Watchlist" and vice-versa and the total number of movie in list will be shown along with the movie cards.

It is very benefecial for movie addictive people who can't keep track of the movies they saw/willing to see.

## Demo

Insert gif or link to demo

  
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## API Reference

Api used : [The Movie DataBase](https://www.themoviedb.org/)

#### Get all movies

```http
  GET /api/movies
  
  https://api.themoviedb.org/3/search/movie?api_key=${REACT_APP_TMDB_KEY}&language=en-US&page=1&include_adult=false&query=${e.target.value}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |
| `movie name`      | `string` | **Required**. Name of movie to fetch |
  
## Run Locally

Clone the project

```bash
  git clone https://github.com/saikatXshrey/Movie-Watchlist-React.git
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```

  
## Deployment

To deploy this project run

```bash
  npm run deploy
```

  
## Lessons Learned

This project heavily uses "React Routing" as we needed to route between "Watchlist","Watched" and "Add" page without any reload so routing plays an important role here.

And ofcourse we needed to maintain states thats why "useState" was used. Along with "useEffect" for causing side effect and "fetch api" for fetching the movie according to our search from the "TMDb Api".

There was a major problem about the movie switching control i.e when we would want to remove a movie/move a movie from Watchlist to watched/vice-versa then there was a rising problem about "prop-drilling" which was solved using "Context Api" for removing/switching a GLobalCOntext was maintained.

And another thing was to store the the movies which we saved for Watchlist/Watched even if we close the app and for that i took the help of "localstorage".
  
