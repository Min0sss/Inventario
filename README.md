# Caso de Estudio: Control de Activos de TI e Infraestructura

Este repositorio contiene el diseño y la estructura de la base de datos relacional utilizada para la gestión, monitoreo de ciclo de vida y auditoría de hardware en la infraestructura corporativa.

## Enlace al Caso de Estudio Completo

El análisis profundo, las métricas de negocio analizadas y el dashboard interactivo final se encuentran documentados en Notion: [Ver Caso de Estudio Completo en Notion](https://vast-century-459.notion.site/Guillermo-Contreras-Portafolio-de-An-lisis-de-Datos-368b566267a4807ba2a8c4d0e07c6bdf)

## Estructura del Proyecto

* `script_inventario.sql` : Script definitivo con la creación del esquema de base de datos en SQL Server (Tablas de Hechos y Dimensiones) y la carga masiva de datos.

## Arquitectura de Datos

El proyecto implementa un **Modelo Estrella (Data Warehouse)** optimizado para analítica y Business Intelligence:

* **Tablas de Hechos:** `fact_inventario`.
* **Tablas de Dimensiones:** `Dim_Hardware`, `Dim_Ubicaciones`, `Dim_Estados`, `Dim_Proveedores`.

---

Proyecto de práctica analítica - Mayo 2026.