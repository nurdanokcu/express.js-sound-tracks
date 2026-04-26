# Spiral Sounds

An Express.js application for an online classic vinyl store.

## Features

- Static frontend served from `public/`
- Products API under `/api/products`
- SQLite database support via `sqlite` and `sqlite3`

## Project structure

- `server.js` - main Express server
- `routes/products.js` - product API routes
- `controllers/productsControllers.js` - product request handlers
- `db/db.js` - SQLite database helper
- `public/` - static frontend assets
- `data.js`, `seedTable.js`, `createTable.js`, `logTable.js` - data and database scripts

## Requirements

- Node.js 18+ recommended

## Install

```bash
npm install
```

## Run

```bash
npm start
```

Then visit: `http://localhost:8000`

## Notes

- The app exposes the product API at `http://localhost:8000/api/products`
