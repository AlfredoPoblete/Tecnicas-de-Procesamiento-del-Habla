

# Introducción a Word Embeddings y Word2Vec

Este repositorio contiene un cuaderno de Jupyter (`009_Word_Embeddings_y_Word2Vec.ipynb`) que sirve como una introducción a los **Word Embeddings** y, en particular, al algoritmo **Word2Vec**. El objetivo es comprender cómo estas representaciones vectoriales densas permiten a los algoritmos de Machine Learning capturar el significado y las relaciones entre palabras.

## Introducción

En el procesamiento de lenguaje natural (PLN), las palabras son las unidades fundamentales de información. Sin embargo, para que las máquinas puedan trabajar con ellas, necesitan ser convertidas en un formato numérico. Métodos tradicionales como Bag-of-Words o TF-IDF tienen limitaciones al no capturar la semántica o las relaciones contextuales entre palabras. Los *Word Embeddings* surgen como una solución, representando palabras como vectores en un espacio multidimensional donde la proximidad entre vectores indica similitud semántica. Word2Vec es uno de los algoritmos pioneros y más influyentes en este campo.

## Objetivos del Cuaderno

  * **Entender las limitaciones de BoW/TF-IDF:** Comprender por qué las representaciones dispersas no son suficientes para capturar la complejidad del lenguaje.
  * **Comprender el concepto de Word Embeddings:** Entender qué son los vectores densos semánticos y por qué son importantes.
  * **Conocer las arquitecturas Word2Vec:** Aprender sobre los dos modelos principales de Word2Vec: CBOW (Continuous Bag-of-Words) y Skip-gram.
  * **Cargar y usar vectores Word2Vec pre-entrenados:** Implementar la carga de modelos pre-entrenados con la librería `gensim`.
  * **Explorar similitud y analogías entre palabras:** Realizar consultas para encontrar palabras similares y resolver analogías vectoriales.
  * **(Opcional) Visualizar embeddings:** Utilizar técnicas de reducción de dimensionalidad para visualizar las relaciones entre palabras en un espacio 2D.
  * **Reflexionar sobre sesgos:** Discutir cómo los sesgos presentes en los datos de entrenamiento pueden reflejarse en los embeddings.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

  * `nltk`
  * `spacy`
  * `gensim`
  * `numpy`
  * `matplotlib`
  * `seaborn`
  * `umap-learn` (opcional, para visualización)

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `009_Word_Embeddings_y_Word2Vec.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `009_Word_Embeddings_y_Word2Vec.ipynb` para abrirlo.

### 3\. Instalar Dependencias y Descargar Modelos/Datos

Una vez abierto el cuaderno, **es crucial ejecutar las primeras celdas de código que contienen los comandos de instalación y descarga.** Estas celdas se encargarán de:

  * Instalar todas las librerías necesarias (NLTK, spaCy, Gensim, UMAP, etc.).
  * Descargar el modelo `es_core_news_sm` de spaCy.
  * Descargar los *stopwords* y *punkt* de NLTK.
  * **Descargar un modelo pre-entrenado de Word2Vec para español.** Ten en cuenta que este archivo puede ser grande (varios cientos de MBs o GBs dependiendo del modelo), por lo que la descarga puede tardar un tiempo considerable dependiendo de tu conexión a internet.

<!-- end list -->

```python
# Instalar librerías
!pip install -q nltk spacy gensim numpy matplotlib seaborn umap-learn

# Descargar modelo de spaCy
!python -m spacy download es_core_news_sm > /dev/null

# Descargar datos de NLTK
import nltk
nltk.download('stopwords')
nltk.download('punkt')

# **IMPORTANTE:** La celda para descargar el modelo pre-entrenado de Word2Vec
# está incluida en el cuaderno. Asegúrate de ejecutarla.
# Puede tomar un tiempo debido al tamaño del archivo.
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la teoría de Word2Vec, la carga de los embeddings, la exploración de similitudes y analogías, y la visualización de los espacios vectoriales de las palabras.

-----
