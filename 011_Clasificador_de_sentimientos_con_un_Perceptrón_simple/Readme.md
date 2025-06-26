

# Clasificador de Sentimientos en Español con un Perceptrón Simple (desde Cero)

Este repositorio contiene un cuaderno de Jupyter (`011_Clasificador_de_sentimientos_con_un_Perceptrón_simple.ipynb`) que te guiará en la implementación de un **Perceptrón simple desde cero utilizando solo NumPy** para la tarea de **análisis de sentimiento en español rioplatense**.

## Introducción

El análisis de sentimiento es una tarea fundamental en el Procesamiento de Lenguaje Natural (PLN) que busca determinar la polaridad emocional (positivo, negativo, neutro) de un texto. Este cuaderno te ofrece una inmersión práctica en las bases del *Machine Learning*, construyendo una de las unidades más elementales de las redes neuronales: el Perceptrón. Al implementarlo desde cero, obtendrás una comprensión profunda de cómo una neurona artificial aprende a clasificar datos mediante el ajuste de pesos.

## Objetivos del Cuaderno

  * **Implementar un Perceptrón desde Cero:** Construir la lógica de una neurona artificial básica utilizando exclusivamente `NumPy`.
  * **Entender el Proceso de Entrenamiento:** Comprender cómo el Perceptrón ajusta sus pesos y el sesgo (`bias`) para minimizar errores y aprender a clasificar.
  * **Aplicar a Análisis de Sentimiento:** Entrenar el Perceptrón con un pequeño conjunto de frases en español rioplatense para clasificar su sentimiento como positivo o negativo.
  * **Realizar Predicciones:** Utilizar el modelo entrenado para predecir el sentimiento de nuevas frases.
  * **Reflexionar sobre Limitaciones:** Entender las capacidades y las limitaciones de un modelo tan simple como el Perceptrón en tareas de PLN.

## Requisitos para Ejecutar el Cuaderno

Para ejecutar este cuaderno en tu entorno local o en Google Colab, solo necesitarás tener instalada la librería:

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
    2.  Haz clic en `File` -\> `Upload notebook` y selecciona `011_Clasificador_de_sentimientos_con_un_Perceptrón_simple.ipynb` de tu repositorio local.
    3.  Alternativamente, puedes abrirlo directamente desde GitHub: `File` -\> `Open notebook` -\> `GitHub`, y pegar la URL de tu `.ipynb`.

  * **Localmente con Jupyter Notebook/Lab:**

    1.  Asegúrate de tener Jupyter instalado (`pip install jupyter`).
    2.  Navega hasta el directorio donde guardaste el cuaderno en tu terminal.
    3.  Ejecuta `jupyter notebook` o `jupyter lab`.
    4.  Se abrirá una interfaz en tu navegador. Haz clic en `011_Clasificador_de_sentimientos_con_un_Perceptrón_simple.ipynb` para abrirlo.

### 3\. Instalar Dependencias

Una vez abierto el cuaderno, ejecuta la primera celda de código (si no la tienes ya instalada):

```python
!pip install -q numpy
```

### 4\. Ejecutar las Celdas del Cuaderno

Ejecuta las celdas de código de forma secuencial. El cuaderno te guiará paso a paso a través de la definición de los datos, la creación de la clase `Perceptron`, el entrenamiento del modelo y la realización de predicciones.

-----
