# WorldExplorer – Client

Web front end for **WorldExplorer**, an interactive platform for exploring countries around the world. It talks to an ASP.NET Core REST API through jQuery/AJAX.

> Built as a pair project at Ruppin Academic Center. Server repository: [TT_Proj_Server-updated_Final-](https://github.com/TalVaizbord/TT_Proj_Server-updated_Final-)

## Live Demo

**[Open the live site](https://proj.ruppin.ac.il/cgroup29/test2/tar2/Pages/index.html)**

Demo account (regular user, no admin rights):

- Email: `123@gmail.com`
- Password: `122112`

## Screenshots
### Home
![Home Screen](Screenshots/Home%20Screen.png)

### Favorites map
![Favorites Map](Screenshots/Favorites%20Map.png)

### Quizzes
![Quiz Page](Screenshots/Quiz%20Page.png)
![Capital City Quiz](Screenshots/Capital%20City%20Quiz.png)

### Pubs map
![Pubs Map](Screenshots/Pubs%20Map.png)

## Features

- **Country explorer** – browse all countries with live search, filtering (region, language, currency, population, area) and sorting.
- **Country details** – flag, capital, population, area, languages and currency, plus community comments (add, edit, delete).
- **AI trip planner** – generates a travel itinerary for a chosen country through the server's AI endpoint.
- **Interactive world map and 3D globe** – mark countries as favorites, travel destinations or visited.
- **Personal lists** – manage and move countries between your lists; changes are saved to the database.
- **Quizzes** – timed capital-city and flag quizzes with points and a top-10 leaderboard.
- **Pubs map** – search any city and see nearby pubs and bars on a map (Leaflet, OpenStreetMap Nominatim geocoding, Overpass API, marker clustering).
- **Accounts and admin** – registration, login, locked-account handling, and an admin dashboard for user management and statistics.

## Tech Stack

- HTML5, CSS3, JavaScript (ES6)
- jQuery and AJAX for all server communication
- Leaflet and Leaflet.markercluster for maps
- jsVectorMap for the interactive world map
- globe.gl and Three.js for the 3D globe
- OpenStreetMap Nominatim and Overpass APIs

## Project Structure

```
├── index.html          # Home page
├── Pages/              # login, register, my-lists, quizzes, nightlife, admin
├── JS/AjaxCall.js      # AJAX calls and page logic
└── CSS/StyleSheet.css  # Styling
```

## Getting Started

1. Run the [server](https://github.com/TalVaizbord/TT_Proj_Server-updated_Final-) locally (see its README).
2. In `JS/AjaxCall.js`, set `BASE_API_URL` to your local API address, for example `https://localhost:7234/api/`.
3. Open `index.html` in a browser, or run the solution in Visual Studio.
