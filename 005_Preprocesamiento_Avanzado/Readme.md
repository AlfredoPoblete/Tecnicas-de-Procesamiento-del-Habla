#Preprocesamiento Avanzado en PLN: Stemming vs. Lematización con NLTK y spaCy

Este repositorio contiene un cuaderno de Jupyter que explora técnicas avanzadas de preprocesamiento de texto en Procesamiento de Lenguaje Natural (PLN), centrándose en la comparación entre Stemming y Lematización.

**Introducción**

El preprocesamiento de texto es un paso fundamental en cualquier proyecto de PLN. Antes de aplicar modelos de aprendizaje automático o realizar análisis complejos, es crucial limpiar y normalizar los datos textuales. Este cuaderno repasa las técnicas básicas de limpieza y tokenización, y luego profundiza en dos métodos clave para reducir la dimensionalidad y agrupar palabras con significados similares: Stemming y Lematización.

Se compararán ambas técnicas utilizando las librerías NLTK y spaCy en español, demostrando sus diferencias, ventajas y desventajas.

**Objetivos del Cuaderno**
1. Repasar la limpieza básica de texto: Convertir a minúsculas, eliminar números, quitar signos de puntuación y eliminar stopwords.
2. Entender y aplicar Stemming (NLTK): Conocer el proceso heurístico de cortar sufijos para obtener la "raíz" de una palabra.
3. Entender y aplicar Lematización (spaCy): Comprender el proceso lingüístico de encontrar la forma canónica o de diccionario de una palabra (su "lema").
4. Comparar los resultados: Analizar las diferencias entre los stems y los lemas generados por ambas técnicas.
5. Reflexionar sobre el impacto del preprocesamiento: Discutir cómo las decisiones de preprocesamiento pueden afectar el análisis posterior y potencialmente introducir sesgos.

**Requisitos para Ejecutar el Cuaderno**
Para ejecutar este cuaderno en tu entorno local o en Google Colab, necesitarás tener instaladas las siguientes librerías de Python:

1. nltk
2. spacy

Además, para spaCy, es necesario descargar el modelo de idioma español.

**Cómo Ejecutar el Cuaderno**
Sigue estos pasos para poner en marcha el cuaderno:

1. Clonar el Repositorio (Opcional, si no lo tienes ya)
Bash

git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>
2. Abrir el Cuaderno
Puedes abrir el cuaderno de dos maneras:

En Google Colab (Recomendado para una configuración rápida):

Ve a Google Colab.
Haz clic en File -> Upload notebook y selecciona 005_Preprocesamiento_Avanzado.ipynb de tu repositorio local.
Alternativamente, puedes abrirlo directamente desde GitHub: File -> Open notebook -> GitHub, y pegar la URL de tu .ipynb.
Localmente con Jupyter Notebook/Lab:

Asegúrate de tener Jupyter instalado (pip install jupyter).
Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
Ejecuta jupyter notebook o jupyter lab.
Se abrirá una interfaz en tu navegador. Haz clic en 005_Preprocesamiento_Avanzado.ipynb para abrirlo.
3. Instalar Dependencias y Descargar Modelos
Una vez abierto el cuaderno, ejecuta la primera celda de código que contiene los siguientes comandos:

Python
Instalar librerías (si no están ya en Colab)
!pip install nltk spacy > /dev/null
!python -m spacy download es_core_news_sm > /dev/null # Modelo pequeño de español para spaCy
Este paso instalará nltk y spaCy, y descargará el modelo pequeño de español necesario para la lematización con spaCy.

4. Ejecutar las Celdas del Cuaderno
Ejecuta las celdas de código de forma secuencial. El cuaderno está estructurado para guiarte a través de los conceptos y las aplicaciones de Stemming y Lematización, incluyendo un ejercicio práctico para aplicar ambas técnicas a un conjunto de frases de ejemplo.

##Contenido del Cuaderno
El cuaderno está dividido en las siguientes secciones principales:

1. Instalaciones e Importaciones: Configuración inicial del entorno.
2. Repaso: Limpieza básica y Tokenización: Se revisan los pasos fundamentales de preprocesamiento como pasar a minúsculas, quitar números, puntuación y stopwords, y la tokenización.
3. El problema de las variantes de palabras: Se introduce la necesidad de agrupar palabras con la misma raíz o significado base.
4. Stemming con NLTK: Explicación y aplicación del SnowballStemmer para español.
5. Lematización con spaCy: Explicación y aplicación del proceso de lematización utilizando el modelo es_core_news_sm de spaCy.
6. Comparación Stemming vs. Lematización: Análisis lado a lado de los resultados y discusión sobre cuándo usar cada técnica.
7. Micro-Laboratorio (Ejercicio Práctico): Un ejercicio guiado para aplicar y comparar ambas técnicas en un dataset de reseñas de películas.
8. Brainstorming: Reflexión sobre cómo el preprocesamiento puede influir en sesgos y discriminaciones, y la importancia de documentar las decisiones.
