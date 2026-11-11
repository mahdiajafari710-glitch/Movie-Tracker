# MovieTrack – Project Planning

## Project Overview

MovieTrack is a movie-tracking website that helps users explore movies, search for titles, keep a personal watchlist, and save their favorite movies. The project will be built with HTML, CSS, and JavaScript.

For the first version, movie information and posters will be added manually as sample data. An external movie API will **not** be connected yet. API integration can be added later after learning it with the instructor.

## 1. List the Nouns (Data)

1. Movie
2. Movie title
3. Movie poster
4. Release date
5. Rating
6. Overview or description
7. Genre
8. Movie ID
9. Search input
10. My List
11. Favorites
12. Watched status
13. Dashboard
14. Explore page
15. About page
16. User's theme preference (light or dark)

## 2. Identify Their Data Types

| Property | Data Type | Example |
|---|---|---|
| id | Number | 1 |
| title | String | "Inception" |
| poster | String | "images/inception.jpg" |
| releaseDate | String | "2010-07-16" |
| rating | Number | 8.8 |
| overview | String | "A skilled thief enters people's dreams." |
| genre | Array | ["Action", "Sci-Fi"] |
| isFavorite | Boolean | true |
| isInMyList | Boolean | false |
| isWatched | Boolean | false |
| searchQuery | String | "Inception" |
| theme | String | "dark" |

## 3. List the Verbs (Actions)

1. Display movies on the Dashboard.
2. Explore and browse available movies.
3. Search for a movie by its title.
4. Display the movie poster and information.
5. Open a movie's details.
6. Add a movie to My List.
7. Remove a movie from My List.
8. Add a movie to Favorites.
9. Remove a movie from Favorites.
10. Mark a movie as watched.
11. Filter or sort the movie list.
12. Navigate between Dashboard, My List, Favorites, Explore, and About.
13. Switch between light mode and dark mode.
14. Save the user's lists and preferences in LocalStorage.

## 4. Identify Inputs and Outputs

| Function | Input | Output |
|---|---|---|
| displayMovies() | Movie data | Movies displayed on the page |
| searchMovies() | Search text and movie data | Movies matching the title |
| showMovieDetails() | Movie ID | Selected movie's details |
| addToMyList() | Movie ID | Movie added to My List |
| removeFromMyList() | Movie ID | Movie removed from My List |
| addToFavorites() | Movie ID | Movie added to Favorites |
| removeFromFavorites() | Movie ID | Movie removed from Favorites |
| markAsWatched() | Movie ID | Movie marked as watched |
| filterMovies() | Genre or filter option | Filtered movies |
| sortMovies() | Movie data and sort option | Sorted movies |
| changeTheme() | Theme name | Page displayed in the selected theme |
| saveData() | User's lists and preferences | Data saved in LocalStorage |
| loadData() | LocalStorage data | Previously saved data loaded |

## 5. Add Conditions for Invalid Inputs

1. The search input should not be empty when the user submits a search.
2. If no movie matches the search text, display a message such as "No movies found."
3. A movie must have a valid ID and title.
4. A movie should not be added to My List more than once.
5. A movie should not be added to Favorites more than once.
6. Removing a movie should only affect the selected movie.
7. The rating must be a valid number within the chosen rating scale (for example, 0 to 10).
8. If a poster image cannot be loaded, display a default placeholder image.
9. If LocalStorage has no saved data, load the default sample movie data.
10. The theme value must be either "light" or "dark".

## Movie Data

| Property | Type | Example |
|---|---|---|
| id | Number | 1 |
| title | String | "Interstellar" |
| poster | String | "images/interstellar.jpg" |
| releaseDate | String | "2014-11-07" |
| rating | Number | 8.7 |
| overview | String | "A team travels through space to find a new home for humanity." |
| genre | Array | ["Adventure", "Drama", "Sci-Fi"] |

Example sample movies for the first version:

- Inception
- Interstellar
- The Dark Knight
- Avengers: Endgame

## Main Website Sections

| Section | Purpose |
|---|---|
| Dashboard | Shows the main movie content and an overview |
| My List | Shows movies saved to the user's watchlist |
| Favorites | Shows movies marked as favorites |
| Explore | Allows users to browse and search movies |
| About | Provides information about the MovieTrack project |

## Application Actions

| Function | Parameters | Output |
|---|---|---|
| searchMovies() | searchQuery, movies | Matching movies |
| addToMyList() | movieId | Updated My List |
| addToFavorites() | movieId | Updated Favorites |
| markAsWatched() | movieId | Updated watched status |
| filterMovies() | movies, genre | Filtered movies |
| sortMovies() | movies, sortBy | Sorted movies |
| saveData() | key, data | Data saved in LocalStorage |
| loadData() | key | Saved data returned |

## Technologies

- **HTML:** Creates the structure of the website.
- **CSS:** Designs the layout, colors, and responsive appearance.
- **JavaScript:** Handles searching, movie lists, favorites, filters, and other interactions.
- **LocalStorage:** Saves the user's lists and preferences in the browser.

## Important Project Note

In the first version, movie posters and information will be stored as manually written sample data. No movie API will be connected at this stage. API integration can be studied and added later with the instructor.

## Conclusion

This plan identifies the main data, data types, actions, inputs, outputs, and validation conditions for MovieTrack. It provides a clear starting point before building the website with HTML, CSS, and JavaScript.
