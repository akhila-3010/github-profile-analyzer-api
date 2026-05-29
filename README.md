# GitHub Profile Analyzer API

## Objective

Build a backend service that analyzes a GitHub user profile using the GitHub public API and stores useful insights in a MySQL database.

---

# Tech Stack

* Node.js
* Express.js
* MySQL
* GitHub REST API

---

# Features

## Required Features

* Fetch public GitHub profile data using username
* Store profile analysis in MySQL database
* API to fetch all analyzed profiles
* API to fetch a single analyzed profile

## Additional Features

* Most used programming language detection
* Most starred repository analysis
* Followers & following insights
* Account age calculation
* Error handling & validation
* Environment variable configuration
* RESTful API architecture
* Modular folder structure

---

# Project Structure

```bash
github-profile-analyzer-api/
│
├── config/
├── controllers/
├── routes/
├── services/
├── models/
├── middleware/
├── database/
├── utils/
│
├── .env
├── app.js
├── package.json
├── README.md
└── github_profiles.sql
```

---

# API Endpoints

## Analyze GitHub Profile

```http
POST /api/profile/:username
```

Fetches GitHub profile data from GitHub API and stores analysis in MySQL.

---

## Get All Profiles

```http
GET /api/profiles
```

Returns all analyzed GitHub profiles stored in database.

---

## Get Single Profile

```http
GET /api/profile/:username
```

Returns analysis data for a specific GitHub user.

---

# Database Schema

Stored fields include:

* Username
* Name
* Bio
* Followers Count
* Following Count
* Public Repository Count
* Most Used Language
* Most Starred Repository
* GitHub Profile URL
* Account Creation Date

---

# Installation

## Clone Repository

```bash
git clone https://github.com/akhila-3010/github-profile-analyzer-api.git
cd github-profile-analyzer-api
```

---

## Install Dependencies

```bash
npm install
```

---

## Setup Environment Variables

Create `.env` file:

```env
PORT=5000

MYSQL_HOST=localhost
MYSQL_USER=root
MYSQL_PASSWORD=yourpassword
MYSQL_DATABASE=github_analyzer

GITHUB_TOKEN=your_github_token
```

---

## Run Project

```bash
npm start
```

For development:

```bash
npm run dev
```

---

# Deployment

Backend deployed using Render.

Example:

```bash
https://github-profile-analyzer-api.onrender.com
```

---

# Future Improvements

* Swagger API Documentation
* Redis Caching
* Docker Support
* Profile Comparison Feature
* Analytics Dashboard

---

# Author

Akhila Chinta
