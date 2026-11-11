# Paradise Nursery Shopping Application

Welcome to the **Paradise Nursery Shopping Application**, a modern, responsive e-commerce web application built with **React** and **Redux Toolkit** for an online houseplant nursery.

---

## 🌿 Project Overview

**Paradise Nursery** is an intuitive online plant shopping application where "Green Meets Serenity". The application allows plant lovers and home decorators to browse a wide variety of houseplants categorized by their distinct characteristics, view plant details, manage their shopping cart, and calculate real-time totals.

---

## ✨ Features

- **Landing Page & Company Profile:**
  - Engaging hero section with background imagery and nursery branding.
  - Informative "About Us" section highlighting Paradise Nursery's passion, mission, and standards.
  - "Get Started" call-to-action button seamlessly transitioning users into the plant catalog.

- **Dynamic Product Catalog (`ProductList.jsx`):**
  - Multiple plant categories (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance).
  - At least 6 unique houseplants per category, complete with high-quality thumbnails, names, descriptions, and unit prices.
  - Interactive "Add to Cart" buttons that add items to the global cart state, disable immediately to prevent duplicate additions, and provide clear user feedback ("Added to Cart").
  - Responsive navigation bar with links to Home, Plants catalog, and the Shopping Cart, including a dynamic badge displaying total cart items.

- **Global State Management with Redux Toolkit (`CartSlice.jsx`):**
  - Centralized cart slice managing the items array.
  - `addItem`: Adds selected plants with initial quantity or increments if already present.
  - `removeItem`: Removes specific items from the shopping cart.
  - `updateQuantity`: Updates individual item quantities when incremented or decremented.

- **Interactive Shopping Cart (`CartItem.jsx`):**
  - Detailed cart breakdown displaying thumbnail, plant name, and unit price.
  - Individual item subtotal calculation (`cost × quantity`).
  - Overall total cart amount computed dynamically.
  - Quantity controls (`+` and `-` buttons) to increase or decrease quantities, automatically removing items when quantity reaches zero.
  - "Delete" button for direct removal of individual plants.
  - "Continue Shopping" button returning users directly to the plant catalog.
  - "Checkout" button providing a "Coming Soon" prompt.

---

## 🛠️ Technology Stack

- **Frontend Framework:** React 18
- **State Management:** Redux Toolkit & React-Redux
- **Build Tool:** Vite
- **Styling:** CSS3 (Flexbox, Grid, Responsive Media Queries)
- **Icons & Graphics:** SVG Icons and Pixabay/Unsplash CDN Imagery

---

## 🚀 Getting Started

### Prerequisites

- Node.js (version 16 or above recommended)
- npm or yarn

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/carwynetic/coursera4.git
   cd coursera4
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Build for production:
   ```bash
   npm run build
   ```

---

## 📁 Project Structure

```text
├── public/
├── src/
│   ├── assets/
│   ├── AboutUs.css
│   ├── AboutUs.jsx         # Company mission, details, and introduction
│   ├── App.css             # Styling for landing page and overall layout
│   ├── App.jsx             # Main App component with landing page & toggle logic
│   ├── CartItem.css        # Styling for cart items and totals
│   ├── CartItem.jsx        # Shopping cart view with item controls & totals
│   ├── CartSlice.jsx       # Redux slice with addItem, removeItem, updateQuantity
│   ├── index.css           # Global CSS styles
│   ├── main.jsx            # React root mount with Redux Provider
│   ├── ProductList.css     # Styling for product cards, grid, and navigation bar
│   ├── ProductList.jsx     # Plant catalog grouped by category with cart counter
│   └── store.js            # Redux store configuration
├── index.html
├── package.json
└── vite.config.js
```

---

## 👨‍💻 Author

- Developed for the IBM Full-Stack / Front-End Developer Course - Final Project: Paradise Nursery Shopping Application.
