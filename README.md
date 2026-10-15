# Paradise Nursery - Online Plant Shopping Application

Welcome to **Paradise Nursery**, where green meets serenity! This is a complete e-commerce web application designed for houseplant enthusiasts to browse, select, and purchase various types of plants. Developed using **React**, **Redux Toolkit**, and **Vite**, this application demonstrates modern front-end design, modular component architecture, and centralized state management.

---

## 🌿 Key Features

1. **Landing Page (`App.jsx` & `AboutUs.jsx`)**
   - High-resolution aesthetic background with ambient glassmorphism effects.
   - Company name ("Welcome to Paradise Nursery") and tagline ("Where Green Meets Serenity").
   - Detailed company background, values, and mission in the **About Us** section.
   - Interactive **Get Started** button transitioning smoothly into the plant shopping gallery.

2. **Categorized Product Listing (`ProductList.jsx`)**
   - 6 curated plant categories:
     - *Air Purifying Plants* (Snake Plant, Spider Plant, Peace Lily, Boston Fern, Rubber Plant, Aloe Vera)
     - *Aromatic Fragrant Plants* (Lavender, Jasmine, Rosemary, Mint, English Lavender, Honeysuckle)
     - *Insect Repellent Plants* (Marigold, Geraniums, Citronella, Chrysanthemum, Basil, Catnip)
     - *Medicinal Plants* (Aloe Vera, Echinacea, Peppermint, Lemon Balm, Chamomile, Calendula)
     - *Low Maintenance Plants* (ZZ Plant, Pothos, Snake Plant, Cast Iron Plant, Succulents, Aglaonema)
   - Visual plant cards with thumbnail photos, names, descriptive details, and unit prices.
   - Dynamic **Add to Cart** action buttons that disable and switch state to **Added to Cart** once selected.

3. **Centralized Cart State Management (`CartSlice.jsx`)**
   - Built with Redux Toolkit (`createSlice`).
   - Implements three core reducers:
     - `addItem`: Adds an item to the shopping cart, initializing quantity to 1 or incrementing if already present.
     - `removeItem`: Removes an item completely from the cart by identifier/name.
     - `updateQuantity`: Adjusts item quantity based on user action (+ / -).

4. **Interactive Shopping Cart (`CartItem.jsx`)**
   - Dynamic total items count badge positioned on the shopping cart icon in the navigation bar.
   - Full cart management with real-time total order amount computation.
   - Item quantity controls: increase (`+`) and decrease (`-`) buttons (auto-removes item when quantity reaches zero).
   - Instant calculation of subtotal costs per item and overall cart total.
   - Direct item removal via the "Delete" button.
   - Navigation buttons to **Continue Shopping** and **Checkout**.

---

## 📂 Project Architecture

```
e-plantShopping/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── AboutUs.css
│   ├── AboutUs.jsx          # Company background and mission statement
│   ├── App.css              # Global styling, layout, and landing page styling
│   ├── App.jsx              # Landing page component with "Get Started" trigger
│   ├── CartItem.css         # Styling for shopping cart item cards and controls
│   ├── CartItem.jsx         # Cart display, item increments/decrements, totals
│   ├── CartSlice.jsx        # Redux slice with addItem, removeItem, updateQuantity
│   ├── ProductList.css      # Styling for categorized grid and plant cards
│   ├── ProductList.jsx      # Plant shop page with category grouping & cart badge
│   ├── index.css
│   ├── main.jsx             # React DOM root entry point with Redux Provider
│   └── store.js             # Redux store configuration
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16.0.0 or higher recommended)
- npm or yarn

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/hmumar-cse/e-plantShopping.git
   cd e-plantShopping
   ```

2. **Install project dependencies:**
   ```bash
   npm install
   ```

3. **Launch the development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## 🛠️ Technology Stack

- **Framework:** React 18
- **State Management:** Redux Toolkit & React-Redux
- **Build Tool / Bundler:** Vite
- **Styling:** Modular CSS3 with Flexbox, CSS Grid, and responsive media queries
- **Icons:** SVG vector graphics

---

## 📜 License

This project is licensed under the MIT License.