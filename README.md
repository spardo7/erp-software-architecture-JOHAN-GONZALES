# Proyecto ERP - Grupo X

Este repositorio contiene la **documentación de la arquitectura del sistema ERP** de la empresa, siguiendo la plantilla arc42 y utilizando herramientas como PlantUML para los diagramas.
El objetivo es centralizar los procesos de negocio, especialmente el **Módulo de Compras**, y servir como guía para el desarrollo futuro.

---

## 📌 Contenido del repositorio

### Carpetas principales

- `docs/images/` → Contiene todas las imágenes de diagramas:
- `c1_context.png` → Diagrama de Contexto (Nivel 1)
- `c2_containers.png` → Diagrama de Contenedores (Nivel 2)
- `sequence_registrar_producto.png` → Diagrama de Secuencia (Registrar Producto)
- `mer_compras.png` → Diagrama MER de Compras

- `arc42-template/` → Plantilla arc42 con la documentación:
- `01_introduction_and_goals.md` → Objetivos y requisitos del sistema
- `02_architecture_constraints.md` → Restricciones y decisiones tecnológicas
- `03_system_scope_and_context.md` → Alcance y Diagrama de Contexto
- `05_building_block_view.md` → Diagrama de Contenedores y descripción de componentes
- `06_runtime_view.md` → Escenario crítico y Diagrama de Secuencia
- `07_deployment_view.md` → (Opcional) Vista de despliegue
- `10_glossary.md` → Glosario de términos clave del dominio

---

## 🖥 Diagramas y vistas del sistema

### Diagrama de Contexto (C1)

![Diagrama de Contexto](./docs/images/c1_context.png)
Muestra el sistema ERP como caja negra, sus usuarios (administradores y empleados) y sistemas externos (Contabilidad y EIS).

### Diagrama de Contenedores (C2)

![Diagrama de Contenedores](./docs/images/c2_containers.png)
Detalle de los componentes internos del ERP: SPA frontend, API monolítica y Base de Datos.

### Diagrama de Secuencia

![Diagrama de Secuencia](./docs/images/sequence_registrar_producto.png)
Flujo de la historia de usuario "Registrar Producto": interacción entre administrador, frontend, API y base de datos.

### Diagrama de Entidad-Relación (MER)

![Diagrama de Entidad-Relación](./docs/images/mer_compras.png)
Modelo de datos simplificado para el módulo de Compras: Producto, Proveedor y su relación.

---

## ⚙ Tecnologías y decisiones de arquitectura

- **Backend:** Java con Spring Boot
- **Base de datos:** PostgreSQL
- **Frontend:** SPA con React y JavaScript
- **Comunicación:** HTTPS/JSON entre frontend y API
- **Diagramas:** PlantUML

---

## 📝 Historias de usuario y gestión ágil

- Tablero Jira/Notion con todas las **épicas**, **historias de usuario**, **criterios de aceptación** y **priorización**:
[Jira - Tablero ERP](https://sb1858153.atlassian.net/jira/software/projects/ERP/boards/3?atlOrigin=eyJpIjoiZTdhYTg5NGEzZjE3NDNiYzhlMGVlMGVkZDkzYzIwM2QiLCJwIjoiaiJ9)

---

## 🗂 Glosario de términos

- **Producto:** Artículo que se compra y vende en la empresa
- **Proveedor:** Entidad que suministra productos
- **Orden de Compra:** Solicitud formal de adquisición de productos
- **Administrador de Compras:** Usuario que gestiona productos, proveedores y órdenes

---

## 📦 Cómo usar este repositorio

1. Revisar los diagramas en `docs/images/`.
2. Consultar la documentación técnica en `arc42-template/`.
3. Seguir la estructura y los diagramas como guía para implementar o expandir el sistema ERP.

---

### Autor: Grupo X
Fecha: 10/02/2026
