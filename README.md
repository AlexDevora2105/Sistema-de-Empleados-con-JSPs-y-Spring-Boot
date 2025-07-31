# Desarrollo de Sistema de Empleados con JSPs y Spring Boot

CRUD completo con validaciones, búsqueda y lógica condicional, además incluye la parte visual para el usuario final.

---

## 🎯 Qué hace

- Permite registrar Empleados con:
    - Nombre, Departamento, y Sueldo
- Permite listar, editar, eliminar

---

## 🧩 Prácticas pendientes que aplicar
- Agregar email del empleado
- Agregar edad del empleado
- Valida emails, validar longitud de texto en el nombre, validar negativos de edad.
- - `@Valid`, `@Email`, `@Min`, `@Size`



## 💾 Base de Datos MySql 
✅ La base de datos se crea de forma automatica si no existe en tu Gestor de Base de Datos. 

✔️ La configuracin para lograr esto, se encuentra en el archivo `application.properties`

```
# Conexion mysql
spring.datasource.url=jdbc:mysql://localhost:3306/empleados_db?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=Devora
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# Si la base de datos no existe, se debe crear de forma automatica con la siguiente linea // Si ya existiera la base de datos y no queremos que se cree o sobreescriba el valor debe ser none y quitar el parametro de la linea 4
spring.jpa.hibernate.ddl-auto=update

# Mostrar sentencias SQL
spring.jpa.show-sql=true
```