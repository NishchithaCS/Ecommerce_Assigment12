This is a simple e-commerce backend application built with *Node.js, **Express, and **MongoDB*. 
It provides APIs for user authentication, product management, cart handling, and order processing.

## Features

- User registration and login with JWT authentication
- Role-based access control (Admin and Customer)
- Product CRUD operations (Admin only)
- Shopping cart management
- Order creation from cart
- Basic search and pagination support for products

# 🛒 E-Commerce Backend API

This is a RESTful E-Commerce backend built with *Node.js, **Express, **MongoDB, and **JWT* for authentication and role-based access control.

## 📁 Features

- ✅ *User Authentication* (Register/Login)
- 🛡 *JWT-based Auth* & Role Middleware (Customer/Admin)
- 📦 *Product Management*
- 🛍 *Cart Management*
- 📑 *Order Placement & Tracking*
- 🔐 Role-based Admin Access (for Product Create/Update/Delete)

---

## ⚙ Tech Stack

- *Backend*: Node.js, Express.js
- *Database*: MongoDB (Mongoose ODM)
- *Authentication*: JSON Web Token (JWT)
- *Security*: Role-based middleware
- *Other*: dotenv, bcryptjs, cors

---

## 🧾 API Endpoints

### 🔐 Auth
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Register a new user |
| POST | /api/auth/login | Login and get JWT token |

---

### 📦 Products
| Method | Endpoint | Description | Role |
|--------|----------|-------------|------|
| GET | /api/products | Get all products (with search + pagination) | Public |
| POST | /api/products | Create product | Admin |
| PUT | /api/products/:id | Update product | Admin



├── app.js
├── server.js
├── .env
├── models/
│ ├── User.js
│ ├── Product.js
│ └── Order.js
├── routes/
│ ├── authRoutes.js
│ ├── productRoutes.js
│ ├── cartRoutes.js
│ └── orderRoutes.js
├── controllers/
│ ├── authController.js
│ ├── productController.js
│ ├── cartController.js
│ └── orderController.js
├── middleware/
│ ├── authMiddleware.js
│ └── roleMiddleware.js

markdown
Copy
Edit
