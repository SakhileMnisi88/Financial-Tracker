# Finance Tracker - Beginner's Guide

A web application for tracking your money - income, expenses, and savings.

## What Is This Project?

Think of this like a digital checkbook or budget app. You can:
- Log in securely
- Add your income and expenses
- See where your money is going
- View charts and summaries of your finances

## Languages Used

This project uses **3 main programming languages**:

1. **JavaScript** - Makes the website interactive (the frontend/what you see)
2. **Python** - Handles the business logic and data (the backend/behind the scenes)
3. **SQL** - Stores and organizes your financial data (the database)

Plus **HTML** and **CSS** for structuring and styling the web pages.

## Breaking Down The Tech Stack (ELI5)

### 🎨 Frontend (What You See)
The part of the app you interact with in your web browser.

- **React** - A JavaScript library that makes building interactive websites easier. Think of it like LEGO blocks for websites - you build the site by combining reusable pieces.
- **TailwindCSS** - A tool that helps make the website look pretty without writing tons of custom styling code. It's like having pre-made design templates.
- **Language Used:** JavaScript (plus HTML and CSS)

### 🧠 Backend (The Brain)
The "server" - the part that runs on a computer somewhere and handles all the logic.

- **FastAPI** - A Python framework that makes it easy to create an API. An **API** is like a waiter at a restaurant - it takes your order (request), goes to the kitchen (database), and brings back your food (data).
- **PyJWT** - Handles secure logins. When you log in, you get a special "token" (like a temporary ID card) that proves who you are.
- **Language Used:** Python

### 🗄️ Database (The Filing Cabinet)
Where all your financial data is stored permanently.

- **PostgreSQL** - A type of database (think of it as a super-organized Excel spreadsheet on steroids). It stores all your transactions, accounts, etc.
- **SQLAlchemy** - A Python tool that lets your backend code "talk" to the database without writing complex SQL commands.
- **Alembic** - Helps manage changes to your database structure over time (like if you want to add a new column).
- **Language Used:** SQL (Structured Query Language)

### 📚 Other Tools

- **Swagger** - Auto-creates documentation for your API, so developers can see what data they can request and how.
- **ORM** - "Object-Relational Mapping" - a translator between Python code and database SQL code.
- **Auth** - Short for "authentication" - the login/security system.

## How It All Works Together

Here's what happens when you use the app:

1. **You open the website** → Your browser loads the **React frontend** (JavaScript)
2. **You log in** → The frontend sends your username/password to the **FastAPI backend** (Python)
3. **Backend checks your credentials** → It queries the **PostgreSQL database** (SQL) to verify your account
4. **You get a token** → The backend uses **JWT** to create a secure token and sends it back
5. **You add an expense** → Frontend sends the data to the backend API
6. **Data gets saved** → Backend stores it in the PostgreSQL database
7. **You view your finances** → Frontend requests data from the backend, which fetches it from the database and sends it back

```
┌─────────────┐         ┌─────────────┐         ┌─────────────┐
│   Frontend  │ ←────→  │   Backend   │ ←────→  │  Database   │
│             │         │             │         │             │
│ JavaScript  │         │   Python    │         │     SQL     │
│   (React)   │         │  (FastAPI)  │         │ (PostgreSQL)│
└─────────────┘         └─────────────┘         └─────────────┘
     ↑                                                   ↑
     │                                                   │
  Your Browser                               Stores Your Data
```

## Summary of Technologies

| Technology | Type | Purpose | Language |
|------------|------|---------|----------|
| React | Library | Build the user interface | JavaScript |
| TailwindCSS | Framework | Style the website | CSS |
| FastAPI | Framework | Create the API/server | Python |
| PostgreSQL | Database | Store financial data | SQL |
| SQLAlchemy | ORM | Connect Python to database | Python |
| Alembic | Tool | Manage database changes | Python |
| PyJWT | Library | Handle secure logins | Python |

## Getting Started

### What You Need Installed
- **Python** - The programming language for the backend
- **Node.js** - JavaScript runtime to run React
- **PostgreSQL** - The database software

### Quick Start Steps

1. Download the code
2. Install Python dependencies (backend)
3. Install JavaScript dependencies (frontend)
4. Set up the database
5. Run the backend server
6. Run the frontend server
7. Open your browser and start tracking finances!

## Key Concepts Explained

**API (Application Programming Interface)** - A messenger that lets the frontend and backend talk to each other. Like a waiter taking orders between you and the kitchen.

**Frontend vs Backend** - Frontend is what you see and click. Backend is the logic and data processing you don't see.

**Database** - Where data is permanently stored, like a filing cabinet.

**Authentication** - Proving who you are (logging in).

**JWT Token** - A secure "ticket" that proves you're logged in, so you don't have to enter your password every time.

**ORM** - Lets you work with database data as if it were regular Python objects instead of writing SQL queries.

## Questions?

If you're new to programming, here's the learning path:
1. Learn basic HTML, CSS, JavaScript
2. Learn React (JavaScript frontend)
3. Learn Python basics
4. Learn FastAPI (Python backend)
5. Learn SQL and databases

This project combines all these skills into one full-stack application!
