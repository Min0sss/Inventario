# Caso de Estudio: Control de Activos de TI e Infraestructura

Este repositorio contiene el diseño, la estructura de la base de datos relacional y el backend analítico utilizado para la gestión centralizada, monitoreo de ciclo de vida y auditoría de hardware crítico en una infraestructura corporativa.

## Enlace al Caso de Estudio Completo

El análisis profundo, las métricas de negocio analizadas y el dashboard interactivo final se encuentran documentados en Notion: [Ver Caso de Estudio Completo en Notion](https://vast-century-459.notion.site/Guillermo-Contreras-Portafolio-de-An-lisis-de-Datos-368b566267a4807ba2a8c4d0)

## Estructura del Proyecto

* `/sql/script_inventario.sql` : Script definitivo con la creación de tablas, restricciones de llaves foráneas y la carga masiva de los 50 activos operativos.

## Arquitectura de Datos

El proyecto implementa un **Modelo Estrella (Data Warehouse)** optimizado para analítica y Business Intelligence (OLAP), garantizando la integridad referencial mediante restricciones estrictas de llaves foráneas (`FOREIGN KEY`):

* **Tablas de Hechos:** `fact_inventario` (Centraliza costos en USD, fechas de inspección, llaves dimensionales y control de activos individuales mediante un identificador único `Asset_ID`).
* **Tablas de Dimensiones:** * `Dim_Hardware` (Catálogo de dispositivos: Laptops, Servidores, Switches, Firewalls, Access Points).
  * `Dim_Ubicaciones` (Mapeo físico e infraestructura: Sedes, Data Centers Principales/Redundantes y Áreas Operativas).
  * `Dim_Estados` (Ciclo de vida del activo: Excelente, Alerta, En Reparación, Obsoleto).
  * `Dim_Proveedores` (Entidades de adquisición y soporte).

## Dashboard de Inteligencia de Negocio (Power BI)

El entregable analítico final se compone de un tablero ejecutivo interactivo diseñado bajo estándares profesionales de UI/UX sobre un tapete oscuro de alta fidelidad, enfocado en resolver preguntas críticas de infraestructura:

1. **Monitoreo de Infraestructura Crítica:** Distribución exacta del volumen de activos desplegados por área de trabajo.
2. **Ciclo de Vida e Inspección:** Identificación automatizada de equipos obsoletos o que requieren atención/mantenimiento preventivo inmediato mediante tablas de auditoría temporal.
3. **Métricas Financieras Centralizadas:** KPIs de control de costo total invertido en infraestructura tecnológica (Suma total de inventario en USD).

---

Proyecto de práctica analítica - Mayo 2026.