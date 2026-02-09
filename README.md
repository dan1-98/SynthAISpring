# SpringProyect1 - Base Spring Boot Application

![Java](https://img.shields.io/badge/Java-17-orange) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.4.2-green) ![Docker](https://img.shields.io/badge/Docker-Ready-blue)

## 🤖 Generative AI Proof of Concept
This project serves as a **Proof of Concept (PoC)** generated entirely using **Generative AI Agents**. It demonstrates the capability of AI to scaffold, implement, test, and containerize a modern Java application with zero manual coding.

## 📋 About The Application
This is a production-ready template for a Spring Boot application that integrates three core capabilities:
1.  **Web API**: RESTful endpoints using Spring MVC.
2.  **Batch Processing**: Robust batch job scheduling and execution using Spring Batch.
3.  **Testing**: Comprehensive unit and integration testing suite.

## 🛠️ Technology Stack
*   **Language**: Java 17 (OpenJDK)
*   **Framework**: Spring Boot 3.4.2
*   **Build Tool**: Maven 3.9+
*   **Database**: H2 (In-Memory for Batch metadata)
*   **Containerization**: Docker & Docker Compose

## 🚀 Key Features
*   **Standard Directory Layout**: Follows Maven best practices.
*   **Health Check Endpoint**: Simple `/hello` endpoint for connectivity verification.
*   **Sample Batch Job**: A pre-configured job (`sampleJob`) that executes on startup.
*   **CI/CD Ready**: Includes `Dockerfile` and `docker-compose.yml`.

## 🏃 Getting Started

### Prerequisites
*   Java 17+
*   Maven 3.6+
*   Docker (Optional)

### Running Locally
1.  **Clone the repository**.
2.  **Build the project**:
    ```bash
    mvn clean package
    ```
3.  **Run the application**:
    ```bash
    mvn spring-boot:run
    ```
    *Access the endpoint at: `http://localhost:8080/hello`*

### Running with Docker 🐳
No need to install Java or Maven locally!
```bash
docker-compose up --build
```

### Running Tests
Execute the full test suite (Web + Batch):
```bash
mvn test
```

## 📂 Project Structure
```
src/
├── main/
│   ├── java/.../batch/   # Batch Configuration and Jobs
│   ├── java/.../web/     # REST Controllers
│   └── resources/        # Config (application.properties)
└── test/                 # Unit and Integration Tests
```
