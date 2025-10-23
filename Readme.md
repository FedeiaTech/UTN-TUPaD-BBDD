# Trabajo Práctico Integrador – Bases de Datos I

**Universidad Tecnológica Nacional (UTN)** – Tecnicatura Universitaria en Programación a Distancia

## Título del trabajo: Trabajo Final Integrador (TFI) – Bases de Datos I

* **Materia:** Bases de Datos I
* **Profesor Coordinador:** Oscar Londero
* **Fecha de entrega:** 23/10/2025

---

## Integrantes

| Nombre              | Comisión | Email                     |
| :------------------ | :------- | :------------------------ |
| Eric Suárez Dubs    | 13       | ericgodzilladubs@gmail.com |
| Gonzalo Vega        | 11       | gonzaarg03@gmail.com      |
| Federico Iacono     | 6        | iaconofede@gmail.com      |
| Mateo Serafini      | 5        | matuserafini@gmail.com    |

---

## Video Explicativo

**YouTube – Presentación del proyecto:** [https://youtu.be/JCD1Q-m4_KM?si=yaOb2_iOfDZiR0Zx](https://youtu.be/JCD1Q-m4_KM?si=yaOb2_iOfDZiR0Zx)

---

## Descripción General

Este proyecto consiste en el desarrollo de un modelo de base de datos especializado en la gestión de códigos de barras de productos, implementado en MySQL Workbench.

El trabajo integra conocimientos teóricos y prácticos sobre diseño lógico y físico de bases de datos, normalización, integridad, seguridad, concurrencia y rendimiento.

El objetivo es construir una solución sólida, escalable y alineada con los estándares profesionales, que sirva como modelo de referencia para entornos reales de administración de productos e inventarios.

---

## Estructura del Proyecto

El proyecto se organiza en cinco etapas principales, cada una acompañada por sus scripts SQL y evidencias de ejecución.

### Etapa 1 – Modelado y Definición de Constraints

* Diseño del modelo relacional (`tpi_productos`) con las tablas `productos` y `codigos_barras`.
* Definición de dominios, PK, FK, CHECK, UNIQUE y índices.
* Validación práctica mediante inserciones válidas e inválidas.

### Etapa 2 – Generación y Carga Masiva de Datos

* Procedimiento almacenado `GenerarDatosMasivos` con funciones aleatorias y control transaccional.
* Carga de más de 600.000 registros respetando la integridad referencial.
* Análisis de rendimiento: mejora del 92.2% en consultas con índice.

### Etapa 3 – Consultas Avanzadas y Reportes

* Consultas con `JOIN`, `GROUP BY`, `HAVING` y subconsultas.
* Reportes útiles sobre precios, categorías, marcas y promedios.
* Evaluación comparativa con y sin índices para medir eficiencia.

### Etapa 4 – Seguridad e Integridad

* Creación de un usuario con privilegios mínimos.
* Implementación de vistas públicas para ocultar datos sensibles.
* Uso de `CONCAT` para prevenir inyección SQL.
* Pruebas de integridad (duplicados, precios negativos, referencias inexistentes).

### Etapa 5 – Concurrencia y Transacciones

* Simulación de deadlocks entre sesiones concurrentes.
* Procedimiento almacenado con manejo de retry y registro de errores.
* Comparación de niveles de aislamiento (`READ COMMITTED` vs `REPEATABLE READ`).

---