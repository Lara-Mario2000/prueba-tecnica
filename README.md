# Prueba Tecnica

El objetivo de esta prueba es evaluar tu capacidad para procesar datos con Python y transformarlos en un tablero de control estratégico. Buscamos ver cómo integras lógica de negocio avanzada en un entorno visual.

**Tiempo máximo:** 60 - 90 minutos.  

## Preparación: Obtención de Datos
Para comenzar la prueba, puedes obtener el dataset de cualquiera de las siguientes formas:

1. **Desde este Repositorio:** Descarga el archivo `supermarket_sales.csv` que se encuentra en la carpeta raíz.
2. **Desde la Fuente Original:** Si prefieres la fuente oficial, descárgalo en [Kaggle - Supermarket Sales](https://www.kaggle.com/datasets/faresashraf1001/supermarket-sales).

*Utiliza este archivo como base para tu script de Python.*

---

## 1. Lógica de Negocio (Python)
Tu tarea principal es ejecutar una segmentación avanzada para identificar el Top Performers del catálogo, utilizando el Percentil 75 como umbral de éxito en rentabilidad y satisfacción.

**Tareas en Python:**
* **Identificar Umbrales:** Calcula el percentil 75 de la columna `gross income` y de la columna `Rating`.
* **Crear Columna `Product_Tier`:** Clasifica cada transacción bajo la siguiente lógica:
    * **Star:** Si el Profit Y el Rating están en el Top 25%.
    * **Cash Cow:** Si el Profit está en el Top 25%, pero el Rating NO.
    * **Hidden Gem:** Si el Rating está en el Top 25%, pero el Profit NO.
    * **Standard:** Todo lo que no entre en las categorías anteriores.
* **Exportación:** Genera el `.csv` final para tu dashboard.

---

## 2. Dashboard (Power BI / Looker)
Diseña un reporte de **una sola página** que sea creativo y funcional. El diseño es libre, pero debe responder a lo siguiente:

1.  **Ventas y Tendencias:** Una línea de tiempo que permita filtrar por la nueva categoría `Product_Tier`.
2.  **Análisis de Segmentos:** Un gráfico (ej. Treemap o Donut) que muestre qué porcentaje del total de ventas representa cada "Tier" de producto.
3.  **Matriz de Rendimiento:** Un gráfico de dispersión (Scatter Plot) de Profit vs Rating, donde los puntos estén coloreados por tu segmentación de Python.

**✨ Libertad Creativa:**
Tienes total libertad para agregar KPIs adicionales (Ticket promedio, Rating por ciudad, etc.) y personalizar el estilo visual (Dark mode, branding, etc.). Valoramos que el dashboard sea "limpio" y fácil de interpretar para un gerente.

---

## Entregables
1.  Script de Python (`.py` o `.ipynb`).
2.  Archivo del dashboard (`.pbix` o link de Looker).

---

## ¿Qué evaluaremos?
* **Integración:** El uso real de la segmentación calculada en Python.
* **Visualización:** Claridad, uso de colores y capacidad de síntesis visual.
* **Pensamiento Crítico:** Tu capacidad para ir más allá de los datos y proponer una acción de negocio.

¡Mucho éxito! 📈
