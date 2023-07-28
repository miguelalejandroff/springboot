# Microservicio de Gestión de Libros con Spring Boot

Este proyecto es un microservicio desarrollado con Spring Boot que permite gestionar libros a través de una API REST. El microservicio tiene las siguientes capacidades:

- Obtener todos los libros.
- Obtener un libro por su ID.
- Crear un nuevo libro.
- Editar un libro existente.

## Requisitos

- Java 17
- Maven

## Cómo ejecutar el proyecto

1. Clona el repositorio en tu máquina local usando `git clone [url_del_repositorio]`.

2. Navega hasta el directorio del proyecto.

3. Ejecuta `mvn spring-boot:run` para iniciar la aplicación. La aplicación comenzará a escuchar en `http://localhost:8080`.

## Cómo probar la API

La API tiene cuatro endpoints:

- `GET /api/books`: Obtiene todos los libros.
- `GET /api/books/{id}`: Obtiene el libro con el ID dado.
- `POST /api/books`: Crea un nuevo libro. Se debe enviar un cuerpo de solicitud con el título y autor del libro.
- `PUT /api/books/{id}`: Edita el libro con el ID dado. Se debe enviar un cuerpo de solicitud con el nuevo título y/o autor del libro.

Para probar la API, puedes importar la colección de Postman que se encuentra en este repositorio. La colección contiene ejemplos de solicitudes que puedes hacer a la API.

## Base de datos

Este microservicio utiliza una base de datos en memoria H2. La base de datos se crea automáticamente cuando se inicia el microservicio y se destruye cuando se detiene.
