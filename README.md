# Laravel + React Boilerplate

## Overview

This boilerplate combines the power of Laravel (PHP) for backend APIs and React (TypeScript) for a modern frontend, using Vite for fast development and hot module replacement.

## Getting Started

1. **Install PHP dependencies:**

   ```sh
   composer install
   ```

2. **Install Node.js dependencies:**

   ```sh
   npm install
   ```

3. **Copy environment files and configure:**

   ```sh
   cp .env.example .env
   # By default, the project uses SQLite for local development.
   # No extra setup is needed for the database.
   # If you want to use MySQL, update the DB_* variables in .env and ensure MySQL is running.
   ```

4. **Generate application key:**

   ```sh
   php artisan key:generate
   ```

5. **Run database migrations:**

   ```sh
   php artisan migrate
   # For SQLite, the database file will be created automatically at database/database.sqlite
   ```

6. **Build frontend assets for Laravel integration:**

   ```sh
   npm run build
   # This step generates the Vite manifest required by Laravel for production or SSR.
   ```

7. **Start Laravel backend server:**

   ```sh
   php artisan serve
   ```

8. **Start frontend development server:**
   ```sh
   npm run dev
   ```

## Usage

- Backend API: [http://localhost:8000](http://localhost:8000)
- Frontend: [http://localhost:5173](http://localhost:5173) (default Vite port)

## Features

- Laravel 10+ backend
- React + TypeScript frontend
- Vite for fast builds and HMR
- Inertia.js for seamless SPA experience
- Authentication (Laravel Fortify)
- Example components and layouts

## Project Structure

- `app/` - Laravel backend code
- `resources/js/` - React frontend code
- `routes/` - Laravel route definitions
- `public/` - Public assets and entry points

## Useful Commands

- Run tests:
  ```sh
  php artisan test
  npm test
  ```
- Build frontend for production:
  ```sh
  npm run build
  ```

---

For more details, see the documentation for [Laravel](https://laravel.com/docs) and [Vite](https://vitejs.dev/).
