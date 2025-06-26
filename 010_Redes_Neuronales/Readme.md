
# Redes Neuronales en PLN: Preparación y Clasificación de Texto con TensorFlow/Keras

Este repositorio contiene un cuaderno de Jupyter (`010_Redes_Neuronales.ipynb`) que introduce los conceptos fundamentales para preparar datos de texto y construir un modelo básico de clasificación utilizando **Redes Neuronales** con la biblioteca **TensorFlow/Keras**.

## Introducción

Las redes neuronales son herramientas increíblemente poderosas en el Procesamiento de Lenguaje Natural (PLN) para comprender y generar texto. Sin embargo, antes de poder alimentar texto crudo a estos modelos, necesitamos transformarlo en un formato numérico que puedan entender. Este cuaderno te guiará a través de los pasos esenciales para realizar esta transformación y construir un clasificador de texto simple, sentando las bases para arquitecturas más complejas en PLN.

## Objetivos del Cuaderno

  * **Creación de un Dataset Sintético:** Generar un pequeño conjunto de datos de ejemplo para ilustrar el proceso de principio a fin.
  * **Tokenización de Texto:** Convertir palabras en números enteros, creando un vocabulario. Esto es el puente entre el texto y las representaciones numéricas.
  * **Padding (Relleno) de Secuencias:** Asegurar que todas las secuencias de texto tengan la misma longitud, un requisito clave para la entrada a las redes neuronales.
  * **Construcción de un Modelo Simple:** Crear una red neuronal básica utilizando la API de Keras de TensorFlow, incluyendo una capa de *Embedding* para aprender representaciones de palabras.
  * **Entrenamiento y Evaluación:** Entrenar el modelo con los datos preparados y evaluar su rendimiento en una tarea de clasificación de texto.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `tensorflow`
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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `010_Redes_Neuronales.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `010_Redes_Neuronales.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código que contiene los comandos de instalación:

```python
# Instalar TensorFlow y otras librerías necesarias
!pip install -q tensorflow numpy
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la creación del dataset sintético, el preprocesamiento de texto (tokenización y padding), la definición de la arquitectura de la red neuronal y su entrenamiento.

-----
