# 🚚📦 Análisis de la cadena de suministro para productos sanitarios

EDA, análisis de costos y aprendizaje automático

## 📌Descripción del proyecto

Este proyecto analiza datos históricos de envíos y precios de productos sanitarios (ARV, VIH y otros insumos médicos) dentro de una cadena de suministro internacional apoyada por organizaciones como PEPFAR y el Fondo Mundial.

El objetivo es comprender patrones de costos, volúmenes, logística y modos de envío, así como aplicar modelos de Machine Learning para:
- Predecir la cantidad de artículos enviados
- Clasificar el modo de envío más probable (Air, Ocean, Truck, etc.)

El análisis combina EDA, visualización, regresión, clasificación y optimización de modelos, generando insights accionables para mejorar decisiones logísticas y de planificación.

## 🎯Objetivos

- Analizar volúmenes y costos de envíos por país, proveedor y producto
- Identificar factores que impactan en:
- Cantidad enviada
- Valor del pedido
- Costos logísticos
- Evaluar la relación entre modo de envío y variables operativas
- Construir modelos predictivos para:
- Regresión: cantidad de artículos por envío
- Clasificación: tipo de transporte
- Comparar múltiples algoritmos de Machine Learning
- Optimizar modelos mediante selección de features e hiperparámetros

## 📂Conjunto de datos

Archivo principal

SCMS_Delivery_History_Dataset_20150929.csv

Información contenida
- País de destino
- Modo de envío
- Grupo y subclasificación del producto
- Marca y proveedor
- Dosis y forma farmacéutica
- Precios (unitario, por paquete)
- Cantidad enviada
- Costos de flete y seguros
- Fechas logísticas clave

## ⚠️Dataset real con valores faltantes y alta cardinalidad, tratado mediante limpieza y transformación.

## 🛠️Tecnologías utilizadas

- Python
- Pandas / NumPy – Manipulación de datos
- Matplotlib / Seaborn / Plotly – Visualización
- Statsmodels – Regresión OLS
- Scikit-learn – Modelos de ML
- XGBoost – Clasificación avanzada
- SciPy – Estadística
- Label Encoding / One-Hot Encoding
- StandardScaler

## 🔍Metodología

1️⃣ Limpieza y preprocesamiento

- Manejo de valores faltantes
- Normalización de nombres de columnas
- Codificación de variables categóricas
- Extracción de features temporales
- Eliminación de columnas de alta cardinalidad

2️⃣ Análisis Exploratorio (EDA)

- Estadísticas descriptivas
  
- Análisis por:
  -- País
  -- Marca
  -- Subclasificación
  -- Proveedor
  -- Modo de envío

- Visualizaciones:
  -- Barras
  -- Boxplots
  -- Pie charts
  -- Matrices de correlación

3️⃣ Análisis de correlación

- Identificación de variables clave asociadas a:
- Cantidad enviada
- Valor del pedido
- Costos logísticos

## 🤖Modelado Predictivo
🔹 Regresión – Cantidad de artículos

- Linear Regression (OLS)

- Evaluación:
  -- R²
  -- MAE
  -- MSE

- Análisis de significancia estadística (p-values)

- Identificación de multicolinealidad

🔹 Clasificación – Modo de envío

Modelos evaluados:

- Decision Tree
- Gaussian Naive Bayes
- Random Forest
- KNN
- XGBoost (mejor desempeño)

Evaluación:

- Accuracy
- Confusion Matrix
- Feature Importance
- Cross-validation

🔹 Optimización

- Selección de variables más importantes
- RandomizedSearchCV para hiperparámetros
- Comparación de modelos optimizados vs baseline

## 📊Resultados destacados

Variables como país, tipo de producto, proveedor y precios influyen fuertemente en:
- Cantidad enviada
- Modo de transporte
- XGBoost logra la mayor precisión en la clasificación del modo de envío
- Reducción de ruido mejora la capacidad predictiva
- El análisis permite identificar oportunidades de:
- Optimización logística
- Reducción de costos
- Mejora en planificación de inventarios


## 🚀Posibles mejoras futuras

- Modelos de optimización logística (ruteo, costos)
- Forecast de demanda
- Integración con datos geográficos
- Dashboards interactivos (Power BI / Streamlit)
- Explicabilidad de modelos (SHAP)

## ⚠️Disclaimer

Este proyecto tiene fines educativos y analíticos.
No representa conclusiones oficiales de ninguna organización.
