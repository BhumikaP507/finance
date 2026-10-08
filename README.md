# Finance

A personal finance dashboard for reviewing income, expenses, and spending trends. Add transactions, compare totals, and explore the data through charts and filters.

## Features

- Summary cards for balance, income, and expenses
- Transaction entry for income and expenses
- Search, filter, and sort transactions
- Charts for balance over time and expenses by category
- Spending insights, including monthly comparison
- Viewer and admin display modes
- Browser storage using `localStorage`
- Responsive layout with light and dark themes

## Technology

- React 19
- Vite
- Recharts
- React Context API
- Plain CSS

## Run locally

You need Node.js and npm installed.

```bash
git clone https://github.com/BhumikaP507/finance.git
cd finance
npm install
npm run dev
```

Open the local address printed by Vite. The development server is configured for port 3000.

To create a production build:

```bash
npm run build
```

## How data works

The app starts with sample transactions from `src/utils/sampleTransactions.js`. Changes are stored in the browser's local storage, so they stay in that browser and are not synced to a server. Clearing site data resets the app to the sample transactions.

This version has no backend, API, authentication, or server-side database. The role selector changes the interface only; it is not an access-control feature.

## Project layout

```text
src/
  components/    Reusable dashboard sections and controls
  context/       Shared transaction, role, and filter state
  pages/         Dashboard page composition
  utils/         Currency formatting, sample data, and storage helpers
  App.jsx        App shell and theme control
  App.css        Dashboard styles and responsive layout
  index.css      Global browser styles
index.html       Vite HTML entry point and page metadata
```

## Learning project

This repository is a customized learning project based on the public [Finance Dashboard UI](https://github.com/AarushAnsh/Finance_Dashboard) reference. The layout, branding, color palette, metadata, and project documentation have been adapted for this repository. Extend it with your own features and be prepared to explain every part you include in a portfolio.
