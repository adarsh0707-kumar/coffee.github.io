# ☕ Coffee Shop Web Application (`coffee.github.io`)

A sleek, responsive, modern digital storefront and interactive landing page built for specialty coffee shops and roasteries. Built with semantic HTML5, custom CSS3, and modern vanilla JavaScript, this project features zero external dependencies, fast loading speeds, and seamless deployment on **GitHub Pages**.

---

## 📸 Preview & Highlights

- **Dark & Warm Aesthetic**: Premium dark UI paired with warm golden accents (`#d3ad7f`) tailored for coffee lovers.
- **Fully Responsive**: Optimized for desktops, tablets, and mobile devices with fluid layout grids and touch-friendly controls.
- **Interactive UI Components**: Real-time sliding cart panel, live search overlay, dynamic navigation toggle, and smooth anchor scrolling.

---

## 📑 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)
- [Quick Start & Local Setup](#-quick-start--local-setup)
- [Deployment Guide](#-deployment-guide)
- [JavaScript Interactivity Breakdown](#-javascript-interactivity-breakdown)
- [Customization & Configuration](#-customization--configuration)
- [Roadmap & Future Enhancements](#-roadmap--future-enhancements)
- [License & Acknowledgments](#-license--acknowledgments)

---

## ✨ Features

### 🎨 Design & Layout
- **Hero Banner**: Eye-catching visual greeting with custom call-to-action (CTA) buttons encouraging immediate ordering.
- **About Us Section**: Split-grid layout showcasing brand story, bean origins, and roasting philosophy.
- **Menu & Products Grid**: Dynamic product cards highlighting featured espresso drinks, cold brews, and whole bean coffee bags with price tags and star ratings.
- **Customer Reviews**: Testimonial cards featuring customer quotes, user avatars, and star ratings.
- **Contact & Map Integration**: Embedded Google Maps iframe alongside an intuitive customer inquiry form.

### ⚡ Client-Side Interactivity
- 🛒 **Slide-Out Cart Drawer**: Dynamic sliding sidebar menu showing chosen items, quantities, subtotal calculations, and checkout buttons.
- 🔍 **Search Bar Overlay**: Sleek search modal overlay accessible directly from the header utility bar.
- 📱 **Responsive Mobile Menu**: Hamburger menu navigation with automated menu dismissal on viewport scroll.
- ⚓ **Smooth Scrolling**: Native CSS smooth navigation between page sections (`#home`, `#about`, `#menu`, `#products`, `#review`, `#contact`).

---

## 🛠️ Tech Stack

| Technology | Role / Usage |
| :--- | :--- |
| **HTML5** | Semantic structure (`<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`) |
| **CSS3** | Flexbox, CSS Grid, Custom CSS Variables, Keyframe Animations, `@media` queries |
| **JavaScript (ES6+)** | Lightweight DOM manipulation, event listeners, class toggling for sidebars |
| **Font Awesome / Lucide** | High-quality vector icon set for UI buttons, stars, and social media links |
| **GitHub Pages** | Free static website hosting directly from the repository |

---

## 📂 Repository Structure

```text
coffee.github.io/
│
├── index.html              # Core single-page HTML layout
├── css/
│   └── style.css           # Global styles, variables, grid layouts, and media queries
├── js/
│   └── script.js          # DOM manipulation logic (cart, search bar, navigation)
├── images/                 # Product photography, hero background, avatars, logo
│   ├── about-img.jpeg
│   ├── menu-1.png
│   ├── product-1.png
│   ├── pic-1.png
│   └── hero-bg.jpeg
├── README.md               # Project documentation
└── LICENSE                 # License file
```

---

## 🚀 Quick Start & Local Setup

### Prerequisites
To run this project locally, you only need a modern web browser (Google Chrome, Firefox, Safari, Edge).

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/adarsh0707-kumar/coffee.github.io.git
   ```

2. **Navigate into the project directory:**
   ```bash
   cd coffee.github.io
   ```

3. **Open the project in your browser:**
   - Double-click `index.html` to open it directly in your default browser.
   - Or use VS Code's **Live Server** extension:
     1. Open the project folder in VS Code.
     2. Right-click `index.html` and select **"Open with Live Server"**.

---

## 🌐 Deployment Guide (GitHub Pages)

Because this repository is structured as a static website, it can be published online for free using **GitHub Pages**:

1. Push your changes to the `main` or `master` branch on GitHub.
2. Navigate to your repository on GitHub: `https://github.com/<username>/coffee.github.io`.
3. Go to **Settings** > **Pages**.
4. Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder, then click **Save**.
6. Your live site will be accessible at:
   ```text
   https://<username>.github.io/coffee.github.io/
   ```

---

## ⚡ JavaScript Interactivity Breakdown

The dynamic drawer toggles and overlay behavior are powered by lightweight ES6 vanilla JavaScript:

```javascript
// Selecting DOM Elements
const navbar = document.querySelector('.navbar');
const cartItem = document.querySelector('.cart-items-container');
const searchForm = document.querySelector('.search-form');

// Toggle Mobile Menu
document.querySelector('#menu-btn').onclick = () => {
    navbar.classList.toggle('active');
    cartItem.classList.remove('active');
    searchForm.classList.remove('active');
};

// Toggle Shopping Cart Drawer
document.querySelector('#cart-btn').onclick = () => {
    cartItem.classList.toggle('active');
    navbar.classList.remove('active');
    searchForm.classList.remove('active');
};

// Toggle Search Bar Overlay
document.querySelector('#search-btn').onclick = () => {
    searchForm.classList.toggle('active');
    navbar.classList.remove('active');
    cartItem.classList.remove('active');
};

// Auto-close open drawers on page scroll
window.onscroll = () => {
    navbar.classList.remove('active');
    cartItem.classList.remove('active');
    searchForm.classList.remove('active');
};
```

---

## 🎨 Customization & Configuration

### Modifying Theme Colors
All primary colors and typography are centralized using CSS custom variables defined at the top of `css/style.css`:

```css
:root {
    --main-color: #d3ad7f;    /* Accent Gold / Warm Tan */
    --black: #13131a;         /* Main Dark Theme Background */
    --bg: #010103;            /* Dark Background Panels */
    --border: .1rem solid rgba(255, 255, 255, .3);
}
```

To change the primary accent color across the entire site, simply edit `--main-color`:
```css
:root {
    --main-color: #e67e22; /* Warm Orange Accent */
}
```

---

## 🛣️ Roadmap & Future Enhancements

- [ ] **Dynamic Cart Management**: Implement `localStorage` persistence so cart items remain saved upon page refresh.
- [ ] **Payment Integration**: Integrate Stripe JS or PayPal Sandbox checkout capabilities.
- [ ] **Filterable Menu**: Add categories (e.g., Hot Drinks, Cold Brews, Beans, Pastries) with live filter buttons.
- [ ] **Dark/Light Mode Toggle**: Add a user-selected theme switcher.

---

## 📜 License & Acknowledgments

- **License**: Distributed under the [MIT License](LICENSE).
- **Icons**: [Font Awesome](https://fontawesome.com/)
- **Fonts**: [Google Fonts (Roboto / Poppins)](https://fonts.google.com/)

---

<p align="center">
  Crafted with ☕ and passion for great coffee.
</p>