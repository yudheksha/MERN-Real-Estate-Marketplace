# MERN Real Estate Marketplace (Avenue Estate)

A full-stack real estate marketplace built with the MERN stack. Users can sign up or sign in (including Google OAuth), create property listings with images, browse and search listings, and contact landlords from the listing page.

## Features
- Authentication
  - Email and password signup/signin
  - Google OAuth (Firebase)
  - JWT-based auth (stored in an httpOnly cookie)
- Listings
  - Create, edit, and delete your own listings
  - Upload up to 6 images per listing (Firebase Storage)
  - Listing details page with image carousel and share link
- Search and discovery
  - Filter by rent/sale, offer, parking, furnished
  - Sort by price or latest
  - Pagination with "Show more"
- Contact landlord
  - Generates a mailto message to the listing owner

## Tech stack
- Frontend: React (Vite), Tailwind CSS, Redux Toolkit, React Router, Swiper
- Backend: Node.js, Express, MongoDB (Mongoose)
- Auth and storage: JWT, Firebase Auth (Google), Firebase Storage

## Project structure
- `api/` - Express API, routes, controllers, models
- `client/` - React frontend (Vite)

## Environment variables

Create a `.env` file in the project root:
```env
MONGO=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

