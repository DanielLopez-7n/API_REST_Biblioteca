# 📚 API REST de Biblioteca

Esta es una API construida con **Django** y **Django REST Framework** para gestionar el inventario y los préstamos de una biblioteca. 

## 🚀 Características Principales

* **Gestión de Autores:** Registro de autores con su información básica y nacionalidad.
* **Gestión de Libros:** Control del catálogo de libros, incluyendo disponibilidad, género y relación con su autor.
* **Sistema de Préstamos:** Permite a los usuarios registrados solicitar préstamos de libros y registrarlos cuando son devueltos. La API valida automáticamente que un libro no pueda ser prestado si ya está en uso.

## 🛠️ Tecnologías Usadas

* Python
* Django
* Django REST Framework
* SQLite (Base de datos por defecto)

## 📌 Endpoints Principales

La API cuenta con varias rutas para interactuar con los datos. Algunas de las más importantes son:

* `/api/libros/` - Lista todos los libros.
* `/api/libros/disponibles/` - Muestra únicamente los libros que se pueden prestar.
* `/api/libros/{id}/prestar/` - Acción para prestar un libro específico.
* `/api/prestamos/` - Historial de préstamos (los usuarios solo ven los suyos).
* `/api/prestamos/{id}/devolver/` - Acción para registrar la devolución de un libro.