# 🔗 URL Shortener - Spring Boot

A production-ready URL Shortener built from scratch using Java and Spring Boot. This project covers the complete backend flow — from API design to database interactions.

## 🚀 Features

- Shorten long URLs into compact, shareable links
- Instant redirection from short URL to original URL
- Collision-free unique short code generation
- RESTful APIs with proper HTTP status codes
- Persistent storage using MySQL database
- Input validation and error handling

## 🛠️ Tech Stack

- **Java 21** — Core programming language
- **Spring Boot 4.0.1** — Backend framework
- **Spring MVC** — REST API handling
- **Hibernate / JPA** — ORM for database interaction
- **Thymeleaf** — Frontend templating engine
- **MySQL** — Relational database
- **Maven** — Build tool

## 🌐 Live Demo

> Currently running on localhost:8081
> Live deployment link will be added after Railway deployment

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/shorten` | Generate a short URL |
| GET | `/{shortCode}` | Redirect to original URL |
| GET | `/api/all` | Get all shortened URLs |
| DELETE | `/api/{shortCode}` | Delete a short URL |

## 💡 How It Works

1. User sends a long URL via POST request
2. System generates a unique 6-character short code
3. Mapping is saved in MySQL database
4. When short URL is accessed, system redirects to original URL

## ⚙️ How to Run Locally

### Prerequisites

- Java 21+
- MySQL installed and running
- Maven 3.9+

### Steps

1. Clone the repository
