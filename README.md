# Spiral Sounds

A classic vinyl storefront built with Express.js, SQLite, and a static frontend.

## Features

- Static storefront served from `public/`
- Product catalog API with genre filtering and search
- User registration, login, and session-based authentication
- Protected cart endpoints for adding, viewing, and removing items
- SQLite persistence via `database.db`

## Includes

- `server.js` - Express server and route mounting
- `routes/` - REST API route definitions for products, auth, cart, and current user
- `controllers/` - request handlers for product browsing, auth, and cart operations
- `db/db.js` - SQLite connection helper
- `public/` - frontend pages, client scripts, and styles
- `createTable.js` - creates the product table in `database.db`
- `seedTable.js` - inserts sample vinyl products into the database
- `data.js` - sample vinyl catalog used by `seedTable.js`
- `database.db` - prebuilt database file containing products, users, and cart items

## Requirements

- Node.js 18 or newer

## Installation

```bash
npm install
```

## Environment

The server uses `express-session` for authentication, and supports an optional session secret via environment variable:


## Database setup

The repository includes a working `database.db` file. To recreate product data manually:

```bash
node createTable.js
node seedTable.js
```

## Run

```bash
npm start
```

Then visit:

```text
http://localhost:8000
```


## Notes

- The app runs on port `8000` by default.
- Sessions are stored in memory, which is suitable for development but not production.
- Passwords are hashed using `bcryptjs`.
