# Redes Neuronales II

Repositorio correspondiente al desarrollo de las prácticas de Redes Neuronales II, realizadas mediante Google Colab, Python, NumPy, TensorFlow/Keras y PyTorch

En el proyecto se aborda la implementación y entrenamiento de redes neuronales artificiales, iniciando con modelos desarrollados desde cero utilizando NumPy y posteriormente utilizando frameworks de Deep Learning


## Objetivo

Entender los fundamentos y el funcionamiento de las redes neuronales artificiales a través de la implementación de modelos para clasificación binaria, clasificación multiclase y reconocimiento de imágenes

Durante el desarrollo se aplican conceptos como:

-Forward Propagation: Lleva los datos de entrada hacia la salida para obtener una predicción
-Funciones de activación: Determinan cómo responde cada neurona
-Funciones de pérdida: Miden qué tan equivocada está la predicción
-Backpropagation: Calcula cómo corregir los errores de la red
-Actualización de pesos: Ajusta los pesos para mejorar las predicciones
-Descenso del gradiente: Busca reducir el error modificando los pesos
-Entrenamiento de redes neuronales: Repite estos procesos para que la red aprenda
-Evaluación mediante Accuracy: Mide el porcentaje de predicciones correctas
-Clasificación multiclase mediante Softmax: Calcula la probabilidad de cada clase y selecciona la más probable
-Reconocimiento de imágenes mediante MNIST: Entrena una red para identificar dígitos escritos a mano del 0 al 9

---

## Herramientas y tecnologías

- Python
- NumPy
- Matplotlib
- TensorFlow
- Keras
- PyTorch
- Google Colab
- GitHub

---

## Contenido del proyecto

### 01. Clasificación de frutas con NumPy

**Archivo:** `01_Frutas_NumPy.ipynb`

Implementación desde cero de una red neuronal para realizar clasificación binaria entre:

- Manzana
- Banano

En este notebook se trabajan:

- Preparación de datos.
- División de datos en entrenamiento y prueba.
- Normalización de características.
- Función de activación Sigmoid.
- Cálculo del error.
- Inicialización de pesos.
- Forward Propagation.
- Backpropagation.
- Entrenamiento.
- Predicciones.
- Evaluación mediante Accuracy.

---

### 02. Red neuronal multicapa con NumPy

**Archivo:** `02_Frutas_Multicapa_NumPy.ipynb`

Implementación desde cero de una red neuronal multicapa para clasificación binaria

La arquitectura utilizada es:

**3 → 4 → 1**

La red contiene:

- 3 características de entrada
- 4 neuronas en la capa oculta
- Función de activación ReLU
- 1 neurona de salida
- Función de activación Sigmoid
- Forward Propagation
- Backpropagation
- Actualización de pesos
- Entrenamiento mediante descenso del gradiente
- Evaluación mediante Accuracy

---

### 03. Clasificación de frutas con TensorFlow/Keras

**Archivo:** `03_Frutas_Keras.ipynb`

Implementación del problema de clasificación binaria utilizando TensorFlow y Keras.

Se utiliza una arquitectura:

**3 → 4 → 1**

En este notebook se aplican:

- Keras Sequential
- Capas Dense
- Función ReLU
- Función Sigmoid
- Optimizador Adam
- Binary Crossentropy
- Accuracy
- Entrenamiento mediante `fit()`
- Evaluación mediante `evaluate()`
- Predicción de nuevas muestras

---

### 04. Clasificación multiclase de frutas

**Archivo:** `04_Frutas_Multiclase_Keras.ipynb`

Se amplía el problema de clasificación para identificar tres tipos de frutas:

- Manzana
- Banano
- Naranja

Se utiliza una red neuronal con clasificación multiclase y función de activación Softmax

También se utilizan:

- TensorFlow/Keras
- Capas Dense
- `sparse_categorical_crossentropy`
- Accuracy
- Predicciones
- `argmax()` para determinar la clase correspondiente

---

