# Sample Spring Kafka Microservices  

This project demonstrates a **microservices-based architecture** using **Spring Boot** and **Apache Kafka** for real-time communication between distributed services. It showcases how to design and implement **event-driven systems** where microservices publish and consume messages asynchronously, enabling scalability and fault tolerance.  

---

## 🚀 Features
- Event-driven communication with **Apache Kafka**.  
- Multiple Spring Boot microservices interacting asynchronously.  
- Dockerized setup for easy local deployment.  
- REST endpoints to produce/consume Kafka events.  
- Example use case: banking transactions & notifications.  

---

## 🛠️ Technologies Used
- **Backend Framework:** Spring Boot, Spring Cloud  
- **Messaging System:** Apache Kafka  
- **Build Tool:** Maven / Gradle  
- **Containerization:** Docker, Docker Compose  
- **Database (optional):** PostgreSQL / MySQL  
- **Other Tools:** Zookeeper, Lombok, Swagger  

---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/AmishNavadia/spring-kafka-microservices.git
cd spring-kafka-microservices
```

2. Start Kafka with Docker

Make sure Docker is installed and running. Start Kafka & Zookeeper using Docker Compose:
```bash
docker-compose up -d
```
3. Build the Microservices

Navigate into each microservice folder (e.g., producer-service, consumer-service) and run:
```bash
mvn clean install
```
4. Run the Services

You can start each Spring Boot service with:
```bash
mvn spring-boot:run
```

Or run all together with Docker Compose (if configured):
```bash
docker-compose up --build
```

📊 Usage

Start the Kafka broker & microservices.

Use the Producer REST API to send messages.

POST http://localhost:8080/api/v1/messages
Body: { "message": "Hello Kafka" }


The Consumer Service will automatically receive and log/process the message.
