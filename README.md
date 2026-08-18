<div align="center">

# 🛋️ Designer — Furniture E-Commerce Website

**A furniture & interior-design storefront with a companion admin dashboard — built with React** ⚛️

🎓 Final project for the **ITI (Information Technology Institute) Front-End Web Development Training**

🌐 **[Live Demo](https://final-iti-project-u8b3.vercel.app/)**

</div>

---

**Designer** is a two-app monorepo: a customer-facing **e-commerce storefront** where users browse a furniture catalog, manage a shopping cart, and walk through a validated checkout flow — plus a separate **admin dashboard** with analytics charts and user/product management tables.

---

## 🛠️ Tech Stack

### 🛒 E-Commerce Storefront (`E-Commerce/`)

| Category | Technology |
|---|---|
| ⚛️ Framework | [React 18](https://react.dev) (Create React App) |
| 🧭 Routing | [React Router v6](https://reactrouter.com) (`createBrowserRouter`) |
| 🛒 Cart State | [react-use-cart](https://www.npmjs.com/package/react-use-cart) (localStorage persistence) |
| 🎨 Styling | Bootstrap 5 ([TemplateMo 572 "Designer"](https://templatemo.com) template) + Reactstrap |
| 🎬 Animations | [AOS](https://michalsnik.github.io/aos/) scroll animations + Owl Carousel |
| 🔔 Feedback | [SweetAlert2](https://sweetalert2.github.io) + [Notyf](https://carlosroso.com/notyf/) toasts |
| 📧 Email | [EmailJS](https://www.emailjs.com) — order confirmation emails |
| 🖼️ Icons | Font Awesome, Bootstrap Icons, Boxicons |

### 📊 Admin Dashboard (`Dashboard/`)

| Category | Technology |
|---|---|
| ⚛️ Framework | [React 18](https://react.dev) (Create React App) |
| 🧩 UI | [Material-UI](https://mui.com) + styled-components |
| 📈 Charts | [Recharts](https://recharts.org) |
| 📋 Tables | [material-table](https://material-table.com) with in-memory CRUD |

---

## ✨ Key Features

### 🛒 Storefront

- 🏠 **Home page** — hero banner, search section, trending picks, contact map, and call-to-action
- 🛋️ **Shop** (`/Shop`) — catalog of 32 furniture products (chairs, tables, beds, sofas) with prices, ratings, and shuffle-style ALL / NEW / TRENDS / CUSTOM views
- 🖼️ **Gallery & Details** — 12-item interior-design gallery, each opening a dedicated detail page (`/Details/:id`)
- 🛒 **Shopping cart** — add to cart, quantity + / −, remove items, empty cart, live totals, and a navbar badge counter (persisted via localStorage)
- 🔐 **Login & Sign-Up** — client-side forms with regex validation and toast feedback; User/Admin roles (admin login redirects to the dashboard app)
- 💳 **Guarded checkout** — cart checkout requires login, then walks through a multi-section payment form (account info, date of birth, gender, credit-card/PayPal details with card-number, CVC & expiry validation, and terms acceptance)
- 📧 **Order confirmation email** — sent via EmailJS on successful checkout, with a SweetAlert2 success modal
- 📱 **Fully responsive** — Bootstrap 5 layout with AOS scroll animations throughout
- ℹ️ **About, Explore & Contact pages** — services, testimonials, and a Google Maps embed

### 📊 Admin Dashboard

- 📈 **Analytics home** — revenue / sales / costs cards and a monthly active-users line chart (Recharts)
- 👥 **User management** (`/users`) — material-table with add / edit / delete
- 🛋️ **Product management** (`/products`) — CRUD table for furniture products
- 🧭 **Topbar + sidebar** admin layout with widgets for new members and latest transactions

> ⚠️ **Note:** This is a front-end training project — authentication, payments, and dashboard data are simulated client-side (no backend server).

---

## ⚙️ Installation & Setup

### 📋 Prerequisites

- **Node.js 16+** and **npm**

### 🚀 Getting Started

**1. Clone the repository**

```bash
git clone https://github.com/omniyanasser/Final-ITI-Project.git
cd Final-ITI-Project
```

**2. Run the E-Commerce storefront** 🛒

```bash
cd E-Commerce
npm install
npm start          # → http://localhost:3000
```

**3. Run the Admin Dashboard** 📊 (in a separate terminal)

```bash
cd Dashboard
npm install
npm start          # → http://localhost:3000 (use another port if the storefront is running)
```

### 📜 Available Scripts (both apps)

| Command | Description |
|---|---|
| `npm start` | 🔧 Start the development server |
| `npm run build` | 📦 Create an optimized production build |
| `npm test` | 🧪 Run tests |

---

## 📁 Project Structure

```
Final-ITI-Project/
├── E-Commerce/               # 🛒 Storefront (CRA)
│   ├── public/               #    Bootstrap 5 template assets & vendor scripts
│   └── src/
│       ├── index.js          #    Router + AOS init
│       ├── App.js            #    Checkout / payment page
│       ├── Homepage/ About/ Explore/ Gallery/ Contact/
│       ├── Shop/             #    Product grid + catalog data (DataApi.js)
│       ├── Cart/             #    Shopping cart
│       ├── Details/          #    Product detail pages
│       └── Components/       #    Login, SignUp, Payment, validation
└── Dashboard/                # 📊 Admin app (CRA)
    └── src/
        ├── components/       #    Topbar, Sidebar, charts, widgets
        └── components/Pages/ #    Homepage, UserList, ProductList
```

---

## 👥 Contributors

An ITI team project built by:

- 👨‍💻 **Ahmed Abdel Fatah**
- 👩‍💻 **Engy Mohamed**
- 👩‍💻 **Norhan Elyan**
- 👩‍💻 **Omniya Nasser** — [GitHub](https://github.com/omniyanasser) · [LinkedIn](https://www.linkedin.com/in/omniya-nasser-060584248)

---

## 🙏 Credits

- 🎨 Storefront design based on the free [TemplateMo 572 "Designer"](https://templatemo.com/tm-572-designer) Bootstrap 5 template
- 📷 Stock photos from Pexels

---

<div align="center">

Made with ❤️ at **ITI — Information Technology Institute**

</div>
