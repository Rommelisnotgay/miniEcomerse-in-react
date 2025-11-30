# Shop E-Commerce Application

A modern, fully-functional e-commerce platform built with React and Redux. This project demonstrates advanced frontend development practices with state management, routing, and responsive design.

**Author:** Rommel  
**Project Type:** Full-Stack Ready E-Commerce Application

---

## 📋 Project Overview

This is a comprehensive e-commerce shopping platform that showcases best practices in React development, state management, and modern web technologies. The application includes product browsing, shopping cart functionality with persistent storage, and a clean, responsive user interface.

---

## 🚀 Technologies & Stack

### Frontend Framework

- **React 19.2.0** - Latest React version with modern hooks and features
  - Component-based architecture
  - React Hooks (useState, useEffect)
  - Functional components with composition pattern

### State Management

- **Redux Toolkit 2.11.0** - Modern Redux with simplified API
  - Redux Slices for reducer logic
  - Immer middleware for immutable state updates
  - Integrated thunk middleware for async operations
- **react-redux 8.x** - Official React bindings for Redux
  - useSelector hook for accessing store state
  - useDispatch hook for dispatching actions

### Routing

- **React Router 7.9.6** - Modern client-side routing
  - BrowserRouter for SPA navigation
  - Link components for seamless page transitions
  - Dynamic route handling

### Styling & UI

- **Tailwind CSS 4.1.17** - Utility-first CSS framework
  - Responsive design utilities
  - Custom component styling
  - Mobile-first approach
- **@tailwindcss/vite 4.1.17** - Vite integration for optimized Tailwind CSS

### Build Tool

- **Vite 7.2.4** - Next-generation build tool
  - Lightning-fast HMR (Hot Module Replacement)
  - Optimized production builds
  - ES module support

### Development Tools

- **ESLint 9.39.1** - Code quality and consistency
  - React-specific linting rules
  - React Hooks exhaustive-deps warnings
  - Best practices enforcement

---

## 🎯 Key Features Implemented

### 1. **State Management with Redux Toolkit**

- Centralized cart state management
- Redux Slices for organized reducer logic
- Local storage persistence for cart data
- Actions: `addToCart`, `changeQuantity`, `toggleStatusTab`

### 2. **Component Architecture**

- **Header Component** - Navigation and cart badge
  - Real-time quantity calculation
  - Dynamic badge updates using useEffect
  - Cart toggle functionality
- **ProductCart Component** - Individual product display
  - Add to cart functionality
  - Product information display
  - Responsive grid layout
- **CartTab Component** - Shopping cart display
  - Cart items management
  - Quantity adjustment
  - Item removal functionality
- **Layout Component** - Page wrapper and structure

### 3. **Responsive Design**

- Mobile-first approach with Tailwind CSS
- Responsive grid layouts (lg, md, sm breakpoints)
- Flexible component sizing
- Touch-friendly interface elements

### 4. **Data Persistence**

- localStorage integration in Redux store
- Cart data survives page refreshes
- Automatic serialization/deserialization

### 5. **Modern Routing**

- Client-side routing with React Router
- Product detail pages
- Home page navigation
- Clean URL structure

---

## 📁 Project Structure

```
shope/
├── src/
│   ├── components/
│   │   ├── Header.jsx          # Navigation & cart badge
│   │   ├── ProductCart.jsx     # Product card component
│   │   ├── CartTab.jsx         # Shopping cart display
│   │   ├── Layout.jsx          # Page wrapper
│   ├── pages/
│   │   ├── Home.jsx            # Products listing
│   │   ├── Details.jsx         # Product details
│   ├── store/
│   │   ├── index.js            # Redux store configuration
│   │   ├── Cart.js             # Cart slice with reducers
│   ├── Products.js             # Product database
│   ├── App.jsx                 # Main app component
│   ├── main.jsx                # React entry point
│   ├── index.css               # Global styles
│   ├── App.css                 # App styles
│   └── assets/
│       └── images/             # Static assets
├── public/                      # Static files
├── package.json                # Dependencies
├── vite.config.js              # Vite configuration
├── eslint.config.js            # ESLint rules
└── README.md                   # This file
```

---

## 🛠️ Installation & Setup

### Prerequisites

- Node.js 16+
- npm or yarn

### Installation Steps

```bash
# Clone the repository
git clone <repository-url>

# Navigate to project directory
cd shope

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linting
npm lint
```

---

## 💡 Learning Outcomes & Skills Demonstrated

### React Concepts

- ✅ Functional components and hooks
- ✅ useState for local component state
- ✅ useEffect for side effects and lifecycle management
- ✅ useSelector and useDispatch from React-Redux
- ✅ Component composition and reusability
- ✅ Props drilling and prop management
- ✅ Event handling and user interactions

### State Management

- ✅ Redux store architecture
- ✅ Redux Toolkit slices and configureStore
- ✅ Action creators and reducers
- ✅ Middleware integration
- ✅ State selectors with useSelector
- ✅ localStorage synchronization with Redux

### Routing

- ✅ Client-side routing with React Router
- ✅ Navigation between pages
- ✅ Dynamic route parameters
- ✅ Link components for SPA navigation

### CSS & Styling

- ✅ Utility-first CSS with Tailwind
- ✅ Responsive design patterns
- ✅ Mobile-first development
- ✅ Flexbox layouts
- ✅ Grid systems
- ✅ Tailwind component composition

### Development Tools

- ✅ Vite build tool and configuration
- ✅ HMR (Hot Module Replacement)
- ✅ ESLint code quality rules
- ✅ Modern JavaScript (ES6+)
- ✅ Module imports/exports

### E-Commerce Functionality

- ✅ Product listing and filtering
- ✅ Shopping cart management
- ✅ Quantity adjustment
- ✅ Item removal
- ✅ Cart persistence
- ✅ Real-time quantity calculations

---

## 🔄 Redux Store Structure

```javascript
// Initial State
{
  cart: {
    items: [
      { productId: 1, quantity: 2 },
      { productId: 3, quantity: 1 }
    ],
    statusTab: false
  }
}

// Actions
addToCart({ productId, quantity })
changeQuantity({ productId, quantity })
toggleStatusTab()
```

---

## 🎨 Key Components

### Header Component

Displays navigation and real-time cart quantity badge using Redux state selectors and useEffect hooks.

### ProductCart Component

Shows product information and handles adding items to cart through Redux dispatch.

### CartTab Component

Displays cart items with quantity controls and removal functionality.

---

## 📱 Responsive Breakpoints

- **Mobile:** < 640px
- **Tablet:** 640px - 1024px (sm, md)
- **Desktop:** > 1024px (lg)

---

## 🚀 Performance Optimizations

- Vite for fast development and optimized builds
- Tree-shaking of unused code
- Code splitting for better load times
- Tailwind CSS purging of unused styles
- Redux selectors for memoized state access

---

## 🔐 Best Practices Implemented

- ✅ Immutable state updates (Redux Toolkit with Immer)
- ✅ Proper dependency arrays in useEffect
- ✅ Component-level state management
- ✅ Separation of concerns (containers vs presentational components)
- ✅ localStorage API for data persistence
- ✅ Clean code with meaningful variable names
- ✅ Responsive design patterns
- ✅ ESLint configuration for code quality

---

## 🚧 Future Enhancements

- User authentication and authorization
- Payment gateway integration
- Product search and filtering
- Order management system
- Admin dashboard
- Unit and integration tests
- TypeScript migration
- API integration

---

## 📝 License

This project is open source and available for educational purposes.

---

**Created with ❤️ by Rommel**  
_Building modern web applications with React and best practices_
