
# Movie Watchlist React

This app helps you search any movie from the web any helps you keep track of your "Watchlist", "Watched".

You can remove any movie,move your movies from "Watched" to "Watchlist" and vice-versa and the total number of movie in list will be shown along with the movie cards.

It is very benefecial for movie addictive people who can't keep track of the movies they saw/willing to see.

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


  
