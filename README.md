# 📚 API de Gestión de Libros

API RESTful desarrollada con **Kotlin + Spring Boot** para gestionar una librería personal. Permite crear, consultar, actualizar, eliminar y buscar libros por título o autor. Utiliza PostgreSQL como base de datos.

---

## 🚀 Tecnologías utilizadas

- Kotlin
- Spring Boot (Web, Data JPA)
- PostgreSQL
- Gradle
- Postman (para pruebas)

---

## 📁 Estructura del proyecto

bookapi/
├── controller/ # Controladores REST
├── model/ # Entidades JPA
├── repository/ # Acceso a datos
├── service/ # Lógica de negocio
├── resources/
│ └── application.properties
└── build.gradle.kts


---

## ⚙️ Configuración del entorno

### Requisitos

- Java 17 o 21
- PostgreSQL
- Gradle
- VS Code o IDE compatible

### Base de datos

1. Crear la base:

Nombre: bookapidb
Usuario: bookuser
Contraseña: bookpass


2. Editar `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/bookapidb
spring.datasource.username=bookuser
spring.datasource.password=bookpass
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
server.port=8080


./gradlew bootRun

EJEMPLO:

{
  "title": "Clean Code",
  "author": "Robert C. Martin",
  "year": 2008,
  "isbn": "9780132350884",
  "read": false
}

