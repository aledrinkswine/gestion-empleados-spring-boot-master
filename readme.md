# 👨‍💼 Gestión de Empleados – Spring Boot

Este proyecto es una **aplicación web de gestión de empleados** desarrollada con **Spring Boot**, **Spring MVC**, **Spring Data JPA** y **Thymeleaf**. Permite realizar operaciones CRUD completas sobre empleados, con autenticación básica y paginación.

Está orientado a **aprendizaje práctico** y como base para sistemas administrativos más completos.

---

## 🚀 Funcionalidades

- ✅ Listado de empleados con paginación
- ➕ Crear nuevos empleados
- ✏️ Editar empleados existentes
- ❌ Eliminar empleados
- 🔍 Ver detalle de un empleado
- 🔐 Login básico
- 🌐 Internacionalización (i18n)
- 📄 Vistas con Thymeleaf

---

## 🛠️ Tecnologías utilizadas

- **Java 11+**
- **Spring Boot**
- **Spring MVC**
- **Spring Data JPA**
- **Spring Security (básico)**
- **Thymeleaf**
- **Hibernate**
- **Maven**
- **MySQL / H2 (configurable)**

---

## 📁 Estructura del proyecto

```
gestion-empleados-spring-boot-master/
└── mini-control-empleados/
    ├── pom.xml
    ├── mvnw / mvnw.cmd
    ├── src/
    │   ├── main/
    │   │   ├── java/com/gestion/empleados/
    │   │   │   ├── controllers/
    │   │   │   ├── models/
    │   │   │   ├── repositories/
    │   │   │   ├── services/
    │   │   │   └── MiniControlEmpleadosApplication.java
    │   │   └── resources/
    │   │       ├── templates/
    │   │       │   ├── layout/
    │   │       │   ├── listar.html
    │   │       │   ├── form.html
    │   │       │   ├── ver.html
    │   │       │   └── login.html
    │   │       ├── application.properties
    │   │       └── messages.properties
    │   └── test/
    │       └── MiniControlEmpleadosApplicationTests.java
```

---

## ⚙️ Configuración del proyecto

### 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/aledrinkswine/gestion-empleados-spring-boot.git
cd mini-control-empleados
```

### 2️⃣ Configurar base de datos

En el archivo `application.properties` puedes configurar la base de datos:

```properties
spring.datasource.url=jdbc:mysql://localhost/empleados_db
spring.datasource.username=root
spring.datasource.password=tu_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

> 💡 Puedes usar **H2** para pruebas locales sin configuración adicional.

---

## ▶️ Ejecutar la aplicación

Con Maven Wrapper:

```bash
./mvnw spring-boot:run
```

O en Windows:

```bash
mvnw.cmd spring-boot:run
```

La aplicación estará disponible en:

```
http://localhost:8080
```

---

## 🔐 Acceso al sistema

Credenciales por defecto (si están configuradas):

```
Usuario: admin
Contraseña: admin
```

*(Puede variar según la configuración de Spring Security)*

---

## 🧩 Capas de la aplicación

- **Controller**: maneja las peticiones HTTP
- **Service**: lógica de negocio
- **Repository**: acceso a datos con JPA
- **Model/Entity**: entidades del sistema
- **View**: vistas Thymeleaf

---

## 🌍 Internacionalización (i18n)

Los textos de la aplicación se gestionan desde:

```
messages.properties
```

Esto permite soportar múltiples idiomas fácilmente.

---

## 🧪 Posibles mejoras futuras

- Roles y permisos avanzados
- Validaciones más robustas
- API REST
- Frontend con Angular o React
- Dockerización

---

## 📄 Licencia

Proyecto desarrollado con fines **educativos** y de **aprendizaje**.

---
## 👨‍💻 Autor

**Manuel Alejandro** - Desarrollador Full Stack

---