# expense-manager-web
A single-page application for tracking personal expenses, built with HTML, CSS, and JavaScript. Features include recurring expenses, charts, budgeting, dark mode, and a responsive design.
# Modern Expense Manager

A single-page application (SPA) for tracking personal expenses, built entirely with HTML, CSS, and vanilla JavaScript. It features a responsive design, light/dark themes, data visualization with Chart.js, and local persistence using `localStorage`.

## Features

*   **Passcode Protection:** Optional 4 or 6-digit passcode stored locally.
*   **Dashboard:** Overview of total expenses, monthly totals with daily activity indicators, and per-account summaries.
*   **Expense Tracking:** Add, edit, and remove expenses via a modal form.
*   **Recurring Expenses:** Mark expenses as recurring with optional end dates. Recurring expenses are automatically calculated for relevant views (dashboard, calculator, charts). Option to remove recurring expenses entirely or just for a specific month.
*   **Tile View:** Interactive tile-based display of expenses for the selected month on the dashboard.
*   **Detailed Expense List:** Filterable, searchable, and sortable table view of all expenses.
*   **Data Visualization (Chart.js):**
    *   Line chart: Monthly expense trends.
    *   Pie chart: Expense distribution by category.
    *   Stacked Bar chart: Monthly expenses broken down by account.
    *   Scatter plot: Expense amount vs. day of the month.
*   **Budgeting:** Set a monthly budget and track spending against it.
*   **Remaining Money Calculator:** Calculates remaining funds based on current balances (combined or per-account) and projected expenses for a selected month.
*   **Settings:**
    *   Manage passcode.
    *   Manage custom categories and accounts.
    *   Data management (Clear all, Export/Import via CSV).
*   **Theming:**
    *   Light Mode (Custom warm theme).
    *   Dark Mode.
    *   Uses CSS variables and a consistent accent color (`#da7756`).
*   **Responsive Design:** Adapts layout for desktop and mobile devices using top navigation (desktop) and a mobile-specific navigation bar.
*   **Local Persistence:** All data (expenses, categories, accounts, settings) is saved in the browser's `localStorage`.

## Tech Stack

*   **HTML5:** Structure and content.
*   **CSS3:** Styling, layout (Flexbox), responsiveness (Media Queries), theming (CSS Variables).
*   **JavaScript (ES6+):** Application logic, DOM manipulation, event handling, data management, Chart.js integration.
*   **Chart.js:** Library for creating interactive charts.
*   **(Note:** This project is purely client-side and does *not* currently include Java or any server-side component.)

## Getting Started / Usage

1.  **Download:** Clone the repository or download the `app.html` file.
2.  **Open:** Simply open the `app.html` file in a modern web browser (like Chrome, Firefox, Edge, Safari).

No build process or server is required. All data is stored locally in your browser's `localStorage`. Clearing your browser data for the site will erase all saved expenses and settings.

## Screenshots

*(Suggestion: Add screenshots of the dashboard, charts, modal, and settings pages here)*

## Key Design Choices

*   **Single-File Structure:** Designed for simplicity, combining HTML, CSS, and JS in one file.
*   **Client-Side Logic:** All calculations and data handling occur within the browser.
*   **CSS Variables & Theming:** Leverages CSS variables for easy theme management (dark mode and a custom light mode). A strong accent color (`#da7756`) is used for visual consistency.
*   **Top Navigation:** Uses a horizontal top navigation bar for desktop and a dedicated mobile navigation bar instead of a traditional sidebar.
*   **Recurring Expense Handling:** Implements logic (`isExpenseActive`) to correctly display and calculate recurring expenses based on start date, end date, and specific monthly exclusions.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue.

## License
This project is licensed under the **GNU Affero General Public License v3** - see the [LICENSE] file for details.