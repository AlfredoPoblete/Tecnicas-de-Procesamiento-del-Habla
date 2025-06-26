# Anexo Integrador PLN: Preprocesamiento y Representación de Texto
Este repositorio contiene un cuaderno de Jupyter (007_Anexo_Integrador.ipynb) que sirve como un anexo integrador de los conceptos clave de preprocesamiento y representación de texto en Procesamiento de Lenguaje Natural (PLN). El objetivo es consolidar los conocimientos adquiridos en módulos anteriores, aplicándolos en un flujo de trabajo unificado.

## Introducción
En el ámbito del PLN, el preprocesamiento y la representación de texto son etapas fundamentales que preparan los datos textuales para el análisis computacional. Un preprocesamiento adecuado asegura la calidad de la información, mientras que una representación efectiva permite que los algoritmos de machine learning puedan trabajar con los datos lingüísticos. Este cuaderno combina técnicas de limpieza, normalización (stemming/lematización) y vectorización (Bag-of-Words, TF-IDF, Word Embeddings) para transformar texto crudo en un formato numérico útil para tareas de PLN.

## Objetivos del Cuaderno
* Integrar conocimientos: Unificar los conceptos de limpieza, tokenización, eliminación de stopwords, stemming, lematización y diferentes métodos de representación de texto.
* Aplicación práctica: Realizar un flujo de trabajo completo de preprocesamiento y representación sobre un conjunto de datos real.
* Comparar técnicas: Observar cómo las diferentes etapas de preprocesamiento y representación impactan en la forma final de los datos.
* Preparar para el modelado: Entender cómo estas transformaciones son la base para aplicar modelos de machine learning en tareas de PLN.

## Requisitos para Ejecutar el Cuaderno
Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

* nltk
* spacy
* scikit-learn
* gensim
* matplotlib
* seaborn
* umap-learn
* pandas
* Además, para spaCy, es necesario descargar el modelo de idioma español.

## Cómo Ejecutar el Cuaderno
Sigue estos pasos para poner en marcha el cuaderno:

### 1. Clonar el Repositorio (Opcional, si no lo tienes ya)

git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>

### 2. Abrir el Cuaderno
Puedes abrir el cuaderno de dos maneras:

En Google Colab (Recomendado para una configuración rápida):

1. Ve a Google Colab.

2. Haz clic en File -> Upload notebook y selecciona 007_Anexo_Integrador.ipynb de tu repositorio local.

3. Alternativamente, puedes abrirlo directamente desde GitHub: File -> Open notebook -> GitHub, y pegar la URL de tu .ipynb.

4. Localmente con Jupyter Notebook/Lab:

* Asegúrate de tener Jupyter instalado (pip install jupyter).
* Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
* Ejecuta jupyter notebook o jupyter lab.
* Se abrirá una interfaz en tu navegador. Haz clic en 007_Anexo_Integrador.ipynb para abrirlo.
### 3. Instalar Dependencias y Descargar Modelos
Una vez abierto el cuaderno, ejecuta las primeras celdas de código que contienen los comandos de instalación y descarga:

**Instalar librerías**

!pip install -q nltk spacy scikit-learn gensim matplotlib seaborn umap-learn pandas

**Descargar modelo de spaCy en español**

!python -m spacy download es_core_news_sm > /dev/null

**Descargar datos de NLTK**
import nltk

nltk.download('stopwords')

nltk.download('punkt')

### 4. Ejecutar las Celdas del Cuaderno
Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará a través de la carga de datos, el preprocesamiento con diferentes técnicas y la creación de representaciones de texto, consolidando los aprendizajes de módulos previos.

