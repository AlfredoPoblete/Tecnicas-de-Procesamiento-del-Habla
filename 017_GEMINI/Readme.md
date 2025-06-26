
# Procesamiento de Lenguaje Natural con Google Gemini API

Este repositorio contiene un cuaderno de Jupyter (`017_GEMINI.ipynb`) que demuestra diversas aplicaciones de Procesamiento de Lenguaje Natural (PLN) utilizando el modelo **Gemini de Google** a través de la librería `google-generativeai`.

## Introducción

Los modelos de lenguaje grandes (LLMs) como Gemini están transformando la forma en que interactuamos con el texto, permitiendo realizar tareas de PLN complejas con una facilidad sin precedentes. Este cuaderno te guiará a través de ejemplos prácticos de cómo integrar la API de Gemini en tus proyectos Python para llevar a cabo diversas operaciones, desde la generación de texto hasta el análisis avanzado de contenido.

## Objetivos del Cuaderno

  * **Conectar con la API de Gemini:** Aprender a configurar el entorno y autenticarse para usar la API de Google Gemini.
  * **Generación de Texto:** Explorar la capacidad del modelo para generar texto coherente y relevante a partir de *prompts* dados.
  * **Análisis de Sentimiento:** Clasificar la polaridad emocional de frases y textos.
  * **Resumen de Texto:** Generar resúmenes concisos de documentos más largos.
  * **Extracción y Clasificación de Entidades:** Identificar y categorizar entidades nombradas dentro de un texto (personas, lugares, organizaciones, etc.).
  * **Traducción de Texto:** Realizar traducciones automáticas entre idiomas.
  * **Aplicar modelos multimodales (opcional si el cuaderno lo cubre):** Si el cuaderno incluye ejemplos multimodales, se mostrará cómo Gemini puede procesar y generar contenido basado en texto e imágenes.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás:

  * **Clave de API de Google Gemini:** Debes obtener una clave de API desde [Google AI Studio](https://makersuite.google.com/app/apikey) o la consola de Google Cloud.
  * Librería `google-generativeai`.
  * `python-dotenv` (opcional, para gestionar la clave de API de forma segura)

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `017_GEMINI.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `017_GEMINI.ipynb` para abrirlo.

### 3\. Instalar Dependencias y Configurar la API Key

Una vez abierto el cuaderno, ejecuta las primeras celdas de código. Asegúrate de:

1.  **Instalar las librerías necesarias:**

    ```python
    !pip install -q -U google-generativeai python-dotenv
    ```

2.  **Configurar tu Clave de API:**
    El cuaderno te indicará cómo cargar tu clave de API, ya sea directamente en una variable de entorno de Colab o desde un archivo `.env` si estás ejecutando localmente. **Nunca compartas tu clave de API directamente en tu código público.**

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de ejemplos interactivos de diversas tareas de PLN, utilizando la API de Gemini para procesar y generar texto.

-----
