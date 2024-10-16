# JS30-6-TypeAhead

# Type Ahead 👀

This project is part of Wes Bos's **"30 Days of JavaScript"** challenge, specifically Day 6: **Type Ahead**. It implements a live search feature that displays city and state suggestions as the user types, using data from a JSON file.

## Project Overview

The **Type Ahead** project dynamically filters and displays cities or states that match the user's input. As the user types, it suggests possible matches based on a large dataset of U.S. cities and states. The matched text is highlighted within the suggestions.

### Features

- **Live Search**: As you type, the input is matched against a dataset of cities and states.
- **Highlighted Matches**: The part of the city or state that matches the user's input is highlighted.
- **Comma-formatted Population**: The population numbers are formatted with commas for readability.
- **Real-time Suggestions**: Displays suggestions based on input with every keystroke.

## Demo

Type the name of a city or state into the search bar, and a list of matching results will appear. The matches are highlighted, and the population of each result is displayed.

## Technologies Used

- **HTML**: For structuring the page.
- **CSS**: For basic styling of the search form and results (assumed to be in `style.css`).
- **JavaScript**:
  - Fetching data from an external API.
  - Filtering and displaying search results in real time.
  - Using regular expressions to highlight matches.

## How It Works

1. **Data Fetching**: The list of cities is fetched from an external JSON file hosted on GitHub. This dataset contains U.S. cities and their populations.
2. **Search Functionality**:
   - When the user types, JavaScript filters the cities and states that match the input using regular expressions.
   - The matches are displayed below the input field, with the matched part of the word highlighted.
3. **Displaying Results**: The results are shown in an unordered list (`<ul>`), with the matching text highlighted and the population of each city shown.

## Code Breakdown

- **`fetch()`**: Fetches a list of cities and states from a remote JSON endpoint.
- **`findMatches()`**: Filters the list of cities and states based on user input using a regular expression.
- **`displayMatches()`**: Displays the filtered cities and states in the DOM, with the matching portion of the text highlighted and the population formatted with commas.

## How to Run the Project

1. Download or clone the repository.
2. Open the `index.html` file in your browser.
3. Start typing in the search bar, and you’ll see live suggestions based on your input.

## Credits

This project is part of Wes Bos's [JavaScript 30](https://javascript30.com/) course. It's a great way to practice JavaScript and learn useful web development concepts.
