# API Usage & Subscription Management Backend

A backend-only Spring Boot application that demonstrates secure API access, subscription-based feature control, and usage quota enforcement.  
The system models how real-world SaaS platforms manage authentication, authorization, and plan-based access to protected APIs.

---

## 📌 Project Overview

This project implements a **policy-driven backend system** where users access APIs based on their assigned subscription plan.  
It focuses on backend fundamentals such as security, business rule enforcement, and controlled access rather than frontend functionality.

Key goals:

- Secure REST APIs using JWT authentication
- Role- and plan-based authorization
- Usage tracking and quota enforcement
- Clean API design with proper error handling

---

## 🧠 Core Concepts Implemented

- Authentication vs Authorization
- Role-Based Access Control (RBAC)
- Subscription plans and feature entitlement
- API usage tracking and rate limiting
- Centralized exception handling
- Backend-first system design (no frontend dependency)

---

## 🛠 Tech Stack

- Java 17
- Spring Boot
- Spring Security
- JWT (stateless authentication)
- MySQL
- JPA / Hibernate
- Bean Validation
- Swagger / OpenAPI
- Postman (API testing)

---

## 🔐 Authentication & Authorization

- Users register and log in using secure credentials
- JWT tokens are issued on login
- All protected APIs require a valid JWT
- Access is controlled based on:
  - User role (USER / ADMIN)
  - Subscription plan (FREE / PRO / ADMIN)

---

## 📦 Subscription Plans

| Plan  | Access Level                     |
| ----- | -------------------------------- |
| FREE  | Basic APIs with limited usage    |
| PRO   | Advanced APIs with higher limits |
| ADMIN | Full access without restrictions |

Each plan defines:

- Which APIs can be accessed
- Usage limits per time window

---

## 🔁 API Usage & Limits

- API usage is tracked per user
- Requests exceeding the allowed quota are blocked
- Proper error responses are returned for limit violations

---

## 📄 API Documentation

- Swagger UI is enabled for API exploration
- All endpoints, request/response schemas, and authentication flows are documented
- APIs can be tested using Swagger UI or Postman

---

## 🚀 Project Phases

The project is built incrementally in phases:

1. **Phase 1:** Core backend, security, subscription logic
2. **Phase 2:** Rate limiting, Redis, CI/CD, Docker
3. **Phase 3:** Event-driven logic and WebSockets (optional)
4. **Phase 4:** Payment gateway integration (optional)

Each phase keeps the application in a runnable, resumable state.

---

## 🧪 Running the Application

1. Configure MySQL connection in application properties
2. Build and run the Spring Boot application
3. Access Swagger UI to explore APIs
4. Use Postman for manual testing

---

## 📈 Learning Outcomes

This project demonstrates how to:

- Design secure backend systems
- Enforce business rules at the service layer
- Build production-ready REST APIs
- Apply clean backend architecture principles

---

## 📌 Note

This project is intentionally backend-focused.  
No frontend or UI components are included.

---