### 05. Reconocimiento de dígitos con MNIST y Keras

**Archivo:** `05_MNIST_Keras.ipynb`

Implementación de una red neuronal para reconocer dígitos escritos a mano utilizando el conjunto de datos MNIST

La arquitectura utilizada es:

**784 → 128 → 10**

En este notebook se trabajan:

- Imágenes de 28 × 28 píxeles
- Normalización de imágenes
- Flatten
- Capa Dense con ReLU
- Capa de salida con Softmax
- Entrenamiento
- Validación
- Loss
- Accuracy
- Predicciones
- Identificación de errores de clasificación

---

### 06. Reconocimiento de dígitos con MNIST y PyTorch

**Archivo:** `06_MNIST_PyTorch.ipynb`

Implementación del reconocimiento de dígitos MNIST utilizando PyTorch

La arquitectura utilizada es:

**784 → 128 → 10**

Durante el desarrollo se utilizan:

- PyTorch
- `torch.nn`
- `torch.optim`
- `torchvision`
- `DataLoader`
- ReLU
- `CrossEntropyLoss`
- Optimizador Adam
- Backpropagation
- Evaluación sobre datos de prueba
- Predicción de imágenes individuales

---

## Progresión del proyecto

El proyecto sigue una progresión desde la implementación manual de una red neuronal hasta la utilización de frameworks especializados:

```text
                 REDES NEURONALES II
                         │
                         ▼
              Clasificación de frutas
                         │
                         ▼
             Implementación con NumPy
                         │
                         ▼
              Red neuronal multicapa
                         │
                         ▼
                 TensorFlow / Keras
                         │
                         ▼
              Clasificación multiclase
                         │
                         ▼
                    Dataset MNIST
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
         MNIST + Keras         MNIST + PyTorch
```

---

## Evaluación de los modelos

Durante las diferentes prácticas se utilizaron diferentes elementos para analizar el comportamiento de las redes neuronales:

- Evolución del error durante el entrenamiento
- Accuracy sobre datos de prueba
- Probabilidades de clasificación
- Predicciones de nuevas muestras
- Curvas de pérdida
- Curvas de Accuracy
- Identificación de ejemplos correctamente clasificados
- Identificación de errores de clasificación

Los resultados completos de cada práctica pueden consultarse directamente en los notebooks correspondientes

---

## Aprendizajes

El desarrollo de estas prácticas permitió comprender progresivamente el funcionamiento de las redes neuronales artificiales

La implementación con NumPy permitió observar directamente procesos como el cálculo de las activaciones, la propagación hacia adelante, el cálculo del error, la retropropagación y la actualización de los pesos

Posteriormente, mediante TensorFlow/Keras y PyTorch, fue posible implementar modelos utilizando herramientas especializadas de Deep Learning

También se trabajaron diferentes funciones de activación, como Sigmoid, ReLU y Softmax, además de problemas de clasificación binaria y multiclase

---

## Conclusión

El proyecto permitió reforzar los conocimientos sobre redes neuronales artificiales, mediante la combinación de implementaciones desde cero y el uso de frameworks de Deep Learning

La utilización de NumPy permitió entender los procesos internos de una red neuronal, mientras que TensorFlow/Keras y PyTorch facilitaron la creación, entrenamiento y evaluación de los modelos

El avance desde la clasificación de frutas hasta el reconocimiento de dígitos con MNIST permitió aplicar los conocimientos adquiridos en diversos problemas de clasificación

---

##  Estructura del repositorio

```text
Redes-Neuronales-II/
│
├── 01_Frutas_NumPy.ipynb
├── 02_Frutas_Multicapa_NumPy.ipynb
├── 03_Frutas_Keras.ipynb
├── 04_Frutas_Multiclase_Keras.ipynb
├── 05_MNIST_Keras.ipynb
├── 06_MNIST_PyTorch.ipynb
└── README.md
```

---

**Herramientas principales:** Google Colab - Python - NumPy - TensorFlow/Keras - PyTorch - GitHub
