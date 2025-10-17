# GitHub User Creation Date Checker

This is a single-page web application built with Bootstrap 5 that allows users to fetch the GitHub account creation date for a given username. By default, it displays the creation date for the 'google' GitHub account.

## Features

*   **Fetch GitHub User Data:** Retrieves the `created_at` date for any valid GitHub username.
*   **Default Username:** Automatically fetches data for 'google' on page load.
*   **Date Formatting:** Displays the creation date in `YYYY-MM-DD UTC` format.
*   **Error Handling:** Provides user-friendly messages for invalid usernames or API issues.
*   **Responsive Design:** Styled with Bootstrap 5 for a clean and responsive user interface.

## How to Use

1.  **Open `index.html`:** Simply open the `index.html` file in your web browser.
2.  **Default Display:** On load, the application will display the creation date for the 'google' GitHub account.
3.  **Enter Username:** Type a GitHub username into the input field.
4.  **Fetch Data:** Click the "Fetch Creation Date" button to retrieve and display the creation date for the entered username.

## Technical Details

*   **HTML5:** Standard page structure.
*   **Bootstrap 5 (CDN):** Used for styling and responsive layout.
*   **JavaScript:** Handles form submission, API calls, and DOM updates.
    *   Fetches data from `https://api.github.com/users/`.
    *   Uses `async/await` for asynchronous operations.
    *   `DOMContentLoaded` listener ensures all DOM elements are loaded before script execution.
    *   Date formatting leverages `Date.toISOString().split('T')[0]` to extract the `YYYY-MM-DD` part.

## Project Structure

*   `index.html`: The main and only HTML file containing all the structure, styling links, and JavaScript logic.
*   `README.md`: This file, providing information about the project.

## Getting Started (Development)

To run this project locally, you only need a web browser:

1.  Clone this repository (if applicable, otherwise save the `index.html` file).
2.  Open `index.html` in your browser.

No build steps or server are required as all resources are loaded via CDN and the script runs client-side.