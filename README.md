# Paradise Nursery Shopping Application

A responsive e-commerce web application for browsing and purchasing houseplants, developed as the final capstone project for the Coursera / IBM course **Developing Front-End Apps with React**.

---

## Project Overview

**Paradise Nursery** is an intuitive, user-friendly shopping application where plant enthusiasts can explore an extensive collection of indoor plants, learn about their unique benefits, and manage items in a dynamic shopping cart.

---

## Key Features

### 1. Landing Page
- **Company Branding:** Displays the company name "Paradise Nursery" with the motto *"Where Green Meets Serenity"*.
- **Background Imagery:** Features an ambient greenhouse background image.
- **About Us Section:** Explains the mission, expert plant care standards, and commitment to creating greener spaces.
- **Call-to-Action:** A prominent **"Get Started"** button transitioning smoothly to the product catalog.

### 2. Product Listing Page
- **Category Grouping:** Plants are organized into 5 distinct categories:
  - Air Purifying Plants
  - Aromatic Fragrant Plants
  - Insect Repellent Plants
  - Medicinal Plants
  - Low Maintenance Plants
- **Plant Details:** Each product card includes:
  - High-quality thumbnail image
  - Plant name
  - Brief description of botanical benefits
  - Unit price
  - Interactive **"Add to Cart"** button
- **Interactive State:** When clicked, the plant is added to the cart, the button is disabled, and its text changes to "Added to Cart".
- **Dynamic Header / Navbar:** 
  - Visible across both the Product Listing and Shopping Cart pages.
  - Includes navigation links to **Home**, **Plants**, and **Cart**.
  - Displays a shopping cart icon with a real-time badge counting total items in the cart.

### 3. Shopping Cart Page
- **Summary Metrics:** Prominently displays:
  - Total number of plants in the cart
  - Total cart amount (calculated dynamically)
- **Item Details:** Each added plant displays its thumbnail, name, unit price, quantity, and line-item total cost.
- **Cart Management Controls:**
  - **Increase (`+`) Button:** Increments quantity by 1, automatically updating item total and grand total.
  - **Decrease (`-`) Button:** Decrements quantity by 1 (removes the item if quantity drops to 0).
  - **Delete Button:** Instantly removes the item from the cart and re-enables the product button on the listing page.
- **Navigation & Checkout:**
  - **Continue Shopping Button:** Returns to the product catalog.
  - **Checkout Button:** Prompts a friendly "Coming Soon" notification.

---

## Tech Stack

- **Frontend Library:** [React](https://react.dev/) (v18)
- **State Management:** [Redux Toolkit](https://redux-toolkit.js.org/) & [React-Redux](https://react-redux.js.org/)
- **Build Tool:** [Vite](https://vitejs.dev/)
- **Styling:** CSS3 (responsive grid and flexbox layout)
- **Deployment:** [GitHub Pages](https://pages.github.com/) via `gh-pages`

---

## Project Structure

```text
Paradise Nursery/
├── index.html
├── package.json
├── vite.config.js
├── README.md
├── public/
│   └── vite.svg
└── src/
    ├── App.css
    ├── App.jsx
    ├── AboutUs.css
    ├── AboutUs.jsx
    ├── CartItem.css
    ├── CartItem.jsx
    ├── CartSlice.jsx
    ├── ProductList.css
    ├── ProductList.jsx
    ├── index.css
    ├── main.jsx
    └── store.js
```

---

## Getting Started

### Prerequisites

- Node.js (version 18 or higher)
- npm (version 9 or higher)

### Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd "Paradise Nursery"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the local development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`.

---

## Production Build & Deployment

To create an optimized production build:
```bash
npm run build
```

To deploy the application to GitHub Pages:
```bash
npm run deploy
```

---

## Evaluation & Grading Deliverables

| Deliverable | Description |
|---|---|
| **README.md** | Complete project documentation and details |
| **AboutUs.jsx** | Details about the company and mission statement |
| **App.css** | Landing page background styling and animations |
| **App.jsx** | Landing page with company name, intro, and Get Started button |
| **CartSlice.jsx** | Redux Toolkit slice managing cart state (`addItem`, `removeItem`, `updateQuantity`) |
| **ProductList.jsx** | Catalog grouping plants into categories with dynamic cart badge |
| **CartItem.jsx** | Shopping cart view with total calculations, item adjustments, and navigation |
