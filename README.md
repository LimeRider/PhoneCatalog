#  Nice Gadgets — Phone Catalog

## Introduction

Welcome to **Nice Gadgets** — an online catalog of phones, tablets, and accessories built with React and TypeScript. Users can browse products by category, view detailed specifications, and manage a cart and favorites list while browsing.

The project focuses on real-world SPA concerns: routing, data fetching, client-side filtering/sorting, and state that persists across page reloads.

** [Live Demo](https://limerider.github.io/react_phone-catalog/)**

## Key Features

- **Home Page** — highlighted sections such as "Hot prices," "Brand new models," and "Shop by category"
- **Category Pages** — browse Phones, Tablets, and Accessories, each fetched dynamically from the API
- **Product Details Page** — full specifications, image gallery with color and capacity selection, and related products
- **Filtering & Sorting** — sort by price, newest, or alphabetically, and search products by name, synced with URL query parameters
- **Pagination** — configurable items-per-page and page navigation for long product lists
- **Cart** — add, remove, and adjust item quantities; totals update automatically
- **Favorites** — save products to a favorites list for later
- **Persistent State** — cart and favorites are stored in `localStorage` and survive page reloads
- **Loaders & Empty States** — loading indicators while fetching data, and clear messaging when no products match a filter
- **404 Page** — a `NotFoundPage` with a link back to the home page for any unmatched route
- **Responsive Design** — adapts across mobile, tablet, and desktop breakpoints

## Key Challenges

- **Data Fetching & Caching** — retrieving product lists and individual product details from the API without redundant requests
- **URL as Source of Truth** — keeping filter, sort, and pagination state in sync with URL query parameters so pages are shareable and bookmarkable
- **Global State Management** — sharing cart and favorites state across independent routes without prop drilling
- **Type Safety** — modeling API responses and component props accurately with TypeScript
- **Responsive Layout** — building a product grid and details page that adapt cleanly across screen sizes

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/LimeRider/react_phone-catalog.git
   ```

2. Navigate to the project directory:
   ```bash
   cd react_phone-catalog
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Start the local development server:
   ```bash
   npm start
   ```

## Usage

1. Open the local server URL shown in your terminal (usually `http://localhost:3000` or similar).
2. Browse products from the Home page or the Phones / Tablets / Accessories pages.
3. Use the search and sort controls to narrow down the catalog.
4. Open a product to view its full details, choose a color or capacity, and add it to the cart or favorites.
5. Manage quantities and remove items from the Cart page at any time.

## Technologies Used

- **React** — component-based UI library
- **TypeScript** — static typing across components, hooks, and API models
- **React Router** — client-side routing between Home, category, product details, cart, and favorites pages
- **SCSS** — modular, component-scoped styling
- **Context API** — global state management for the cart and favorites
- **REST API** — fetching product lists and product details
- **Git & GitHub** — version control and repository hosting
- **GitHub Pages** — live demo deployment

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
