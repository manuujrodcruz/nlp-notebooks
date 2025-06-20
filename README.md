# Portafolio de Ejercicios de Procesamiento de Lenguaje Natural (NLP)

Este repositorio contiene un portafolio de ejercicios prácticos realizados como parte de un curso de **Procesamiento de Lenguaje Natural**. Los ejercicios están organizados en dos Jupyter Notebooks que cubren técnicas fundamentales de NLP, incluyendo preprocesamiento de texto, análisis gramatical, representaciones de texto, y word embeddings, utilizando corpus como noticias de ESPN o el `webtext` de NLTK.

## Objetivo del Proyecto

El propósito de este portafolio es aplicar conceptos y técnicas de procesamiento de lenguaje natural a través de ejercicios prácticos, explorando, limpiando, analizando, y representando texto de manera computacional. Los ejercicios buscan desarrollar habilidades en el manejo de herramientas de NLP y la implementación de algoritmos para tareas específicas.

## Contenido

El repositorio incluye dos Jupyter Notebooks con las siguientes tareas:

### Portafolio Ejercicios 1.ipynb
- **Recolección de datos**: Análisis del corpus `webtext` de NLTK, selección de un archivo específico, y justificación de la elección.
- **Descripción y exploración de datos**: Uso de Pandas para generar estadísticas descriptivas y explorar los textos.
- **Limpieza de datos**: Aplicación de técnicas de limpieza (eliminación de puntuación, palabras vacías, etc.) con explicación de cada método.
- **Connotación emocional**: Uso del corpus `opinion_lexicon` de NLTK para identificar palabras con connotaciones positivas y negativas, acompañado de estadísticas y visualizaciones.
- **WordNet**: Desarrollo de una función para obtener synsets de palabras según su categoría gramatical (sustantivo, verbo, adjetivo, adverbio).

### Portafolio Ejercicios 2.ipynb
- **Lematización y stemming**: Preprocesamiento de un corpus de noticias de ESPN para tokenizar, eliminar puntuación y palabras vacías, y generar listas de tokens lematizados y con stemming.
- **Etiquetado gramatical**: Etiquetado de partes del discurso (POS tagging) y almacenamiento de resultados en un diccionario.
- **Taxonomías**: Obtención de hiperónimos para los synsets de tokens según su etiqueta gramatical.
- **N-gramas**: Desarrollo de una función para generar n-gramas de un corpus, con pruebas para diferentes valores de *n*.
- **Representaciones de texto básicas**: Representación de documentos como vectores usando one-hot encoding, bag of words, y TF-IDF, aplicadas a textos tokenizados, lematizados, stemmizados, y bigramas.
- **Word embeddings**: Entrenamiento de un modelo Word2Vec sobre el corpus de documentos, con exploración de vectores y palabras similares.
- **Profundización en word embeddings**: Uso avanzado de la librería Gensim para guardar modelos, emplear KeyedVectors, y experimentar con modelos preentrenados.

## Herramientas Utilizadas

- **Python**: Lenguaje principal para el desarrollo de los ejercicios.
- **NLTK**: Para preprocesamiento de texto, acceso a corpus (`webtext`, `opinion_lexicon`, `wordnet`), y análisis gramatical.
- **Pandas** y **NumPy**: Para manipulación y análisis de datos.
- **Matplotlib** y **Seaborn**: Para visualización de datos.
- **Scikit-learn**: Para vectorización de texto (CountVectorizer, TfidfVectorizer).
- **Gensim**: Para entrenamiento y exploración de word embeddings con Word2Vec.

## Estructura del Repositorio

- `/Portafolio Ejercicios 1.ipynb`: Notebook con los ejercicios de recolección, exploración, limpieza, análisis emocional, y uso de WordNet.
- `/Portafolio Ejercicios 2.ipynb`: Notebook con los ejercicios de preprocesamiento, etiquetado gramatical, taxonomías, n-gramas, representaciones de texto, y word embeddings.

## Instrucciones de Uso

1. Clona este repositorio:
   ```bash
   git clone https://github.com/manuujrodcruz/nlp-notebooks.git
   ```
2. Instala las dependencias necesarias:
   ```bash
   pip install -r requirements.txt
   ```
   Nota: Si no hay un archivo `requirements.txt`, instala las bibliotecas manualmente:
   ```bash
   pip install numpy pandas matplotlib seaborn nltk scikit-learn gensim
   ```
3. Descarga los recursos de NLTK necesarios:
   ```python
   import nltk
   nltk.download('webtext')
   nltk.download('opinion_lexicon')
   nltk.download('wordnet')
   nltk.download('punkt')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('stopwords')
   ```
4. Abre los notebooks en Jupyter:
   ```bash
   jupyter notebook
   ```
5. Ejecuta las celdas en orden para reproducir los ejercicios.

## Contribuciones

Este proyecto fue desarrollado por **Manuel José Rodríguez Cruz**. Agradezco cualquier comentario o sugerencia para mejorar el contenido. Si deseas contribuir, por favor abre un *issue* o envía un *pull request*.