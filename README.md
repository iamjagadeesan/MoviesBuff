# MoviesBuff

MoviesBuff is a movie discovery application that allows users to browse trending movies and manage their personal watchlist. The app integrates with The Movie Database (TMDb) API to fetch popular movies and display them in an intuitive UI. Users can add movies to their watchlist, remove them, and filter the list by genre, search movies by title, and sort by rating or popularity.

## Features

- **Movie Discovery**: Fetches and displays trending movies from TMDb.
- **Watchlist Management**: Users can add or remove movies from their personalized watchlist.
- **Search Functionality**: Search for movies by title in the watchlist.
- **Genre Filtering**: Filter movies by genres (e.g., Action, Comedy, Drama, etc.).
- **Sorting Options**: Sort watchlist movies by rating or popularity (both ascending and descending).
- **Responsive Design**: Fully responsive UI for desktop, tablet, and mobile devices.

## Technologies Used

- **Frontend**: React.js
- **Routing**: React Router DOM
- **State Management**: React's useState, useEffect, useMemo, and useCallback hooks.
- **API Integration**: TMDb API for fetching movie data.
- **Local Storage**: Watchlist is stored in local storage so the data persists between sessions.
- **CSS Styling**: Custom CSS and responsive styling.

## Project Structure

- `App.js`: Main component handling routing and state for watchlist management.
- `Navbar.jsx`: Navigation bar with links to home and watchlist.
- `Movies.jsx`: Displays the list of trending movies fetched from TMDb.
- `Watchlist.jsx`: Manages the user's watchlist with genre filtering, search, and sorting functionality.
- `Banner.jsx`: Displays a prominent banner on the home page.
- `MoviesList.jsx`: Individual movie cards for displaying in the movie list.
- `Utility/genres.js`: Maps genre IDs to genre names for filtering movies.

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/iamjagadeesan/MoviesBuff.git
   ```

2. Navigate to the project directory:

   ```bash
   cd MoviesBuff
   ```

3. Install the dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm start
   ```

5. Open your browser and go to:

   ```
   http://localhost:3000
   ```

## API Integration

MoviesBuff uses the **TMDb API** to fetch popular movies. To enable the API:

1. Visit [The Movie Database (TMDb)](https://www.themoviedb.org/) and create an account.
2. Generate an API key from your TMDb account settings.
3. Replace the placeholder `api_key` in the `Movies.jsx` file with your TMDb API key.

```javascript
axios.get(`https://api.themoviedb.org/3/person/popular?api_key=YOUR_API_KEY&language=en-US&page=${page}`)
```

## Deployment

The project is hosted on GitHub Pages. You can access it [here](https://iamjagadeesan.github.io/MoviesBuff/).

## Future Improvements

- **User Authentication**: Add user login to save watchlists across devices.
- **More Movie Details**: Display detailed movie information like cast, crew, reviews, etc.
- **Pagination**: Improve the pagination system for browsing more movies.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

You can adjust the content based on your preferences, but this template should cover most of the important details for your project.
