# 🍃 NutriTrace - Sistema de Trazabilidad e Higiene Alimentaria

![Estado](https://img.shields.io/badge/Estado-POC_Enterprise_V5-success)
![Tecnología](https://img.shields.io/badge/Tecnolog%C3%ADa-HTML5_%7C_Tailwind_CSS_%7C_Vanilla_JS-blue)
![Despliegue](https://img.shields.io/badge/Despliegue-GitHub_Pages-black)

## 🚀 Demo en Vivo

Puedes probar la versión funcional e interactiva del prototipo directamente desde tu navegador, sin necesidad de instalaciones:

👉 **[Probar NutriTrace (GitHub Pages)](https://sabarettagh.github.io/poc_v1_r/poc_v1.html)**

---

## 📖 Acerca del Proyecto

**NutriTrace** es una Prueba de Concepto (POC) de alta fidelidad diseñada para la gestión, seguridad e higiene en la industria manufacturera de alimentos.

El sistema garantiza una **trazabilidad completa** (hacia atrás, interna y hacia adelante) cumpliendo con los estándares de control sanitario, permitiendo auditar qué lote de materia prima se utilizó en cada producto final y a qué cliente fue despachado.

**Diseñado con un enfoque en la reducción de riesgos, el orden y el control.**

### 🌟 Valor Agregado (Control Sanitario)

- **Trazabilidad 360º (Módulo Estrella):** Visualización en forma de árbol que permite rastrear, con un solo clic, el origen exacto (proveedor/remito) de los insumos de un lote y su destino final (clientes/despachos).
- **Simulación de Alertas Sanitarias:** Capacidad de simular un "Recall" (bloqueo de materia prima) e identificar inmediatamente qué lotes de producción y clientes se encuentran en riesgo.
- **KPIs Estratégicos:** El dashboard muestra indicadores críticos para la gestión: _% de Lotes Conformes_, _Materias Primas Rechazadas_, _Lotes Anulados_ y _Recepciones Mensuales_.

### 🏭 Módulos Operativos (Transaccionales)

- **📦 Recepciones:** Registro de ingresos con validación de estado (Aceptado/Rechazado) y detalle preciso de lotes recibidos.
- **blender Lotes de Producción:** Generación de lotes consumiendo el stock físico disponible mediante Listas de Materiales (BOM).
- **🚚 Despachos:** Salida de mercadería vinculando los lotes terminados con los clientes y el transporte.
- _(Nota UX)_: Implementación del patrón **Maestro-Detalle** con modales de lectura limpios ("Ver Detalles") para evitar la sobrecarga visual en las tablas principales.

### 📇 Módulos de Administración (Catálogos)

- **Productos:** Catálogo con control de temperatura objetiva, vida útil y categorización.
- **Materias Primas:** Diccionario de insumos clasificados por tipo y categoría, vinculados a su proveedor de origen.
- **Proveedores y Clientes:** Directorios completos con validación de CUIT, rubros y zonas logísticas.

---

## ⚙️ Características Técnicas del Prototipo

Este POC fue construido priorizando la velocidad de validación visual y funcional, simulando el comportamiento de un ERP robusto.

- **Sincronización con Base de Datos:** Los formularios y tablas reflejan fielmente el esquema relacional (`v1_initial_schema.sql`).
- **Frontend Responsivo (Mobile-Ready):** Interfaz fluida con Menú Lateral "Off-Canvas" (Hamburguesa) ideal para tablets y móviles en planta.
- **Filtros Inteligentes y Selectores:** Búsqueda avanzada por módulo y selectores dinámicos para evitar errores de tipeo en rubros y categorías.
- **Auditoría Silenciosa:** Registro simulado de creación y modificación de datos para transmitir seguridad y trazabilidad en las operaciones.
- **Cero Dependencias Backend:** Motor en memoria (Vanilla JS) y Tailwind CSS vía CDN. No requiere servidores para su ejecución.

---

## 🗺️ Roadmap y Módulos Sugeridos

La arquitectura final del producto contemplará:

- **Backend:** Spring Boot 3.5 (Java 17+), Spring Data JPA, MySQL/PostgreSQL.
- **Frontend:** Angular 19/20 usando Standalone Components.

**Módulos Sugeridos (Próximamente):**

- 📐Trazabilidad 360°.
- 📄 Generación de Reportes.
- 🕵️ Auditoría de Eventos (Logs del sistema).
