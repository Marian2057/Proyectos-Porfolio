# Sustainable Growth Monitor 📊🌱
**Proyecto de Simulación Laboral - No Country (2025)**

## 📋 Descripción del Proyecto
El **Sustainable Growth Monitor** es un sistema de Inteligencia de Negocios (BI) diseñado para que las PyMEs puedan monitorear su desempeño de manera integral. El objetivo principal es romper con los silos de información financiera, operativa y de recursos humanos, integrando indicadores **ESG** (Ambientales, Sociales y de Gobernanza) para demostrar que la sostenibilidad es una palanca de rentabilidad.

## 🚀 Propuesta de Valor
El sistema permite responder preguntas críticas de negocio mediante la correlación de datos:
* **Eficiencia vs. Rentabilidad:** ¿Cómo impacta el consumo energético en el margen neto?
* **Capital Humano:** ¿Qué relación existe entre la satisfacción del empleado y los costos de rotación?

## 🛠️ Arquitectura y Stack Tecnológico
El proyecto utiliza un modelo de datos consolidado (Star Schema) organizado de la siguiente manera:
* **Base de Datos:** Supabase (Carga y validación técnica).
* **Modelo de Datos:**
    * `dim_tiempo`: Dimensión temporal centralizada.
    * **Tablas de Hechos:** `fact_finanzas`, `fact_ambiental`, `fact_rrhh` y `fact_gobernanza_trimestral`.
    * `objetivos_esg`: Tabla de catálogo para seguimiento de metas.

## 📈 Indicadores Clave (KPIs)

| Categoría | KPIs Principales | Propósito |
| :--- | :--- | :--- |
| **Finanzas** | Margen Neto, Ingresos Totales | Medir salud económica y rentabilidad. |
| **Ambiental (E)** | Huella de Carbono, Tasa de Reciclaje | Monitorear impacto ecológico y eficiencia. |
| **Social (S)** | Satisfacción de Empleados, Tasa de Rotación | Evaluar el bienestar del capital humano. |
| **Gobernanza (G)** | Diversidad en Liderazgo, Cumplimiento Ético | Asegurar transparencia y equidad. |

## 🖥️ Visualización (Dashboard)
El dashboard se estructura en tres vistas principales:
1. **Resumen Ejecutivo:** Vista macro de los indicadores de alto nivel.
2. **Análisis Financiero:** Detalle profundo de ingresos, costos y márgenes.
3. **Impacto ESG:** Visualización del desempeño en sostenibilidad y cumplimiento de metas.

## 💡 Hallazgos y Recomendaciones
Tras el análisis de los datos, se proponen las siguientes acciones:
* **Prioridad 1:** Desacople Energético (Inversión en maquinaria eficiente para romper la dependencia entre producción y alto consumo).
* **Prioridad 2:** Flexibilización de costos fijos ante la estacionalidad de la demanda.
* **Prioridad 3:** Capitalización de la marca empleadora basada en los altos índices de satisfacción (7.5
