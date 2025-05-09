---

# 🛍️ Product Catalog Application

## Overview

This is a simple product catalog web application with a React frontend and an Express + PostgreSQL backend. You can add products, view them, and search by name or description.

🔗 **Live Demo:** [https://shopify-frontend-y14y.onrender.com/](https://shopify-frontend-y14y.onrender.com/)

## Prerequisites

* **Node.js** (v14+)
* **npm** (v6+)
* **PostgreSQL** (v12+)

## Environment Variables

### Backend `.env`

```
DATABASE_URL=postgres://USER:PASSWORD@HOST:PORT/DB_NAME
PORT=3001
```

### Frontend `.env`

```
REACT_APP_API_URL=http://localhost:3001
```

## Database Setup

1. Start PostgreSQL.
2. Create a database:

   ```bash
   createdb product_catalog
   ```
3. Create the `products` table:

   ```sql
   CREATE TABLE products (
     id SERIAL PRIMARY KEY,
     name TEXT NOT NULL,
     price NUMERIC NOT NULL,
     description TEXT,
     image_url TEXT,
     created_at TIMESTAMP DEFAULT NOW()
   );
   ```

## Backend Setup

1. Go to the backend folder:

   ```bash
   cd backend
   ```
2. Install dependencies:

   ```bash
   npm install
   ```
3. Start the server:

   ```bash
   npm start
   ```

## Frontend Setup

1. Go to the frontend folder:

   ```bash
   cd frontend
   ```
2. Install dependencies:

   ```bash
   npm install
   ```
3. Start the development server:

   ```bash
   npm start
   ```

## Features

* ✅ Add new products
* 🔍 Search products by name or description
* 📋 View all products, sorted by newest

## Project Structure

```
backend/
  ├── index.js
  └── .env
frontend/
  ├── src/
  │   ├── App.js
  │   ├── api.js
  │   └── App.css
  └── .env
```

## License

MIT License

---


