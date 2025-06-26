

# Word Embeddings Avanzados: GloVe y FastText

Este repositorio contiene un cuaderno de Jupyter (`008_GloVe_y_FastText.ipynb`) que profundiza en el mundo de los *Word Embeddings*, explorando dos modelos populares y potentes: **GloVe** (Global Vectors for Word Representation) y **FastText**. El objetivo es comprender cómo estos modelos representan palabras en espacios vectoriales densos y cómo pueden capturar relaciones semánticas y sintácticas.

## Introducción

Los *Word Embeddings* son representaciones vectoriales densas de palabras que capturan su significado semántico y sintáctico a partir del contexto en el que aparecen. A diferencia de las representaciones dispersas como Bag-of-Words o TF-IDF, los embeddings permiten a los algoritmos de Machine Learning comprender relaciones entre palabras, como la sinonimia o la analogía. Este cuaderno explora dos enfoques avanzados para generar estos embeddings: GloVe, que se basa en estadísticas globales de co-ocurrencia, y FastText, que extiende la idea al considerar sub-palabras (caracteres n-gramas).

## Objetivos del Cuaderno

  * **Entender GloVe:** Comprender la filosofía de GloVe, cómo construye sus representaciones vectoriales a partir de la matriz de co-ocurrencia global y cómo cargar y utilizar embeddings pre-entrenados.
  * **Entender FastText:** Conocer el enfoque de FastText, su capacidad para manejar palabras fuera del vocabulario (OOV) y su utilidad en idiomas con morfología rica, y cómo cargar y utilizar sus embeddings pre-entrenados.
  * **Comparar propiedades:** Analizar las diferencias entre GloVe y FastText en términos de su construcción y rendimiento.
  * **Visualizar Embeddings:** Utilizar técnicas de reducción de dimensionalidad como UMAP para visualizar las relaciones semánticas entre palabras en un espacio 2D.
  * **Aplicar en español:** Trabajar con embeddings pre-entrenados específicos para el idioma español.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `nltk`
  * `spacy`
  * `gensim`
  * `numpy`
  * `matplotlib`
  * `seaborn`
  * `umap-learn`
  * `pandas`
  * `requests` (para descargar archivos)
  * `tqdm` (opcional, para barras de progreso)

Además, para `spaCy`, es necesario descargar el modelo de idioma español.

## Cómo Ejecutar el Cuaderno

Sigue estos pasos para poner en marcha el cuaderno:

### 1\. Clonar el Repositorio (Opcional, si no lo tienes ya)

```bash
git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>
```

### 2\. Abrir el Cuaderno

Puedes abrir el cuaderno de dos maneras:

  * **En Google Colab (Recomendado para una configuración rápida y descarga de archivos grandes):**

    1.  Ve a [Google Colab](https://colab.research.google.com/).
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `008_GloVe_y_FastText.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `008_GloVe_y_FastText.ipynb` para abrirlo.

### 3\. Instalar Dependencias y Descargar Modelos/Datos

Una vez abierto el cuaderno, **es crucial ejecutar las primeras celdas de código que contienen los comandos de instalación y descarga.** Estas celdas se encargarán de:

  * Instalar todas las librerías necesarias (NLTK, spaCy, Gensim, UMAP, etc.).
  * Descargar el modelo `es_core_news_sm` de spaCy.
  * Descargar los *stopwords* y *punkt* de NLTK.
  * **Descargar los modelos pre-entrenados de GloVe y FastText para español.** Ten en cuenta que estos archivos pueden ser grandes (varios GBs), por lo que la descarga puede tardar un tiempo considerable dependiendo de tu conexión a internet.

<!-- end list -->

```python
# Instalar librerías (estas son las principales, el notebook puede instalar más)
!pip install -q nltk spacy gensim numpy matplotlib seaborn umap-learn pandas requests tqdm

# Descargar modelo de spaCy
!python -m spacy download es_core_news_sm > /dev/null

# Descargar datos de NLTK
import nltk
nltk.download('stopwords')
nltk.download('punkt')

# **IMPORTANTE:** Las celdas para descargar los modelos de GloVe y FastText
# están incluidas en el cuaderno. Asegúrate de ejecutarlas.
# Pueden tomar un tiempo debido al tamaño de los archivos.
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la carga de los embeddings, la exploración de sus propiedades, la realización de analogías y la visualización de los espacios vectoriales de las palabras.

-----
