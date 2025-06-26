
# Reconocimiento de Entidades Nombradas (NER) con Transformers y Gemini API usando Gradio

Este repositorio contiene un cuaderno de Jupyter (`018_gemini_gradio.ipynb`) que presenta un ejercicio práctico sobre **Reconocimiento de Entidades Nombradas (NER)**. El cuaderno demuestra cómo implementar NER utilizando tanto **modelos pre-entrenados de Hugging Face Transformers** como la **API de Google Gemini**, y cómo crear una interfaz interactiva sencilla con **Gradio**.

## Introducción

El Reconocimiento de Entidades Nombradas (NER) es una tarea fundamental en el Procesamiento de Lenguaje Natural (PLN) que consiste en identificar y clasificar entidades (como nombres de personas, organizaciones, ubicaciones, fechas, etc.) dentro de un texto. Este cuaderno explora dos enfoques modernos para NER: el uso de modelos Transformer de última generación, y la aplicación de grandes modelos de lenguaje (LLMs) como Gemini a través de su API. Además, se integra Gradio para construir una interfaz de usuario interactiva que permite probar estos modelos de manera rápida y eficiente.

## Objetivos del Cuaderno

  * **Implementar NER con modelos pre-entrenados:** Utilizar modelos de clasificación de *tokens* de Hugging Face para realizar NER en español.
  * **Utilizar APIs de IA generativa para PLN:** Realizar NER usando la capacidad de los modelos LLM como Google Gemini.
  * **Crear interfaces interactivas con Gradio:** Aprender a construir una aplicación web simple y funcional para interactuar con los modelos de PLN.
  * **Comparar diferentes enfoques de NER:** Observar las diferencias y similitudes en los resultados y la implementación entre los modelos de Transformers y la API de Gemini para la tarea de NER.
  * **Desarrollar prototipos rápidos:** Entender cómo se pueden crear prototipos de aplicaciones de PLN de manera ágil.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `transformers`
  * `torch` o `tensorflow` (como *backend* para `transformers`)
  * `google-generativeai`
  * `gradio`
  * `python-dotenv` (opcional, para gestionar la clave de API de forma segura)

Además, para utilizar la API de Google Gemini, necesitarás obtener una **clave de API** de Google AI Studio.

## Cómo Ejecutar el Cuaderno

Sigue estos pasos para poner en marcha el cuaderno:

### 1\. Clonar el Repositorio (Opcional, si no lo tienes ya)

```bash
git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>
```

### 2\. Abrir el Cuaderno

Puedes abrir el cuaderno de dos maneras:

  * **En Google Colab (Recomendado para una configuración rápida y uso de GPU):**

    1.  Ve a [Google Colab](https://colab.research.google.com/).
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `018_gemini_gradio.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`. Asegúrate de cambiar el entorno de ejecución a GPU (`Runtime` -\> `Change runtime type` -\> `GPU`).

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `018_gemini_gradio.ipynb` para abrirlo.

### 3\. Instalar Dependencias y Configurar la API Key

Una vez abierto el cuaderno, ejecuta las primeras celdas de código. Asegúrate de:

1.  **Instalar las librerías necesarias:**

    ```python
    # Instalación de librerías necesarias
    !pip install -q transformers torch google-generativeai gradio python-dotenv
    ```

2.  **Configurar tu Clave de API de Google Gemini:**
    El cuaderno te indicará cómo cargar tu clave de API, ya sea directamente en una variable de entorno de Colab o desde un archivo `.env` si estás ejecutando localmente. **Nunca compartas tu clave de API directamente en tu código público.**

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la implementación de NER con ambos enfoques y la creación de la interfaz de Gradio para una interacción sencilla y comparación de resultados.

-----
