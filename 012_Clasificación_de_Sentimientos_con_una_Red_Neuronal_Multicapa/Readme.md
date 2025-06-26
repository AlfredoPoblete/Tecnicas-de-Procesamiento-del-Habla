

# Clasificación de Sentimientos en Español con una Red Neuronal Multicapa (PyTorch)

Este repositorio contiene un cuaderno de Jupyter (`012_Clasificación_de_Sentimientos_con_una_Red_Neuronal_Multicapa.ipynb`) que te guiará en la construcción y entrenamiento de una **Red Neuronal Multicapa (MLP)** utilizando la librería **PyTorch** para la tarea de **análisis de sentimiento en español**.

## Introducción

Continuando con la exploración de las redes neuronales en PLN, este cuaderno da un paso adelante del Perceptrón simple para introducir las Redes Neuronales Multicapa (MLPs). Las MLPs son capaces de aprender relaciones más complejas en los datos textuales gracias a sus capas ocultas y funciones de activación no lineales. A través de este ejemplo práctico de clasificación de sentimientos, comprenderás cómo se construyen, entrenan y evalúan estas redes utilizando uno de los frameworks de Deep Learning más populares: PyTorch.

## Objetivos del Cuaderno

  * **Construir una Red Neuronal Multicapa:** Aprender a definir la arquitectura de una MLP con múltiples capas, utilizando `torch.nn`.
  * **Utilizar Funciones de Activación:** Comprender el rol de las funciones de activación (como ReLU) para introducir no linealidad en el modelo.
  * **Implementar el Flujo de Entrenamiento en PyTorch:** Familiarizarse con el ciclo de entrenamiento que incluye la pasada hacia adelante (forward pass), el cálculo de la pérdida, la retropropagación y la optimización.
  * **Preprocesar Texto para MLPs:** Aplicar un preprocesamiento básico de Bag-of-Words para preparar el texto para la entrada a la red.
  * **Comparar con el Perceptrón Simple:** Observar las ventajas y mejoras de una MLP frente a un Perceptrón simple en la tarea de clasificación de sentimientos.
  * **Realizar Predicciones:** Utilizar el modelo entrenado para clasificar el sentimiento de nuevas frases.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, solo necesitarás tener instaladas las siguientes librerías de Python:

  * `torch`
  * `numpy`

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `012_Clasificación_de_Sentimientos_con_una_Red_Neuronal_Multicapa.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `012_Clasificación_de_Sentimientos_con_una_Red_Neuronal_Multicapa.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código (si no las tienes ya instaladas):

```python
!pip install -q torch numpy
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará paso a paso a través de la preparación de los datos de sentimiento, la definición del modelo MLP en PyTorch, su entrenamiento y la evaluación de sus predicciones.

-----
