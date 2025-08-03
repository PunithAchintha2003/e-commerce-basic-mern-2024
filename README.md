# e-commerce-website-mern-2024

MERN E-Commerce Website Tutorial 2024

[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)
- [Scripts](#scripts)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)

## Overview
A full-stack e-commerce web application built with the MERN stack (MongoDB, Express.js, React, Node.js). This project demonstrates a basic online store with product management, shopping cart, and admin dashboard. It is designed for learning and as a boilerplate for new e-commerce projects.

## Features
- User authentication (JWT-based)
- User registration and login
- Product listing, details, and search
- Shopping cart and checkout
- Admin dashboard for product management
- Product image upload (Multer)
- Responsive design (mobile-friendly)
- RESTful API

## Tech Stack
- **Frontend:** React, Vite (admin), Create React App (frontend)
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JWT
- **File Uploads:** Multer

## Project Structure
- `frontend/` - Main user-facing React app
- `admin/` - Admin dashboard (React + Vite)
- `backend/` - Node.js/Express API server

## Getting Started
### Prerequisites
- Node.js (v16+ recommended)
- npm or yarn
- MongoDB (local or cloud)

### Installation
1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd e-commerce-basic-mern-2024
   ```
2. **Install dependencies for each part:**
   ```bash
   cd backend && npm install
   cd ../frontend && npm install
   cd ../admin && npm install
   ```
3. **Set up environment variables:**
   - Create a `.env` file in `backend/` with your MongoDB URI and JWT secret (see [Environment Variables](#environment-variables)).

### Running the App
1. **Start the backend server:**
   ```bash
   cd backend
   npm start
   ```
2. **Start the frontend app:**
   ```bash
   cd ../frontend
   npm start
   ```
3. **Start the admin dashboard:**
   ```bash
   cd ../admin
   npm run dev
   ```

## Usage
- Access the user app at `http://localhost:3000` (default)
- Access the admin dashboard at `http://localhost:5173` (default)
- The backend API runs on `http://localhost:5000` (default)

## API Endpoints
> **Note:** See backend code for full details. Example endpoints:

- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `GET /api/products` - List all products
- `GET /api/products/:id` - Get product details
- `POST /api/products` - Add product (admin)
- `PUT /api/products/:id` - Update product (admin)
- `DELETE /api/products/:id` - Delete product (admin)

## Environment Variables
Create a `.env` file in the `backend/` directory with the following:

```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

## Scripts
- **backend:** `npm start` (starts API server)
- **frontend:** `npm start` (starts user app)
- **admin:** `npm run dev` (starts admin dashboard)

## Folder Structure
```
/ (root)
  |-- backend/      # Express API server
  |-- frontend/     # User-facing React app
  |-- admin/        # Admin dashboard (Vite + React)
```

## Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request
