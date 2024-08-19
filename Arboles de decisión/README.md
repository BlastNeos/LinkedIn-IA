# Árboles de Decisión - Modelo Iris

Este proyecto implementa un modelo de Árbol de Decisión utilizando el famoso conjunto de datos **Iris**. Se incluyen visualizaciones y métricas de rendimiento para evaluar la eficacia del modelo.

## Descripción del Conjunto de Datos

El conjunto de datos **Iris** contiene 150 observaciones de iris de tres especies diferentes: *Iris setosa*, *Iris versicolor* y *Iris virginica*. Cada observación tiene cuatro características:
- **longitud del sépalo** (cm)
- **ancho del sépalo** (cm)
- **longitud del pétalo** (cm)
- **ancho del pétalo** (cm)

Además, incluye una columna de "target" que indica la especie correspondiente.

## Contenido

- **Visualización de Datos:**
  - Se genera un DataFrame que organiza y muestra las características de cada observación.
  - Se utiliza un gráfico de coordenadas paralelas para visualizar las características de las observaciones hasta un índice seleccionado por el usuario.

- **Entrenamiento del Modelo:**
  - El modelo de Árbol de Decisión se entrena utilizando el criterio de `entropy`.
  - El conjunto de datos se divide en entrenamiento y prueba para evaluar el rendimiento del modelo.

- **Evaluación del Modelo:**
  - Se calcula la precisión (`accuracy`) y la precisión de clasificación (`precision`) para evaluar la calidad del modelo.
  - Se grafica el árbol de decisión entrenado para una mejor interpretación visual.

## Requisitos

- **Python 3.x**
- **Bibliotecas:**
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`

Puedes instalar las dependencias necesarias ejecutando:

```bash
pip install pandas numpy scikit-learn matplotlib
