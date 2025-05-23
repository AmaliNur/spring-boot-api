# 👨‍💻 Spring Boot REST API — Software Engineers

Простой CRUD API, реализованный с использованием **Spring Boot** и **Spring Data JPA**, позволяющий управлять сущностями разработчиков программного обеспечения. Приложение подключается к базе данных **PostgreSQL**, запущенной в контейнере **Docker**.

## 🚀 Возможности

* Получение списка всех Software Engineers
* Получение Software Engineer по ID
* Добавление нового Software Engineer
* Использование PostgreSQL в Docker-контейнере
* Простая и чистая архитектура (Controller → Service → Repository)

## 🧰 Стек технологий

* Java 21
* Spring Boot
* Spring Data JPA
* PostgreSQL
* Maven
* Docker & Docker Compose
* IntelliJ IDEA

## 📦 Установка и запуск

### 1. Клонировать репозиторий

```bash
git clone https://github.com/AmaliNur/spring-boot-api.git
cd spring-boot-api
```

### 2. Запустить PostgreSQL и приложение через Docker

```bash
docker-compose up --build
```

API будет доступен по адресу:

```
http://localhost:8080/api/v1/software-engineers
```

## 📘 Примеры запросов

* **GET** `/api/v1/software-engineers` — список всех инженеров
* **GET** `/api/v1/software-engineers/{id}` — получить инженера по ID
* **POST** `/api/v1/software-engineers` — добавить нового инженера

Пример тела POST-запроса:

```json
{
  "name": "Alice Smith",
  "techStack": "Java, Spring Boot"
}
```

## 📂 Структура проекта

```
src/
└── main/
    └── java/
        └── com.nuritdinov/
            ├── SoftwareEngineer.java
            ├── SoftwareEngineerController.java
            ├── SoftwareEngineerService.java
            └── SoftwareEngineerRepository.java
```

## ⚙️ Конфигурация БД

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/software_engineers
spring.datasource.username=postgres
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
```

## 📄 Лицензия

Проект распространяется под лицензией MIT.

## 📬 Контакты

* GitHub: [github.com/AmaliNur](https://github.com/AmaliNur)
* LinkedIn: [linkedin.com/in/amalinuritdinov](https://www.linkedin.com/in/amalinuritdinov/)
* Telegram: https://t.me/Amali_Nur

