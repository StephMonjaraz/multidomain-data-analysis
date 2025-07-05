# 🚰 Predicción de Consumo Excesivo de Agua en la CDMX

Este proyecto utiliza datos públicos de consumo de agua en la Ciudad de México para predecir si una **manzana** (unidad geográfica censal) tendrá un consumo excesivo en un próximo periodo bimestral.

## 📄 Descripción

El modelo de clasificación toma en cuenta características como volumen de consumo, uso del inmueble, ubicación por alcaldía y otros factores relevantes, con el fin de anticipar patrones de alto consumo.

## 📊 Dataset

- Fuente: Portal de Datos Abiertos de la CDMX
- Nivel de agregación: Manzana censal
- Variables posibles:
  - Volumen de agua bimestral
  - Alcaldía
  - Tipo de uso (habitacional, mixto, industrial)
  - Densidad poblacional, estrato, etc.

## 🧠 Modelos utilizados

- Árbol de decisión
- Random Forest
- Regresión logística

## 🔍 Procesamiento y análisis

- Limpieza de datos nulos y errores de formato
- Ingeniería de características para marcar umbrales de consumo excesivo
- Codificación de variables categóricas
- División de datos en conjuntos de entrenamiento y prueba

## 🧪 Evaluación

- Matriz de confusión
- Precisión, recall y F1-score
- Curva ROC y AUC

## ⚙️ Requisitos

- Python 3.8+
- Jupyter Notebook
- Bibliotecas: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, (opcional: `geopandas`)

## ▶️ Cómo ejecutar

1. Coloca el archivo de datos en la carpeta del notebook.
2. Abre el archivo `.ipynb` con Jupyter Notebook.
3. Ejecuta las celdas paso a paso.
