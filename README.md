
# Movie Watchlist React

This app helps you search any movie from the web any helps you keep track of your "Watchlist", "Watched".

You can remove any movie,move your movies from "Watched" to "Watchlist" and vice-versa and the total number of movie in list will be shown along with the movie cards.

It is very benefecial for movie addictive people who can't keep track of the movies they saw/willing to see.

## Demo

Project Demo

https://user-images.githubusercontent.com/76695320/122665382-79ab5980-d1c4-11eb-939e-5d101c140d3d.mp4

  
## Screenshots

![Screenshot (1019)](https://user-images.githubusercontent.com/76695320/122665199-7fed0600-d1c3-11eb-8f80-9dfa308fdd11.png)

![Screenshot (1020)](https://user-images.githubusercontent.com/76695320/122665204-85e2e700-d1c3-11eb-8f6b-4d0aef3c4fde.png)

![Screenshot (1021)](https://user-images.githubusercontent.com/76695320/122665210-8aa79b00-d1c3-11eb-97a6-ab25d4d498e7.png)

![Screenshot (1022)](https://user-images.githubusercontent.com/76695320/122665212-9004e580-d1c3-11eb-950d-1593809a63aa.png)

![Screenshot (1023)](https://user-images.githubusercontent.com/76695320/122665215-94c99980-d1c3-11eb-918b-f8115331d53f.png)

![Screenshot (1024)](https://user-images.githubusercontent.com/76695320/122665224-9d21d480-d1c3-11eb-91b4-99f9d16d0617.png)

![Screenshot (1025)](https://user-images.githubusercontent.com/76695320/122665228-a27f1f00-d1c3-11eb-8616-de28da4f6a15.png)

![Screenshot (1027)](https://user-images.githubusercontent.com/76695320/122665231-a9a62d00-d1c3-11eb-82de-9bd364973e35.png)

![Screenshot (1028)](https://user-images.githubusercontent.com/76695320/122665237-ae6ae100-d1c3-11eb-9342-91898f5a930e.png)

![Screenshot (1029)](https://user-images.githubusercontent.com/76695320/122665241-b296fe80-d1c3-11eb-8b13-4ffc97237b39.png)


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
  
