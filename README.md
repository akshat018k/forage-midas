# JPMorgan Chase & Co. – Software Engineering Job Simulation (Forage)

## 📌 Overview
This project is part of the **JPMorgan Chase & Co. Software Engineering Job Simulation** hosted on **Forage**.  
It simulates real-world backend engineering tasks commonly performed in large-scale financial systems, focusing on microservices, messaging, databases, and RESTful APIs.

The application processes high-volume financial transactions, validates business rules, persists data, integrates with external services, and exposes REST endpoints for querying user balances.

---

## 🛠️ Technologies Used
- **Java**
- **Spring Boot**
- **Spring Data JPA**
- **Apache Kafka**
- **H2 SQL Database**
- **REST APIs**
- **Maven**
- **JUnit / Spring Test Framework**

---

## 🧩 Key Features
- Kafka-based transaction message consumption
- Transaction validation and persistence
- Relational entity modeling with JPA
- External REST API integration
- Balance querying REST endpoint
- Automated testing and debugging

---

## ⚙️ System Architecture
- **Kafka Consumer** listens to transaction topics
- **Service Layer** validates and processes transactions
- **Persistence Layer** stores data using JPA and H2
- **External API Client** communicates with Incentive API
- **REST Controller** exposes balance query endpoints

---

## 🚀 Implementation Details

### 1. Kafka Integration
- Configured Kafka consumers to read high-volume transaction messages
- Deserialized incoming messages into domain objects
- Used embedded Kafka for local testing

### 2. Transaction Processing
- Implemented validation logic for incoming transactions
- Applied business rules before persisting data
- Updated user balances atomically

### 3. Database & Persistence
- Designed relational entities using **Spring Data JPA**
- Used **H2 in-memory database** for fast testing and development
- Ensured data consistency across user records

### 4. External API Integration
- Connected to an external **Incentive REST API** using `RestTemplate`
- Processed incentive responses and integrated them into transaction workflows

### 5. REST API Development
- Developed REST endpoints to retrieve user balances
- Returned structured JSON responses
- Maintained clean separation of controller, service, and repository layers

### 6. Testing & Debugging
- Verified system behavior using **Maven test suites**
- Debugged message ingestion, database operations, and API interactions
- Ensured reliability and correctness across all components

---

## ▶️ How to Run the Project
1. Clone the repository
   ```bash
   git clone <repository-url>
