# FlightOps-API-Suite-Simulated-Airline-Operations-Platform

# ✈️ FlightOps API Suite  
**Simulated Airline Operations Platform — Designed for Scale, Built with TDD, and Ready for Production**

> 🛫 From flight scheduling to gate logistics and crew assignments, this backend system replicates the heart of airline operations with enterprise-grade design and robust testing.

---

## 🚀 Overview

**FlightOps API Suite** is a microservice-ready platform built in **Java (Spring Boot)** that simulates key airline operations:

- ✈️ Flight creation, rescheduling, and cancellation  
- 👨‍✈️ Crew assignment and availability tracking  
- 🛬 Gate and terminal logistics with time-bound constraints  
- 🔐 Secure access using **OAuth2 + RBAC**  
- ✅ CI/CD and testing pipelines for production-readiness  

Built with a **TDD-first approach**, this system mirrors the complexity of real airline systems — minus the turbulence.

---

## 🧰 Tech Stack

| Layer       | Tech Used                                                   |
|-------------|-------------------------------------------------------------|
| Backend     | Java 17, Spring Boot, Spring Web, Spring Security           |
| Auth        | OAuth2, JWT                                                 |
| Database    | MSSQL                                                       |
| Testing     | JUnit, Mockito, Postman                                     |
| DevOps      | GitHub Actions, Azure App Services, Terraform (optional)    |
| CI/CD       | GitHub Actions (build, test, deploy)                        |

---

## 🔑 Key Features

- **Modular REST APIs** – Each operation is a dedicated, versioned REST endpoint  
- **OAuth2 Authentication** – Fine-grained role-based access control  
- **Robust Testing** – >85% JUnit coverage with input validation and error simulation  
- **CI Pipeline** – GitHub Actions workflow to run unit and integration tests on push  
- **Simulated Environments** – Simulates real-world ops: overlapping flights, delayed gates, and unassigned crew fallback  
- **Postman Regression Suite** – Scenario-based simulations for validating API contracts  

---

## 📦 Installation

### Prerequisites
- Java 17+
- Maven
- MSSQL (local or cloud)
- Postman (for API testing)

### Setup

```bash
# Clone the repo
git clone https://github.com/ghantapavan93/FlightOps-API-Suite-Simulated-Airline-Operations-Platform
cd flightops-api-suite

# Run tests
mvn test

# Start server
mvn spring-boot:run

🧪 Test & Coverage
bash
Copy
Edit
# Run unit tests
mvn test

# Generate coverage reports
mvn jacoco:report

📌 Sample API Flow
Scenario: A scheduler creates a new flight, assigns available crew, and validates gate availability.

/api/v1/flights → Create flight

/api/v1/crew/assign → Assign crew (conflict check)

/api/v1/gates/allocate → Auto-assign gate based on terminal availability

Response returns full operational metadata

👤 Author
Pavankalyan Ghanta


