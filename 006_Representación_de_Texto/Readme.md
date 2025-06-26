# Representación de Texto en PLN: Bag-of-Words, TF-IDF y Word Embeddings
Este repositorio contiene un cuaderno de Jupyter (006_Representación_de_Texto.ipynb) que explora diversas técnicas de representación de texto en Procesamiento de Lenguaje Natural (PLN). Se abordan métodos clásicos como Bag-of-Words y TF-IDF, así como la introducción a los modernos Word Embeddings (Word2Vec).

## Introducción
Para que las computadoras puedan "entender" y procesar el lenguaje humano, el texto debe ser transformado en un formato numérico. Esta transformación, conocida como representación de texto, es un paso crucial en cualquier pipeline de PLN, ya que la calidad de esta representación impacta directamente el rendimiento de los modelos de machine learning subsiguientes. Este cuaderno explora diferentes enfoques para convertir palabras y documentos en vectores numéricos, desde métodos simples basados en conteo hasta representaciones densas y semánticamente ricas.

## Objetivos del Cuaderno
Entender la necesidad de la representación numérica: Comprender por qué el texto debe ser convertido a números para el procesamiento computacional.
Aprender Bag-of-Words (BoW): Entender su funcionamiento, implementación con CountVectorizer de scikit-learn, y sus limitaciones.
Aprender TF-IDF: Comprender cómo pondera la importancia de las palabras, su implementación con TfidfVectorizer de scikit-learn, y sus ventajas sobre BoW.
Introducción a Word Embeddings (Word2Vec): Entender el concepto de representaciones densas y contextuales, y cómo se utilizan para capturar relaciones semánticas entre palabras.
Visualizar Embeddings: Utilizar UMAP para reducir la dimensionalidad y visualizar las relaciones entre palabras en un espacio 2D.
Aplicar preprocesamiento: Integrar técnicas de limpieza y lematización vistas en módulos anteriores.
Requisitos para Ejecutar el Cuaderno
Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

* nltk
* spacy
* scikit-learn
* gensim
* matplotlib
* seaborn
* umap-learn
* bokeh (opcional, para visualizaciones interactivas si se habilitan)
* Además, para spaCy, es necesario descargar el modelo de idioma español.

Cómo Ejecutar el Cuaderno
Sigue estos pasos para poner en marcha el cuaderno:

### 1. Clonar el Repositorio (Opcional, si no lo tienes ya)

git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>

### 2. Abrir el Cuaderno
Puedes abrir el cuaderno de dos maneras:

En Google Colab (Recomendado para una configuración rápida):

- I. Ve a Google Colab.

- II. Haz clic en File -> Upload notebook y selecciona 006_Representación_de_Texto.ipynb de tu repositorio local.

- III. Alternativamente, puedes abrirlo directamente desde GitHub: File -> Open notebook -> GitHub, y pegar la URL de tu .ipynb.

- IV. Localmente con Jupyter Notebook/Lab:

a. Asegúrate de tener Jupyter instalado (pip install jupyter).

b. Navega hasta el directorio donde guardaste el cuaderno en tu terminal.

c. Ejecuta jupyter notebook o jupyter lab.

d. Se abrirá una interfaz en tu navegador. Haz clic en 006_Representación_de_Texto.ipynb para abrirlo.

### 3. Instalar Dependencias y Descargar Modelos
Una vez abierto el cuaderno, ejecuta las primeras celdas de código que contienen los comandos de instalación y descarga. Asegúrate de ejecutar todas las celdas de instalación:

**Instalar librerías**
!pip install -q nltk spacy scikit-learn gensim matplotlib seaborn umap-learn bokeh

**Descargar modelo de spaCy en español**
!python -m spacy download es_core_news_sm > /dev/null

**Descargar datos de NLTK**
import nltk
nltk.download('stopwords')
nltk.download('punkt')

### 4. Ejecutar las Celdas del Cuaderno
Ejecuta las celdas de código de forma secuencial. El cuaderno está estructurado para guiarte a través de la teoría y la aplicación práctica de cada método de representación de texto.
