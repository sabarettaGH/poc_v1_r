# 🍃 NutriTrace - Sistema de Trazabilidad e Higiene Alimentaria

![Estado](https://img.shields.io/badge/Estado-POC_Funcional-success)
![Tecnología](https://img.shields.io/badge/Tecnolog%C3%ADa-HTML5_%7C_Tailwind_CSS_%7C_Vanilla_JS-blue)
![Despliegue](https://img.shields.io/badge/Despliegue-GitHub_Pages-black)

## 🚀 Demo en Vivo

Puedes probar la versión funcional e interactiva del prototipo directamente desde tu navegador, sin necesidad de instalaciones:

👉 **[Probar NutriTrace (GitHub Pages)](pocv3_r.html)**

---

## 📖 Acerca del Proyecto

**NutriTrace** es una Prueba de Concepto (POC) de alta fidelidad diseñada para la gestión, seguridad e higiene en la industria manufacturera de alimentos.

El sistema garantiza una **trazabilidad completa** (hacia atrás, interna y hacia adelante) cumpliendo con los estándares de control sanitario, permitiendo auditar qué lote de materia prima se utilizó en cada producto final y a qué cliente fue despachado.

### 🏭 Módulos Principales

- **📊 Dashboard Operativo:** KPIs en tiempo real (Lotes producidos, recepciones, insumos físicos).
- **📦 Recepción (Inventario Físico):** Registro de ingresos de proveedores con validación de remitos, lotes de origen y fechas de vencimiento.
- **blender Elaboración (Producción):** Generación de Lotes de Producción consumiendo dinámicamente el stock físico de materias primas disponible (Lista de Materiales).
- **🚚 Despachos (Logística):** Salida de mercadería vinculando los lotes de producción terminados con los clientes de destino.
- **📇 Administración (Master Data):** Catálogos y directorios de Productos, Materias Primas, Proveedores y Clientes.

---

## ⚙️ Características Técnicas del Prototipo

Este POC fue construido priorizando la velocidad de validación visual y funcional (Nivel 3).

- **Frontend Responsivo:** Diseñado con el enfoque _Mobile-First_. Incluye menú "Off-Canvas" (Hamburguesa) para uso en tablets o celulares por parte de operarios de planta.
- **Motor Dinámico (Vanilla JS):** Base de datos en memoria y generación automática de vistas y formularios (CRUD).
- **Filtros Avanzados:** Buscadores dinámicos por módulo y sincronización de datos relacionales (ej. Proveedor -> Oferta de Insumos).
- **Cero Dependencias:** Utiliza Tailwind CSS vía CDN. No requiere Node.js, Webpack ni configuración de servidores para ejecutarse.

---
