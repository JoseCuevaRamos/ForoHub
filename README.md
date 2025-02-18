# 📢 ForoHub - Desafío con Spring Framework

[![Java](https://img.shields.io/badge/Java-17-orange?style=for-the-badge)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.3-green?style=for-the-badge)](https://spring.io/projects/spring-boot)
[![Spring Security](https://img.shields.io/badge/Spring%20Security-Auth-red?style=for-the-badge)](https://spring.io/projects/spring-security)
[![JWT](https://img.shields.io/badge/JWT-Auth-yellow?style=for-the-badge)](https://jwt.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue?style=for-the-badge)](https://www.postgresql.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8-lightblue?style=for-the-badge)](https://www.mysql.com/)
[![Lombok](https://img.shields.io/badge/Lombok-Annotations-green?style=for-the-badge)](https://projectlombok.org/)
[![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-purple?style=for-the-badge)](https://swagger.io/)
[![Flyway](https://img.shields.io/badge/Flyway-Migrations-red?style=for-the-badge)](https://flywaydb.org/)

🚀 **ForoHub** es una API RESTful desarrollada con **Spring Framework** que permite gestionar un **foro de discusión** en el que los usuarios pueden **crear, consultar, actualizar y eliminar** temas de conversación.  
Además, ofrece autenticación segura con **JWT**, gestión de roles y documentación con **Swagger**.

---

## 🎯 Objetivos del Proyecto

✅ **Implementar una API REST** siguiendo las mejores prácticas del modelo REST.  
✅ **Aplicar validaciones** para garantizar la integridad de los datos y la seguridad.  
✅ **Utilizar una base de datos relacional** para almacenamiento persistente.  
✅ **Configurar autenticación y autorización** con **Spring Security y JWT**.  
✅ **Opcionalmente, documentar la API** utilizando **Swagger**.  

---

## 🌟 Características Principales

### 🔐 **Seguridad y Autenticación**
- 👤 **Autenticación y autorización de usuarios.**
- 🔒 **Implementación de JWT (JSON Web Tokens) para autenticación segura.**
- 🔑 **Uso de BCryptPasswordEncoder para encriptar contraseñas.**
- 🔐 **Gestión de roles y permisos de usuarios.**
- 🔄 **Arquitectura STATELESS para mayor escalabilidad.**

### 📝 **Funcionalidades del Foro**
- 🏷️ **Gestión de temas de discusión** (CRUD de tópicos).
- 💬 **Sistema de comentarios** en tópicos.
- 📌 **Uso de enums** para categorías dentro de los temas.

### 🛠 **API y Manejo de Datos**
- 🔧 **Endpoints específicos según roles de usuario.**
- 📩 **Respuestas API personalizadas** (`DataResponse`, `ApiResponse`).
- ⚠️ **Manejo de excepciones y validaciones de entrada.**
- 📆 **Gestión automática de fechas** con `@PrePersist` y `@PreUpdate`.

### 📚 **Documentación**
- 📖 **Swagger UI** para explorar y probar los endpoints de la API.

---

## 🔥 Funcionalidades Adicionales
- 🚀 **Opcionalmente, implementar endpoints adicionales:**
  - `/api/usuarios` → Gestión de usuarios.
  - `/api/respuestas` → Sistema de respuestas/comentarios en temas.


---

### 🔐 **Autenticación y Seguridad**
Los usuarios deben autenticarse con JWT para acceder a los **endpoints protegidos**.  
Ejemplo de autenticación con **JWT** en las cabeceras:

```http
Authorization: Bearer <tu-token-jwt>
