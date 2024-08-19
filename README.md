# Proyecto de Inteligencia Artificial (IA)

Este repositorio contiene una serie de proyectos enfocados en la aplicación de diferentes técnicas de Inteligencia Artificial (IA) para la resolución de problemas relacionados con el análisis de imágenes médicas. Cada subcarpeta dentro del repositorio representa un proyecto específico, utilizando distintos enfoques de aprendizaje profundo.

## Estructura del Repositorio

### 1. **MLP (Perceptrón Multicapa)**

Este proyecto implementa un Perceptrón Multicapa (MLP) para la clasificación de imágenes médicas. El MLP es un tipo de red neuronal feedforward que se entrena utilizando backpropagation para ajustar sus pesos y realizar predicciones precisas. Es un enfoque básico en IA, utilizado aquí para comparar su rendimiento con técnicas más avanzadas.

- **Ubicación:** `./MLP`
- **Descripción:** Clasificación binaria de imágenes médicas utilizando un MLP.
- **Características:** Incluye la carga y preprocesamiento de datos, entrenamiento del modelo y evaluación de rendimiento.

### 2. **CNN (Redes Neuronales Convolucionales)**

Este proyecto utiliza Redes Neuronales Convolucionales (CNN) para la clasificación de imágenes de rayos X del tórax. Las CNN son especialmente efectivas en tareas de visión por computadora debido a su capacidad para captar características espaciales y patrones en imágenes.

- **Ubicación:** `./CNN`
- **Descripción:** Clasificación de imágenes de rayos X en categorías de neumonía y normalidad utilizando CNN.
- **Características:** Incluye la construcción de una CNN, preprocesamiento de imágenes, entrenamiento, y evaluación con métricas como precisión, recall y F1-score.

## Requisitos

- Python 3.x
- Bibliotecas necesarias para los proyectos incluyen:
  - `numpy`
  - `tensorflow`
  - `cv2`
  - `sklearn`
  - `matplotlib`
  
Cada subproyecto tiene un README individual con instrucciones detalladas sobre la instalación de dependencias, ejecución de scripts y análisis de resultados.

## Cómo Empezar

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/tu_usuario/IA-Proyecto.git
   cd IA-Proyecto
