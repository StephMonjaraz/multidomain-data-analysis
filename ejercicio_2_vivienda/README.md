# 🏠 Análisis de Condiciones de Vivienda en México (ENIGH 2022)

Este proyecto analiza datos de la Encuesta Nacional de Ingresos y Gastos de los Hogares (ENIGH 2022) del INEGI para identificar viviendas en situación de carencia habitacional con técnicas de clasificación.

## 📄 Descripción del Proyecto

Se pretende construir un modelo que, a partir de variables sobre la vivienda (material de construcción, servicios básicos, número de cuartos, etc.), prediga si una vivienda está en condiciones de carencia habitacional.

## 📊 Dataset

- Fuente: `viviendas.csv` (procesado desde la ENIGH 2022)
- Variables consideradas:
  - Material del techo, paredes y piso
  - Disponibilidad de agua y electricidad
  - Número de cuartos
  - Tipo de sanitario
  - Ubicación geográfica (urbana/rural)

- El dataset fue cargado usando `polars`, tratando valores nulos como `"&"`.

## 🧠 Modelos utilizados

- Árbol de Decisión
- Random Forest
- Regresión Logística

## 🔍 Análisis y Preprocesamiento

- Detección de valores nulos y tipos inconsistentes
- Selección de variables relevantes
- Codificación de variables categóricas
- División en conjunto de entrenamiento y prueba

## 🧪 Evaluación del Modelo

- Matriz de confusión
- ROC-AUC y curvas ROC
- Métricas de exactitud y F1-score

## ⚙️ Requisitos

- Python 3.8+
- Jupyter Notebook
- Bibliotecas: `polars`, `matplotlib`, `seaborn`, `scikit-learn`

## ▶️ Cómo ejecutar

1. Clona este repositorio o descarga el archivo notebook.
2. Asegúrate de tener el archivo `viviendas.csv` en la carpeta `datasets/`.
3. Abre `02_inegi_viviendas.ipynb` en Jupyter Notebook.
4. Ejecuta las celdas paso a paso.
