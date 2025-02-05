# Gestión de Clientes y Facturación con FastAPI - Alberto

## Descripción
Este proyecto práctico consiste en desarrollar una API RESTful utilizando FastAPI para gestionar clientes, facturas y transacciones. Debes aplicar los conceptos aprendidos en el Curso de FastAPI, como: la creación de endpoints, validación de datos, autenticación, integración con bases de datos y pruebas automatizadas. El objetivo es construir una solución funcional y escalable que simule un caso de uso real.

## Criterios de Evaluación
El proyecto será evaluado con base en los siguientes criterios:

1. **Funcionalidad (40%)**:
   - Los endpoints deben cumplir con los requisitos especificados.
   - La API debe manejar correctamente las operaciones CRUD (Crear, Leer, Actualizar, Eliminar).

2. **Calidad del Código (20%)**:
   - El código debe seguir buenas prácticas de programación.
   - Debe ser modular, legible y fácil de mantener.

3. **Pruebas (20%)**:
   - Se deben incluir pruebas unitarias y de integración.
   - La cobertura de pruebas debe ser adecuada.

4. **Documentación (10%)**:
   - La API debe incluir documentación generada automáticamente con Swagger.
   - Se debe proporcionar un archivo README claro y completo.

5. **Autenticación y Seguridad (10%)**:
   - Implementación de autenticación básica.
   - Manejo adecuado de errores y validación de datos.

## Requisitos Técnicos
- **Framework**: FastAPI.
- **Base de Datos**: SQLite.
- **Validación de Datos**: Pydantic.
- **Autenticación**: HTTP Basic Credentials.
- **Pruebas**: Pytest.
- **Documentación**: Swagger (OpenAPI).

## Issues a Resolver
A continuación, se presentan los issues que los estudiantes deben resolver:

### **Nivel 1: Fundamentos**
1. **Crear un endpoint para listar clientes**:
   - Endpoint: `GET /customers`
   - Retorna una lista de clientes almacenados en la base de datos.

2. **Crear un endpoint para agregar un cliente**:
   - Endpoint: `POST /customers`
   - Recibe un JSON con los datos del cliente y los almacena en la base de datos.

3. **Validar los datos de entrada con Pydantic**:
   - Asegúrate de que los datos del cliente (nombre, email, etc.) sean válidos antes de almacenarlos.

---

### **Nivel 2: Intermedio**
4. **Implementar un endpoint para actualizar un cliente**:
   - Endpoint: `PUT /customers/{id}`
   - Permite actualizar los datos de un cliente existente.

5. **Crear un endpoint para eliminar un cliente**:
   - Endpoint: `DELETE /customers/{id}`
   - Elimina un cliente de la base de datos.

6. **Agregar paginación a la lista de clientes**:
   - Permite obtener los clientes en páginas, con un número configurable de resultados por página.

---

### **Nivel 3: Avanzado**
7. **Crear un modelo y endpoints para gestionar facturas**:
   - Endpoints:
     - `POST /invoices`: Crear una nueva factura.
     - `GET /invoices`: Listar todas las facturas.
   - Cada factura debe estar asociada a un cliente.

8. **Implementar autenticación básica**:
   - Requiere que los usuarios se autentiquen para acceder a los endpoints.

9. **Escribir pruebas unitarias para los endpoints**:
   - Utiliza Pytest para probar la funcionalidad de los endpoints.

---

### **Nivel 4: Experto**
10. **Agregar un endpoint para calcular el total de una factura**:
    - Endpoint: `GET /invoices/{id}/total`
    - Calcula el total de una factura sumando los montos de las transacciones asociadas.

11. **Optimizar el rendimiento de la API**:
    - Implementa consultas eficientes para reducir el tiempo de respuesta.

12. **Extender la API con funcionalidades adicionales**:
    - Por ejemplo, agregar notificaciones por email al crear una factura.

---

## Cómo Empezar
1. Clona este repositorio.
2. Resuelve los issues en el orden indicado.
