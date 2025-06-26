

# Análisis de Sentimiento con una Red LSTM usando Keras

Este repositorio contiene un cuaderno de Jupyter (`013_Análisis_de_Sentimiento_con_una_Red_LSTM_usando_Keras.ipynb`) que te guiará en la construcción de un modelo de **red neuronal recurrente (RNN)**, específicamente una **LSTM**, utilizando la API Keras de TensorFlow, para la tarea de **análisis de sentimiento en español**.

## Introducción

En el procesamiento de lenguaje natural (PLN), el orden de las palabras y el contexto en una secuencia son cruciales para entender el significado. Las redes neuronales recurrentes (RNNs), y en particular las Long Short-Term Memory (LSTM), son arquitecturas diseñadas para procesar secuencias de datos, lo que las hace ideales para tareas de PLN como el análisis de sentimiento. Este cuaderno demuestra cómo una LSTM puede aprender a capturar estas dependencias temporales y clasificar el sentimiento de frases en español.

## Objetivos del Cuaderno

  * **Construir un modelo LSTM:** Aprender a definir la arquitectura de una red LSTM utilizando Keras en TensorFlow.
  * **Procesar texto como secuencias:** Entender cómo se tokenizan y se aplica *padding* a las frases para prepararlas como entrada a un modelo LSTM.
  * **Captar el contexto secuencial:** Comprender cómo una red LSTM es capaz de recordar el contexto de las palabras en una secuencia y cómo esto influye en el resultado de la clasificación.
  * **Realizar análisis de sentimiento:** Entrenar el modelo para clasificar frases en español como positivas o negativas.
  * **Observar el impacto del orden de las palabras:** Confirmar que el orden de las palabras es un factor influyente en las predicciones del modelo.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `numpy`
  * `tensorflow` (incluyendo `keras`)

## Cómo Ejecutar el Cuaderno

Sigue estos pasos para poner en marcha el cuaderno:

### 1\. Clonar el Repositorio (Opcional, si no lo tienes ya)

```bash
git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>
```

### 2\. Abrir el Cuaderno

Puedes abrir el cuaderno de dos maneras:

  * **En Google Colab (Recomendado para una configuración rápida):**

    1.  Ve a [Google Colab](https://colab.research.google.com/).
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `013_Análisis_de_Sentimiento_con_una_Red_LSTM_usando_Keras.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `013_Análisis_de_Sentimiento_con_una_Red_LSTM_usando_Keras.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código para instalar las librerías necesarias:

```python
import numpy as np
from tensorflow import keras
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Embedding, LSTM, Dense
from tensorflow.keras.preprocessing.text import Tokenizer
from tensorflow.keras.preprocessing.sequence import pad_sequences
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la preparación de los datos de sentimiento, la tokenización y *padding* de las secuencias, la definición de la arquitectura del modelo LSTM, su entrenamiento y la evaluación de sus predicciones con frases nuevas.

-----
