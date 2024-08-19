# Clustering de Imágenes - K-Means

Este proyecto aplica el algoritmo de clustering **K-Means** a una imagen para agrupar los píxeles según sus valores de color. El enfoque principal es el análisis y visualización de la imagen en el espacio de color RGB y cómo estos grupos de colores pueden ser identificados y diferenciados.

## Descripción del Proyecto

En este proyecto se trabaja con una imagen cargada desde Google Drive, la cual se procesa para extraer y analizar la información de color en cada píxel. El objetivo es agrupar los píxeles de la imagen en diferentes clusters utilizando **K-Means**, un algoritmo de clustering popular en aprendizaje automático.

## Contenido

- **Visualización de la Imagen y Canales de Color:**
  - Se muestran la imagen original y sus canales de color (Rojo, Verde y Azul) por separado para una mejor comprensión de la distribución de los colores.

- **Representación en 3D del Espacio de Color RGB:**
  - Se representa en un gráfico 3D la distribución de los píxeles de la imagen en el espacio de color RGB, incluyendo referencias para el negro y el blanco ideales.

- **Clustering con K-Means:**
  - Se ejecuta el algoritmo K-Means para agrupar los píxeles en distintos clusters. Además, se evalúan las inercias (suma de distancias al cuadrado) para diferentes números de clusters, ayudando a identificar el número óptimo de grupos.

- **Visualización de Clusters:**
  - Se añade una columna al DataFrame que contiene los datos de los píxeles, indicando a qué cluster pertenece cada píxel.

## Requisitos

- **Python 3.x**
- **Bibliotecas:**
  - `opencv-python`
  - `matplotlib`
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `ipywidgets`

Puedes instalar las dependencias necesarias ejecutando:

```bash
pip install opencv-python matplotlib numpy pandas scikit-learn ipywidgets
