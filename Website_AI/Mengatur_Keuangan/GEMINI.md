# GEMINI Project Context

## Project Overview

This project is a personal finance management web application. It allows users to track their income, expenses, and savings. The application is a single-page application (SPA) built with vanilla JavaScript, HTML, and Tailwind CSS. It uses Firebase for backend services, including:

*   **Firebase Authentication:** For user login and registration.
*   **Firestore:** As the database to store user data, transactions, budgets, and savings goals.
*   **Firebase Storage:** For storing user profile pictures.

The application provides features like transaction tracking, budget management, savings goals, recurring transactions, and data visualization of financial trends using Chart.js.

## Building and Running

This is a static web project that uses Firebase for its backend. To run the project, you need to have the Firebase CLI installed and configured.

1.  **Install Firebase CLI:**
    ```bash
    npm install -g firebase-tools
    ```

2.  **Login to Firebase:**
    ```bash
    firebase login
    ```

3.  **Serve the project locally:**
    ```bash
    firebase serve
    ```
    This will start a local server, and you can access the application at `http://localhost:5000`.

4.  **Deploy to Firebase Hosting:**
    ```bash
    firebase deploy
    ```

## Development Conventions

*   **Styling:** The project uses [Tailwind CSS](https://tailwindcss.com/) for styling. Utility classes are used directly in the HTML.
*   **JavaScript:** The project uses vanilla JavaScript with ES modules. The main logic is in `public/index.html` within a `<script type="module">` tag.
*   **Backend:** All backend services are provided by Firebase. The Firebase configuration is located in `public/index.html`.
*   **Data Visualization:** [Chart.js](https://www.chartjs.org/) is used for creating charts to visualize financial data.
