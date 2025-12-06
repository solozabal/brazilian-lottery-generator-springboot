# 🎲 Brazilian Lottery Bet Generator

![Java](https://img.shields.io/badge/Java-11%2B-blue.svg)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-2.7-brightgreen.svg)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-%23336791.svg?&style=flat&logo=postgresql&logoColor=white)
![Build](https://img.shields.io/badge/build-passing-success)
![License](https://img.shields.io/github/license/solozabal/brazilian-lottery-generator-springboot)
<p align="center">
<img src="https://raw.githubusercontent.com/solozabal/brazilian-lottery-generator-springboot/main/assets/lottery-banner-v2.png" width="900" alt="Brazilian Lottery Banner">
</p>

Welcome to the **Brazilian Lottery Bet Generator**, an open source project built with Java & Spring Boot!  
Effortlessly generate bets for the main Brazilian lottery games: **Mega Sena**, **Quina**, and **LotoFácil**.  
Designed for both fun and learning, this project demonstrates professional use of modern Java frameworks, clean architecture and an appealing interface.

---

## 🧩 Features

- **Mega Sena:**  
  Select 6 numbers from 1 to 60, or let the system surprise you with a random selection ("Surpresinha").
- **Quina:**  
  Select 5 numbers between 1 and 80. Or use the automatic randomizer.
- **LotoFácil:**  
  Pick between 15 and 20 numbers from a set of 25. Win by matching 11 to 15 numbers!  
  Random selection supported as well.
- Fully responsive UI with **Thymeleaf** and **Bootstrap**.
- Clean separation of concerns (Controller, Service, Model, Repository).
- Built-in support for **PostgreSQL** database.

---

## 🚀 Tech Stack

- [Java 11+](https://www.java.com/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [PostgreSQL](https://www.postgresql.org/)
- [Thymeleaf (HTML templates)](https://www.thymeleaf.org/)
- [Bootstrap](https://getbootstrap.com/)

---

## ⚙️ Getting Started

### Prerequisites

- **Java 11** or newer
- **Maven**
- **PostgreSQL** (running locally or in the cloud)

### Database Setup

Ensure PostgreSQL is installed and running.  
Create the new database:

```sql
CREATE DATABASE gerador_de_apostas;
```

Update your `src/main/resources/application.properties` with your PostgreSQL credentials:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/gerador_de_apostas
spring.datasource.username=your_postgres_user
spring.datasource.password=your_postgres_password
spring.jpa.hibernate.ddl-auto=update
```

### Running the Application

Clone the repository:

```bash
git clone https://github.com/solozabal/brazilian-lottery-generator-springboot.git
cd brazilian-lottery-generator-springboot
```

Build and run the application:

```bash
./mvnw spring-boot:run
```

Visit the app in your browser:

```text
http://localhost:8080
```

---

## 🗂 Project Structure

```plaintext
src/main/java/com/example/geradordeapostas/gerador_de_apostas
├── GeradorDeApostasApplication.java       // Main Spring Boot application class
├── controller/JogoController.java         // Handles HTTP requests for lottery games
├── model/Jogo.java                        // JPA Entity for game data
├── repository/JogoRepository.java         // JPA Repository for game persistence
└── service/JogoService.java               // Business logic for bet generation

src/main/resources
├── application.properties                 // Application configuration
└── templates/index.html                   // Main Thymeleaf HTML page
```

---

## 🤝 Contributing

We welcome contributions from everyone! 🚀

1. Fork this repo
2. Create a feature branch:
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. Commit your changes:
   ```bash
   git commit -am 'Add some amazing feature'
   ```
4. Push to your branch:
   ```bash
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request!

---

## 🌎 Why This Project?

- **Showcase your Java and Spring Boot skills in your portfolio!**
- Clear demonstration of backend–frontend integration with Thymeleaf and Bootstrap.
- Hands-on example of deploying a Java web project with PostgreSQL.
- Great for technical interviews, take-home challenges, or teaching MVC and database integration.

---

## 💡 License

This project is licensed under the MIT License.

---

<p align="center">
  <a href="https://www.linkedin.com/in/pedrosolozabal/">
    <img src="https://img.shields.io/badge/Pedro%20Solozabal-LinkedIn-blue?logo=linkedin&logoColor=white&style=for-the-badge" alt="Pedro Solozabal on LinkedIn">
  </a>
</p>