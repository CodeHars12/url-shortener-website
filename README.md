🌐 Live Demo: https://url-shortener-website-ztwx.onrender.com

⭐ GitHub Repository: https://github.com/CodeHars12/url-shortener-website

# 🔗 URL Shortener

A production-ready URL Shortener application built using Java, Spring Boot, MySQL, Thymeleaf, and Docker. This application allows users to convert long URLs into short, shareable links and redirect instantly to the original destination.

## 🚀 Live Demo

🌐 Application URL

https://url-shortener-website-ztwx.onrender.com

Try it now:

https://url-shortener-website-ztwx.onrender.com

---

## ✨ Features

- Convert long URLs into short URLs
- Instant redirection using generated short codes
- Unique short code generation
- Persistent storage with MySQL
- Clean and responsive UI using Thymeleaf
- RESTful backend architecture
- Input validation and error handling
- Dockerized deployment
- Hosted on Render Cloud Platform

---

## 🛠️ Tech Stack

### Backend
- Java 21
- Spring Boot 4.0.1
- Spring MVC
- Spring Data JPA (Hibernate)

### Frontend
- HTML5
- CSS3
- Thymeleaf

### Database
- MySQL

### Build & Deployment
- Maven
- Docker
- Render

---

## 📸 Application Workflow

1. User enters a long URL.
2. Application generates a unique short code.
3. URL mapping is stored in MySQL database.
4. A shortened URL is returned to the user.
5. When the short URL is accessed, the application redirects to the original URL.

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|----------|----------|----------|
| POST | `/shorten` | Generate a short URL |
| GET | `/{shortCode}` | Redirect to original URL |
| GET | `/api/all` | Get all shortened URLs |
| DELETE | `/api/{shortCode}` | Delete a shortened URL |

---

## 🏗️ Project Architecture

```
Client
   │
   ▼
Thymeleaf UI
   │
   ▼
Spring MVC Controllers
   │
   ▼
Service Layer
   │
   ▼
Spring Data JPA
   │
   ▼
MySQL Database
```

---

## ⚙️ Run Locally

### Prerequisites

- Java 21+
- Maven 3.9+
- MySQL Server

### Clone Repository

```bash
git clone https://github.com/CodeHars12/url-shortener-website.git
cd url-shortener-website
```

### Configure Database

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/urlshortener
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
```

### Build Project

```bash
mvn clean install
```

### Run Application

```bash
mvn spring-boot:run
```

### Open Browser

```text
http://localhost:8080
```

---

## 📂 Database

The application stores:

- ID
- Original URL
- Short Code

using MySQL and Hibernate ORM.

---

## 🐳 Docker Deployment

Build Docker Image

```bash
docker build -t url-shortener .
```

Run Container

```bash
docker run -p 8080:8080 url-shortener
```

---

## 📁 Repository

GitHub Repository:

https://github.com/CodeHars12/url-shortener-website

---

## 👨‍💻 Author

**Harsh Bardhan Kumar**

GitHub:
https://github.com/CodeHars12

LinkedIn:
https://www.linkedin.com/in/harsh-bardhan-kumar/

Email:
harshbardhankumar10@gmail.com

---

## ⭐ Show Your Support

If you like this project, please consider giving it a ⭐ on GitHub.

Happy Coding! 🚀
