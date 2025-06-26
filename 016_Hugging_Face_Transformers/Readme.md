
# Aplicaciones de Transformers en Procesamiento de Lenguaje Natural (Hugging Face)

Este repositorio contiene un cuaderno de Jupyter (`016_Hugging_Face_Transformers.ipynb`) que profundiza en las **aplicaciones de los modelos Transformer** en diversas tareas de Procesamiento de Lenguaje Natural (PLN), haciendo uso extensivo de la librería **Hugging Face `transformers`**.

## Introducción

Los modelos **Transformer** han revolucionado el campo del PLN al introducir el mecanismo de *atención*, que les permite procesar secuencias de texto de manera más eficiente y capturar dependencias a largo plazo que eran difíciles para arquitecturas anteriores como las RNNs. La librería `transformers` de Hugging Face ha democratizado el acceso a estos modelos de vanguardia, facilitando su uso para una amplia gama de tareas sin la necesidad de entrenar modelos desde cero. Este cuaderno ofrece una visión tanto teórica como práctica de los Transformers, cubriendo desde sus fundamentos hasta su aplicación en tareas avanzadas.

## Objetivos del Cuaderno

  * **Comprender la Arquitectura Transformer:** Obtener una comprensión de alto nivel sobre cómo funciona la arquitectura Transformer, especialmente el mecanismo de *atención*.
  * **Dominar la librería `transformers` de Hugging Face:** Aprender a utilizar las clases clave de la librería (`pipeline`, `AutoTokenizer`, `AutoModel`).
  * **Realizar diversas tareas de PLN:**
      * **Generación de Texto:** Crear texto coherente a partir de un *prompt*.
      * **Relleno de Máscaras (Fill-Mask):** Predecir palabras faltantes en una oración.
      * **Detección de Entidades Nombradas (NER):** Identificar y clasificar entidades como personas, organizaciones, lugares, etc.
      * **Resumen Abstractivo:** Generar resúmenes que pueden contener palabras no presentes en el texto original.
      * **Clasificación Zero-Shot:** Clasificar texto en categorías arbitrarias sin necesidad de ejemplos de entrenamiento etiquetados para esas categorías.
  * **Trabajar con modelos en español:** Aplicar modelos pre-entrenados diseñados específicamente para el idioma español.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instalada la siguiente librería de Python:

  * `transformers`
  * `torch` o `tensorflow` (Hugging Face puede usar cualquiera de los backends, y se instalará automáticamente con `transformers` si no está presente)

Si estás ejecutando el cuaderno en Google Colab, la instalación es generalmente sencilla y se recomienda activar la GPU para un mejor rendimiento.

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `016_Hugging_Face_Transformers.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`. Asegúrate de cambiar el entorno de ejecución a GPU (`Runtime` -\> `Change runtime type` -\> `GPU`).

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `016_Hugging_Face_Transformers.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código para instalar la librería `transformers`:

```python
# Instalación de Hugging Face Transformers
!pip install -q transformers
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la teoría de los Transformers, la inicialización de diferentes `pipeline` de Hugging Face y la aplicación de estos modelos a diversas tareas de PLN en español.

-----
