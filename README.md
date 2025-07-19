# BudgetBee

BudgetBee is a full-featured, single-page personal budget planner designed to run entirely in your browser. With no server or database required, you can instantly log income and expenses, categorize transactions, and view interactive tables and charts—all powered by LocalStorage for persistence. Add, edit, or delete entries on the fly, switch between light and dark modes, and back up your data via JSON export/import. Use BudgetBee to gain clarity on your financial habits: visualize monthly expense breakdowns with a pie chart, track your net balance over the last six months with a bar chart, and efficiently manage your cash flow in one professional, responsive interface.

---

## Features

- **Income & Expense Tracking**  
  Log any transaction with type (income or expense), category, amount, date, and optional note.

- **Interactive Table (Tabulator)**  
  Inline editing, sorting, filtering, and delete buttons for rapid CRUD operations.

- **Charts & Insights (Chart.js)**  
  - Pie chart for current month’s expense distribution by category  
  - Bar chart for net balance over the last six months

- **Data Persistence**  
  Transactions are saved in `localStorage`—no backend required.

- **Export & Import**  
  Download or upload your entire budget as a JSON file for backup, transfer, or synchronization.

- **Dark/Light Mode**  
  Toggle theme to suit your environment and reduce eye strain.

- **Client-Side Only**  
  Runs on any static hosting (GitHub Pages, Netlify, local HTTP server).

- **Cross-Device & Responsive**  
  Works flawlessly on desktop, tablet, and mobile browsers.

---

## Demo

View the live demo on GitHub Pages:  
https://bocaletto-luca.github.io/BudgetBee/index.html

---

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/bocaletto-luca/BudgetBee.git
   cd BudgetBee
   ```
2. **Serve with a static HTTP server**  
   - **Python 3**  
     ```bash
     python3 -m http.server 8000
     ```
   - **Node.js (http-server)**  
     ```bash
     npx http-server . -p 8000
     ```
3. **Open in browser**  
   Navigate to `http://localhost:8000/index.html`.

---

## Usage

1. **Add a transaction**  
   - Select **Expense** or **Income**  
   - Enter **Category**, **Amount**, **Date**, and optional **Note**  
   - Click **Add**

2. **Edit or delete**  
   - Inline edit any cell in the table  
   - Click the ❌ button to remove a transaction

3. **View charts**  
   - Pie chart shows expenses by category for the current month  
   - Bar chart shows net balance trend over the last six months

4. **Export / Import**  
   - Click **Export JSON** to download your data file  
   - Click **Import JSON** and select a file to restore

5. **Toggle Dark Mode**  
   - Click the 🌙 / ☀️ button to switch between dark and light themes

---

## Customization

- **Colors & Styles**  
  Edit CSS variables in the `<style>` block of `index.html`:
  ```css
  :root {
    --primary: #28a745;     /* Main brand color */
    --expense: #dc3545;     /* Expense bar color */
    --income: #17a2b8;      /* Income bar color */
    /* ... */
  }
  ```
- **Date Formatting**  
  Adjust the Day.js formatter calls in the script to change how dates are displayed.
- **Chart Options**  
  Modify the `new Chart()` configurations in the `updateCharts()` function for different visuals.

---

## File Structure

```
BudgetBee/
├── index.html       # Single-page app (HTML, CSS, JS)
├── LICENSE          # GNU GPL v3.0 license
└── README.md        # This documentation
```

---

## Contributing

Your feedback and contributions are welcome! To contribute:

1. **Fork** the repository  
2. **Create a feature branch**  
   ```bash
   git checkout -b feature/my-new-feature
   ```
3. **Commit your changes**  
   ```bash
   git commit -m "Add awesome feature"
   ```
4. **Push to your branch**  
   ```bash
   git push origin feature/my-new-feature
   ```
5. **Open a Pull Request** on GitHub

Please ensure compatibility across major browsers and maintain the existing code style.

---

## License

BudgetBee is licensed under the **GNU General Public License v3.0**.  
See the [LICENSE](LICENSE) file for full details.

---

## Author

**Bocaletto Luca**  
- GitHub: [@bocaletto-luca](https://github.com/bocaletto-luca)  
- Repository: [BudgetBee](https://github.com/bocaletto-luca/BudgetBee)
