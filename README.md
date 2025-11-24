# Ecommerce A/B Testing

Este proyecto analiza los resultados de un experimento A/B realizado por una tienda online con el objetivo de evaluar si una modificación en el proceso de compra mejora la conversión y el comportamiento de los usuarios. El análisis incluye limpieza de datos, verificación de sesgos, validación experimental y pruebas estadísticas para determinar la significancia de los resultados.

## 📌 Objetivo
- Evaluar el impacto de un cambio en el embudo de compra.
- Comparar los resultados de los grupos A y B.
- Identificar cualquier sesgo o contaminación entre grupos.
- Analizar eventos del funnel: **product_page → product_cart → purchase**.
- Realizar pruebas de hipótesis para validar diferencias estadísticas.

## 🧹 Preparación y Limpieza de Datos
El proceso incluyó:
- Conversión y estandarización de fechas.
- Unificación del formato de eventos y categorías.
- Detección y eliminación de usuarios que aparecen en ambos grupos (contaminación del experimento).
- Revisión de eventos fuera del periodo del experimento.
- Validación de la estructura del dataset para asegurar un análisis confiable.

## 📊 Análisis Realizado
- Exploración general de los eventos de cada usuario.
- Comparación de tamaños de los grupos A y B.
- Análisis del número de eventos por etapa del funnel.
- Construcción del embudo para evaluar caídas y conversiones.
- Comparación directa entre grupos del embudo completo.
- Pruebas estadísticas (p-value, z-test) para determinar diferencias.

## 📈 Resultados Principales
- Se identificó contaminación entre grupos iniciales (usuarios presentes en A y B), la cual fue corregida.
- Los grupos muestran diferencias en la cantidad de eventos, pero no todas son estadísticamente significativas.
- El análisis indica si el cambio propuesto mejora o no la conversión final.
- La prueba estadística final permite concluir con evidencia si la variante supera al control.

## 🛠 Tecnologías Utilizadas
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Statsmodels / Scipy (para pruebas de hipótesis)**
- **Jupyter Notebook**

## 📁 Archivos del Proyecto
- `ecommerce-ab-testing.ipynb` — Notebook principal con todo el análisis.
- Datos originales del experimento (visitas, eventos, grupos).
