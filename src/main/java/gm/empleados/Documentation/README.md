# Sistema de Gestión de Empleados

---

## Descripción del Proyecto

Este proyecto es un sistema de gestión web para la administración de empleados, desarrollado con **Spring Boot**. El objetivo principal es ofrecer una plataforma robusta y escalable para realizar operaciones **CRUD** (Crear, Leer, Actualizar, Borrar) sobre los datos del personal.

---

## Características Principales

* **Gestión de Empleados**: Permite el registro, consulta, actualización y eliminación de información de empleados.
* **Interfaz de Usuario Web**: Desarrollada con **JSP** y **JSTL** para una interacción intuitiva y dinámica.
* **Persistencia de Datos**: Los datos se gestionan a través de una base de datos **MySQL** con el uso de **JPA** e **Hibernate**.
* **Código Conciso**: Implementación de la librería **Lombok** para reducir la cantidad de código repetitivo (**boilerplate**).

---

## Tecnologías Utilizadas

* **Backend**: Spring Boot, Java, JPA, Hibernate, Lombok
* **Frontend**: JSP, JSTL
* **Base de Datos**: MySQL
* **Servidor**: Tomcat (integrado en Spring Boot)
* **Gestor de Dependencias**: Maven

---

## Requisitos del Sistema

Para compilar y ejecutar el proyecto, necesitarás lo siguiente:

* **JDK 24** o superior
* **Maven**
* **MySQL Server**
* Un IDE compatible con Spring Boot y Maven (como IntelliJ IDEA o Visual Studio Code)

---

## Estructura del Proyecto

La estructura del proyecto sigue el estándar de Spring Boot para facilitar su desarrollo y mantenimiento:

```
├── pom.xml
├── src
│   ├── main
│   │   ├── java
│   │   │   └── gm
│   │   │       └── empleados
│   │   │           ├── modelo
│   │   │           │   └── Empleado.java
│   │   │           ├── controlador
│   │   │           │   └── ControladorInicio.java
│   │   │           ├── servicio
│   │   │           │   └── EmpleadoServicio.java
│   │   │           └── repositorio
│   │   │               └── EmpleadoRepositorio.java
│   │   ├── resources
│   │   │   ├── static
│   │   │   └── application.properties
│   │   └── webapp
│   │       └── WEB-INF
│   │           └── paginas
│   │               └── listado.jsp
│   └── test
└── README.md
```

---

## Cómo Ejecutar el Proyecto

1.  **Clonar el repositorio:**
    `git clone https://github.com/tu-usuario/nombre-del-repositorio.git`

2.  **Configurar la base de datos:**
    * Crea una base de datos en MySQL con el nombre `empleados_bd`.
    * Configura la conexión a la base de datos en el archivo `src/main/resources/application.properties`.

3. **Importar estructura y datos a la base de datos empleados_bd ya creada en el paso anterior**
    * Data Import selecciona la carpeta importarBD_empleados

4. **Compilar y ejecutar:**
    * Desde la terminal, navega hasta el directorio raíz del proyecto.
    * Ejecuta el proyecto con el siguiente comando de Maven:
      `mvn spring-boot:run`
    * También puedes ejecutar la clase principal se encuentra en src/main/java/gm.empleados/servicio `EmpleadosApplication.java` directamente desde tu IDE.

5. **Acceder a la aplicación:**
    * Una vez que la aplicación se haya iniciado, ábrela en tu navegador en la siguiente URL:
      `http://localhost:8081/empleados/`

---

## Contribución

Las contribuciones son bienvenidas. Si encuentras un error o tienes una idea de mejora, no dudes en abrir un *issue* o enviar un *pull request*.

---

## Licencia

Este proyecto le pertenece a @jherraizsoler autor de este repositorio, tiene todos los permisos y derechos de autor.
Este repositorio no se puede copiar o modificar sin autorización del autor expresamente.