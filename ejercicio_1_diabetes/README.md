# 🩺 Predicción de Riesgo de Diabetes

Este proyecto realiza un análisis y modelado para predecir el riesgo de diabetes en pacientes femeninas a partir de registros médicos. Se sigue un enfoque completo que incluye exploración de datos, limpieza, análisis visual y entrenamiento de modelos de clasificación.

## 📄 Descripción del Proyecto

El objetivo es predecir si un paciente tiene diabetes utilizando variables clínicas como presión arterial, glucosa, número de embarazos, etc. Se evaluaron distintos modelos de clasificación y se visualizaron resultados clave para interpretar el comportamiento de los datos.

## 📊 Dataset

- Fuente: `diabetes.csv`
- Atributos: número de embarazos, nivel de glucosa, presión arterial, espesor de piel, insulina, BMI, edad, etc.
- El dataset fue cargado y manipulado usando `polars`.

## 🧠 Modelos utilizados

- Regresión Logística
- K-Nearest Neighbors (KNN)
- Random Forest

## 🔍 Análisis y Preprocesamiento

- Se revisaron valores atípicos y nulos.
- Se identificaron columnas con valores 0 no plausibles (por ejemplo, presión arterial).
- Visualizaciones con `seaborn` y `matplotlib`.
- Balanceo de clases y normalización de variables numéricas.

## 🧪 Evaluación del Modelo

- Matriz de confusión
- ROC-AUC
- Métricas de precisión, recall y F1-score

## ⚙️ Requisitos

- Python 3.8+
- Jupyter Notebook
- Bibliotecas: `polars`, `matplotlib`, `seaborn`, `scikit-learn`

## ▶️ Cómo ejecutar

1. Clona este repositorio o descarga el archivo notebook.
2. Asegúrate de tener el archivo `diabetes.csv` en la carpeta `datasets/`.
3. Abre `01_diabetes_prediction.ipynb` en Jupyter Notebook.
4. Ejecuta las celdas paso a paso.
