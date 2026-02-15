Login Page – Node.js + PostgreSQL

A basic authentication system built using Node.js, Express, EJS, and PostgreSQL.
This project supports user registration, login, password hashing with bcrypt, and session handling using Passport.

Features

User Registration

User Login

Password Encryption (bcrypt)

PostgreSQL Database

Express Sessions

Passport Authentication

EJS Templates

Technologies Used

Node.js

Express

PostgreSQL

EJS

Passport.js

bcrypt

dotenv

Installation
1. Clone Repository
git clone <your-github-repo-url>
cd Login_Page

2. Install Dependencies
npm install

3. Create .env File

Create a .env file in root folder:

DB_USER=princess
DB_PASSWORD=1234
DB_HOST=localhost
DB_PORT=5432
DB_NAME=login
SESSION_SECRET=secret

4. Create Database Table

Run this in PostgreSQL:

CREATE TABLE users(
  id SERIAL PRIMARY KEY,
  name VARCHAR(200),
  email VARCHAR(200) UNIQUE,
  password TEXT
);

5. Run Project
npm run dev


Server runs on:

http://localhost:3000

Learning Purpose

Created to understand backend authentication, Express routing, PostgreSQL integration, and password security.
