# 📊 Modernización Analítica y Modelo Predictivo del Flujo Turístico en Ecuador (2021–2025)

Pipeline automatizado end-to-end en **Python** para la ingesta, procesamiento, visualización interactiva y predicción del flujo migratorio de extranjeros hacia Ecuador, utilizando datos oficiales del **INEC** y el **Ministerio de Turismo (MINTUR)**[cite: 6].

---

## ⚡ Lo más destacado del proyecto

* **Optimizaciones ETL:** Procesamiento de más de **5.88 millones de registros**[cite: 7, 16]. Conversión a formato columnar **Parquet**, reduciendo el consumo de RAM en un **85%** y bajando la carga a menos de **2 segundos**[cite: 7, 14].
* **Visualizaciones dinámicas:** Tableros interactivos desarrollados con **Plotly** que incluyen menús desplegables por año y análisis de estacionalidad[cite: 8, 14, 16].
* **Machine Learning:** Modelo **Random Forest Regressor** con `Scikit-learn` para predecir entradas mensuales de turistas por vía de ingreso y país emisor[cite: 8, 12, 16].
  * **$R^2$:** `96.67%` (varianza explicada)[cite: 7, 12]
  * **MAE:** `~547.52` visitantes/mes[cite: 8, 12]
* **Reportabilidad automática:** Exportación automatizada a un libro de Excel multi-pestaña (8 preguntas de negocio) y CSV consolidado[cite: 7, 8, 14].

---

## 🛠️ Tecnologías utilizadas

* **Lenguaje:** Python 3.x[cite: 7, 16]
* **Procesamiento:** `pandas`, `numpy`, `pyarrow` (Parquet)[cite: 7, 14, 16]
* **Machine Learning:** `scikit-learn` (Random Forest, Train/Test Split, Metrics)[cite: 8, 12, 16]
* **Visualización:** `plotly.express`, `plotly.graph_objects`
* **Exportación de reportes:** `openpyxl`[cite: 8, 14]

---

## 📂 Estructura del repositorio

```text
├── graficos/                 # Capturas PNG de las visualizaciones
├── salida_resultados/        # Reporte Excel multi-hoja y CSV consolidado
├── MINTUR_Analytics.ipynb    # Notebook principal con la solución en Python
├── MINTUR_Analytics.pdf      # Informe ejecutivo final del proyecto
└── README.md                 # Documentación principal del repositorio
