

# Análisis de Sentimiento con Modelos Pre-entrenados de Hugging Face

Este repositorio contiene un cuaderno de Jupyter (`014_Análisis_de_Sentimiento_con_Modelos_Preentrenados_de_HuggingFace.ipynb`) que te guiará en el uso de **modelos pre-entrenados de Hugging Face** para la tarea de **análisis de sentimiento en español**.

## Introducción

En el campo del Procesamiento de Lenguaje Natural (PLN), entrenar modelos complejos desde cero es un proceso costoso y requiere grandes volúmenes de datos. La buena noticia es que el **Transfer Learning** nos permite aprovechar modelos ya entrenados en tareas similares y adaptarlos a nuestras necesidades específicas. Hugging Face es una plataforma líder que democratiza el acceso a miles de modelos pre-entrenados de última generación. Este cuaderno demuestra la facilidad y eficiencia de usar estos modelos para realizar análisis de sentimiento, evitando la necesidad de entrenar una red neuronal desde cero.

## Objetivos del Cuaderno

  * **Comprender la importancia de los modelos pre-entrenados:** Entender por qué y cuándo es ventajoso usar modelos ya entrenados en tareas de PLN.
  * **Utilizar la librería `transformers` de Hugging Face:** Familiarizarse con la API `pipeline` para realizar inferencia de manera sencilla.
  * **Realizar análisis de sentimiento en español:** Aplicar un modelo pre-entrenado específico para el idioma español para clasificar el sentimiento de diversas frases.
  * **Apreciar la eficiencia del Transfer Learning:** Observar cómo se pueden obtener resultados de alta calidad con muy poco código y sin la necesidad de entrenamiento.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `transformers`
  * `torch`
  * `sentencepiece`
  * `numpy`
  * `pandas`

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `014_Análisis_de_Sentimiento_con_Modelos_Preentrenados_de_HuggingFace.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `014_Análisis_de_Sentimiento_con_Modelos_Preentrenados_de_HuggingFace.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código para instalar las librerías necesarias:

```python
!pip install -q transformers torch sentencepiece numpy pandas
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la carga del *pipeline* de Hugging Face y la realización de inferencias de sentimiento sobre frases de ejemplo.

-----
