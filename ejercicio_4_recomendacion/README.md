# 🎬 Sistema de Recomendación de Películas (MovieLens)

Este proyecto implementa un sistema de recomendación de películas utilizando el dataset MovieLens. El enfoque se basa en la similitud entre usuarios o entre ítems (películas), usando técnicas de filtrado colaborativo.

## 📄 Descripción

Se construye un sistema capaz de recomendar películas que probablemente le gusten a un usuario, en función de las calificaciones que han dado otros usuarios similares.

## 📊 Dataset

- Fuente: [MovieLens](https://grouplens.org/datasets/movielens/)
- Contiene: ID de usuario, ID de película, calificación y timestamp.
- Tamaños típicos: `ml-latest-small`, `ml-1m`, etc.

## 🧠 Modelo utilizado

- K-Nearest Neighbors (KNN) con filtrado colaborativo basado en:
  - Similitud entre usuarios (User-based)
  - Similitud entre películas (Item-based)
- Métricas de similitud: Coseno o correlación de Pearson

## 🔍 Procesamiento y análisis

- Creación de matrices usuario–película
- Rellenado de valores nulos
- Cálculo de similitud
- Generación de recomendaciones personalizadas

## 🧪 Evaluación

- Recomendaciones verificadas manualmente
- Visualización de resultados
- (Opcional) Métricas de ranking como Precision@k

## 🌐 Interfaz (opcional)

- Puede implementarse una app web con **Streamlit** para permitir al usuario elegir películas y obtener recomendaciones.

## ⚙️ Requisitos

- Python 3.8+
- Jupyter Notebook
- Bibliotecas: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, (opcional: `streamlit`)

## ▶️ Cómo ejecutar

1. Asegúrate de tener el dataset MovieLens descargado (`ratings.csv`, `movies.csv`, etc.).
2. Abre el archivo `.ipynb` en Jupyter Notebook.
3. Ejecuta todas las celdas para visualizar el sistema en acción.
4. Para lanzar la app Streamlit (opcional):
   ```bash
   streamlit run app.py
