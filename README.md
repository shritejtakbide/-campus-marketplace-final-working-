# Campus Marketplace 🎓

A full-stack web application designed for college students to buy and sell products within their campus community.

Campus Marketplace provides a centralized platform where students can explore product listings, publish items for sale, communicate with sellers, and submit student verification requests.

## ✨ Features

- **User Authentication:** Student registration and login.
- **Product Marketplace:** Browse products listed by students.
- **Search and Filtering:** Find products by name and category.
- **Sell Products:** Add new products with a name, category, price, and description.
- **Product Details:** View information about individual listings and their sellers.
- **Student Verification:** Submit student information and a verification document.
- **Messaging:** Communicate through product-specific chats.
- **MySQL Database:** Store users, products, verification requests, sessions, and chat messages.
- **Responsive Interface:** A modern glass-style interface designed for a smooth user experience.

## 🛠️ Technology Stack

**Frontend**
- HTML5
- CSS3
- JavaScript

**Backend**
- Node.js
- Native HTTP server
- REST API

**Database**
- MySQL
- `mysql2` Node.js package

**Configuration**
- Environment variables using `dotenv`

## 📁 Project Structure

```text
Campus_Marketplace/
├── public/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── uploads/
├── server.js
├── database.sql
├── package.json
├── package-lock.json
├── .env.example
├── .gitignore
└── README.md
```

The exact files may vary depending on the version uploaded to the repository.

## ⚙️ Prerequisites

Install the following before running the application:

- Node.js
- npm
- MySQL Server

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/shritejtakbide/campus-marketplace1.git
cd campus-marketplace1
```

### 2. Install dependencies

```bash
npm install
```

### 3. Create the MySQL database

Open MySQL and run:

```sql
CREATE DATABASE campus_marketplace;
```

If the repository contains a `database.sql` file with the required table definitions, import that file into MySQL as well.

### 4. Configure environment variables

Create a `.env` file in the project root:

```env
DB_HOST=localhost
DB_PORT=3306
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=campus_marketplace
PORT=3000
```

Replace `your_mysql_password` with your local MySQL password.

**Security:** Never commit your actual `.env` file or database credentials to GitHub.

### 5. Start the application

```bash
node server.js
```

If the server starts successfully, open:

http://localhost:3000

## 🔐 Demo Account

If the database initialization creates the demo account, you can use:

- **Email:** `student@campus.local`
- **Password:** `student123`

For development and demonstration purposes only. Change or remove demo credentials before production use.

## 🗄️ Database

The application uses MySQL to persist application data, including:

- User accounts
- Product listings
- Student verification requests
- Login sessions
- Product-specific chat messages

The database must be configured and accessible for the backend to operate.

## 🌐 Deployment

The frontend and Node.js backend can be deployed to a compatible hosting platform. A hosted deployment requires a reachable cloud MySQL database and correctly configured environment variables.

Do not use `localhost` as the database host in a hosted deployment unless the database is running in the same environment.

Uploaded verification documents should use secure, persistent storage suitable for production.

## 🔒 Security Notes

- Keep database credentials in environment variables.
- Do not commit `.env`, private student documents, or `node_modules`.
- Use HTTPS and secure authentication practices for production.
- Restrict access to sensitive student verification information.

## 🎯 Project Objective

The objective of Campus Marketplace is to make it easier for students to exchange useful products within their college community while providing a centralized marketplace and communication platform.

## 👨‍💻 Author

**Shritej Takbide**

GitHub: https://github.com/shritejtakbide

---

*Developed as a full-stack campus marketplace project.*
