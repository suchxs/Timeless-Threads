<img src="./client/public/images/Timeless-Inverted.png" alt="logo" width="120"> <br>
# Timeless Threads
*A Dedicated web-based e-commerce platform for Timeless Threads to replace its reliance on Instagram for sales* <br>
The system will streamline product browsing, secure checkout, payment processing (via QR or Gcash), and automate inventory and Order management, Replacing Error-prone manual spreadsheets.

## 🛠 Tech Stack
![Tech Stack](https://skills-icons.vercel.app/api/icons?i=react,tailwind,mysql,node,vite,axios,express)

[Access the Website Here](https://timelessthreads.xyz/)  (To be Reinstated)
---

## 📁 Project Structure
```
Timeless-Threads/
├── server/                       # Backend (Node.js + Express + MySQL)
│   ├── app.js                    # Express server entry point
│   ├── app.prod.js               # Production server entry (used for PM2)
│   ├── config/                   # Database configuration
│   │   └── db.config.js
│   ├── controllers/              # Express route handler logic
│   │   ├── authController.js
│   │   ├── orderController.js
│   │   └── supplierOrderController.js
│   ├── database/                 # SQL schema and seed files
│   │   ├── schema.sql
│   │   ├── seed.sql
│   │   └── populate-products.sql
│   ├── models/                   # Data access models (raw SQL)
│   │   ├── user.js
│   │   ├── order.js
│   │   ├── productVariant.js
│   │   ├── supplier.js
│   │   ├── supplierOrder.js
│   │   └── supplierOrderItem.js
│   ├── routes/                   # Express route definitions (API endpoints)
│   │   ├── auth.js
│   │   ├── orders.js
│   │   ├── payments.js
│   │   ├── products.js
│   │   ├── suppliers.js
│   │   └── supplierOrders.js
│   ├── uploads/                  # Uploaded files (e.g., user profile pictures)
│   └── utils/                    # Utility functions
│       └── email.js              # Email service functions
│
├── client/                       # Frontend (React + Vite + Tailwind CSS)
│   ├── index.html                # Main HTML entry point
│   ├── public/                   # Public static files
│   │   ├── images/               # Product, logo, and payment images
│   │   │   ├── products/         # Product images (Mens, Womens, Accessories, Footwear, etc.)
│   │   │   ├── payment/          # Payment-related images
│   │   │   └── landing-page/     # Landing page images
│   │   ├── videos/               # Tutorial or promo videos
│   │   └── documents/            # Document files
│   └── src/
│       ├── components/           # Reusable React UI components
│       │   ├── AboutStrip.jsx
│       │   ├── CartModal.jsx
│       │   ├── FAQBubble.jsx
│       │   ├── Modal.jsx
│       │   ├── ProfilePicUploader.jsx
│       │   └── VariantSelector.jsx
│       ├── api/                  # API service layer
│       │   └── apiService.js     # Axios API service functions
│       ├── css/                  # Custom CSS
│       │   └── main.css
│       ├── App.jsx               # Main React app component
│       ├── main.jsx              # React app entry point
│       └── Pages/Components:     # Page and feature components
│           ├── About.jsx
│           ├── Account.jsx
│           ├── Cart.jsx
│           ├── Checkout.jsx
│           ├── Dashboard.jsx
│           ├── DashboardHome.jsx
│           ├── FAQs.jsx
│           ├── Footer.jsx
│           ├── ForgotPassword.jsx
│           ├── Login.jsx
│           ├── Mens.jsx
│           ├── Navbar.jsx
│           ├── OrderApproval.jsx
│           ├── OrderConfirmation.jsx
│           ├── OrderHistory.jsx
│           ├── OrderManagement.jsx
│           ├── ProductCarousel.jsx
│           ├── ProductData.jsx
│           ├── ProductDetails.jsx
│           ├── ProductManagement.jsx
│           ├── ProductReview.jsx
│           ├── Products.jsx
│           ├── ResetPassword.jsx
│           ├── Reviews.jsx
│           ├── Settings.jsx
│           ├── Sidebar.jsx
│           ├── SupplierPortal.jsx
│           ├── UserManagement.jsx
│           ├── VerifyEmail.jsx
│           └── Womens.jsx
│
├── config/                       # Frontend build and styling config
│   ├── postcss.config.js         # PostCSS configuration
│   ├── tailwind.config.js        # Tailwind CSS configuration
│   └── vite.config.js            # Vite build configuration
│
├── .env                          # Backend environment variables
├── .gitignore
├── package.json                  # Project dependencies and scripts
├── package-lock.json
├── README.md
└── LICENSE
```

---

## 📌 Notes
- Backend follows the MVC (Model-View-Controller) Architectural Pattern
- Frontend follows the Component-Based-Architecture Pattern
- Frontend makes API calls (via Axios) to the backend
---

## Prerequisites
- Node.js v18+
- MySQL 8.0+
---
## Setup  
Quick Setup Guide for the Application

1. Create a database named `timeless_db` in MySQL:

    ```bash
    CREATE SCHEMA `timeless_db` ;
    ```
    **OR**
    ```bash
    CREATE DATABASE timeless_db;
    ```

2. Clone the repository:

    ```bash
    git clone https://github.com/suchxs/Timeless-Threads
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Build the project:

    ```bash
    npm run dev
    ```
    **OR**
    ```bash
    npm run dev:server
    npm run dev:client
    ```
    **OR**
    *For Production:*
    ```
    npm run build
    pm2 start server/app.prod.js --name "Timeless"
    ```
---
## Group Members:

[![Joseph Corsega](https://github.com/suchxs.png?size=60 "Joseph Corsega")](https://github.com/suchxs) [![Paul Divinagracia](https://github.com/PaoloBen.png?size=60 "Paul Divinagracia")](https://github.com/PaoloBen) 
<a href="https://github.com/sojaARY">
    <img src="https://github.com/sojaARY.png" width="60" height="60" alt="Alex Yap" />
</a>
