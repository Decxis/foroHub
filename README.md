# Proyecto de Foro con Spring Boot y MySql

Este proyecto consiste en la creación de un sistema de foro que incluye autenticación y autorización mediante JWT (JSON Web Tokens). Utiliza Spring Boot como framework principal y MySql como base de datos.

## Características

- Autenticación y autorización segura con JWT.
- CRUD completo para la gestión de tópicos en el foro.
- Validación de usuarios registrados para crear, actualizar y eliminar tópicos.
- Respuestas HTTP con códigos de estado adecuados (e.g., 201 para creación exitosa, 200 para operaciones exitosas, 403 para accesos no autorizados).
- Organización de tareas usando una metodología ágil con herramientas como Trello.

## Tecnologías utilizadas ⚒️

- Java
- Spring Boot
- Spring Security
- JWT (JSON Web Tokens)
- JPA (Java Persistence API)
- H2 Database (para desarrollo y pruebas)
- Postman (para pruebas de API)
- Swagger (para documentación de API)

## Instalación y Configuración

1. **Clonar el repositorio**:
   ```bash
   https://github.com/Decxis/foroHub.git
   ```

3. **Probar los endpoints**:
   Utiliza Postman o cualquier cliente API para interactuar con los endpoints.

## Endpoints Principales

### Autenticación
- **POST /auth/login**
  - Parámetros: `username`, `password`.
  - Respuesta: Devuelve un token JWT si las credenciales son válidas.

### Gestión de Tópicos
- **GET /topics**
  - Retorna una lista de tópicos.
  - Requiere un token JWT válido.

- **POST /topics**
  - Crea un nuevo tópico.
  - Requiere un token JWT válido.

- **PUT /topics/{id}**
  - Actualiza un tópico existente.
  - Requiere un token JWT válido.

- **DELETE /topics/{id}**
  - Elimina un tópico.
  - Requiere un token JWT válido.

## Uso de JWT

- Al iniciar sesión, se genera un token JWT.
- Incluye este token en la cabecera de las solicitudes protegidas:


## Organización del Proyecto

Se utilizó Trello para organizar las tareas del proyecto en pequeñas actividades manejables. Cada tarea está documentada y categorizada en el tablero de Trello.


## Contribuciones

Si deseas contribuir al proyecto, ¡eres bienvenido/a! Haz un fork del repositorio, crea una rama y envía tu pull request.

