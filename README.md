# 🏋️ Zona Fit - Sistema de Gestión de Clientes (Spring Boot)

Aplicación de consola desarrollada en **Java 21** y **Spring Boot** para la gestión integral (CRUD) de clientes y membresías de un gimnasio, conectada a una base de datos relacional **MySQL** mediante **Spring Data JPA**.

---

## 🚀 Funcionalidades

El sistema cuenta con un menú interactivo por consola que permite ejecutar las siguientes operaciones:

1. **Listar Clientes:** Recupera y muestra todos los socios registrados en la base de datos.
2. **Buscar Cliente por ID:** Consulta la información detallada de un cliente específico.
3. **Agregar Cliente:** Registra un nuevo socio validando que el número de membresía sea único.
4. **Modificar Cliente:** Actualiza los datos (nombre, apellido y número de membresía) de un registro existente.
5. **Eliminar Cliente:** Da de baja un cliente del sistema a partir de su ID.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Java 21
* **Framework:** Spring Boot 3 (Spring Data JPA)
* **Base de Datos:** MySQL
* **Gestor de Dependencias:** Maven
* **Librerías Adicionales:** Lombok, MySQL Connector/J

---

## 📂 Arquitectura del Proyecto

El código está estructurado siguiendo el patrón de diseño en capas:

```text
src/main/java/gm/zona_fit/
├── modelo/          # Entidad JPA (Cliente) mapeada a la tabla de MySQL
├── repositorio/     # Interfaz IClienteRepositorio extendiendo de JpaRepository
├── servicio/        # Lógica de negocio (IClienteServicio y ClienteServicio)
└── ZonaFitApplication.java  # Punto de entrada (CommandLineRunner) y menú de consola

