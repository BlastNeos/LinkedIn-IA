# Clasificación de Neumonía con Redes Neuronales Convolucionales (CNN)

Este proyecto implementa una Red Neuronal Convolucional (CNN) para la clasificación de imágenes de rayos X de tórax, diferenciando entre imágenes normales y aquellas que presentan neumonía. El objetivo es aplicar técnicas de aprendizaje profundo para procesar y analizar las imágenes, asignando la clase correspondiente a cada una.

## Estructura del Proyecto

### 1. Carga y Exploración de Datos

Se define la estructura de carpetas para los conjuntos de datos:

- **Entrenamiento:**
  - `PNEUMONIA`: Imágenes con diagnóstico de neumonía.
  - `NORMAL`: Imágenes normales.

- **Prueba:**
  - `PNEUMONIA`: Imágenes con diagnóstico de neumonía.
  - `NORMAL`: Imágenes normales.

- **Validación:**
  - `PNEUMONIA`: Imágenes con diagnóstico de neumonía.
  - `NORMAL`: Imágenes normales.

### 2. Preprocesamiento de Imágenes

Las imágenes se cargan y preprocesan antes de ser utilizadas en la CNN:

- **Asignación de etiquetas:** Las imágenes se etiquetan como `0` para normales y `1` para neumonía.
- **Redimensionamiento:** Las imágenes se redimensionan a `224x224` píxeles.
- **Normalización:** Las imágenes se normalizan dividiendo los valores de píxel por `255`.

### 3. Arquitectura del Modelo

La CNN se construye con las siguientes capas:

- **Capas Convolucionales:** Tres capas convolucionales con filtros de tamaño `3x3` y activación `ReLU`.
- **MaxPooling:** Capas de MaxPooling para reducir la dimensionalidad espacial de las imágenes.
- **Dropout:** Una capa de Dropout con una tasa del `50%` para prevenir el sobreajuste.
- **Capa Densa:** Una capa densa con `256` neuronas y activación `ReLU`.
- **Capa de Salida:** Una capa de salida con una única neurona y activación `sigmoide` para la clasificación binaria.

### 4. Entrenamiento del Modelo

El modelo se entrena utilizando los datos preprocesados. El entrenamiento se realiza durante `10` épocas, y se valida con el conjunto de validación.

### 5. Evaluación del Modelo

Se utiliza una matriz de confusión y métricas de rendimiento (Precisión, Recall, F1-score) para evaluar la efectividad del modelo en el conjunto de prueba.

## Requisitos

- Python 3.x
- Bibliotecas necesarias: `numpy`, `cv2`, `tensorflow`, `sklearn`, `os`, `matplotlib`

## Instrucciones

1. **Cargar los datos:**
   - Colocar las imágenes en las carpetas correspondientes según la estructura mencionada.

2. **Ejecutar el script:**
   - Preprocesar las imágenes.
   - Entrenar la CNN.
   - Evaluar el rendimiento en el conjunto de prueba.

3. **Interpretar los resultados:**
   - Revisar la matriz de confusión y las métricas de rendimiento para analizar la precisión del modelo.

## Resultados

Los resultados del modelo, incluyendo la matriz de confusión y las métricas de rendimiento (Precisión, Recall, F1-score), se mostrarán al finalizar el entrenamiento y evaluación.

---

Este README ofrece una guía básica para entender y ejecutar el proyecto de clasificación de neumonía utilizando CNN. Asegúrate de revisar el código fuente para detalles específicos y personalizaciones adicionales.
