# 🛒 E-Commerce Order Management API

A scalable backend system for managing users, products, and orders in an e-commerce environment.  
Built with Golang and designed following Clean Architecture principles.

## 🚀 Tech Stack
- Golang (Gin Framework)
- PostgreSQL
- Docker & Docker Compose
- JWT Authentication

## 🧱 Architecture
Clean Architecture:
Handler → Service → Repository

## ✨ Features
- User authentication using JWT
- Role-based access control (Admin / User)
- Product management (CRUD)
- Order creation with transaction handling
- Automatic stock deduction
- Order history retrieval
- Middleware logging & request validation

## 🗄 Database
- PostgreSQL
- Indexing on frequently queried fields (user_id, product_id, created_at)

## 🐳 Deployment
- Dockerized application
- Multi-container setup (API + Database)

## 📌 Status
This project is under active development.

## 📎 Author
Tran Quoc Ky – Backend Golang Developer
## ▶️ Run Application

### Run locally
```bash
go run ./cmd/server
Run with Docker
docker build -t ecommerce-api .
docker run -p 8080:8080 ecommerce-api
Health Check
GET http://localhost:8080/health
