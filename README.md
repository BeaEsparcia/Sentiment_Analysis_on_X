# Análisis de Sentimientos en Twitter sobre Feminismo

## Descripción del Proyecto

Este proyecto realiza un análisis de sentimientos en una colección de tuits sobre el tema del feminismo. El objetivo principal es identificar y categorizar las emociones predominantes en estas publicaciones utilizando un modelo preentrenado de procesamiento de lenguaje natural (PLN).

## Enfoque Utilizado

Se empleó el modelo `nlptown/bert-base-multilingual-uncased-sentiment`, un modelo preentrenado diseñado para realizar análisis de sentimientos en múltiples idiomas, incluyendo español. Este modelo clasifica cada tuit en una de las siguientes categorías: `Muy Negativo`, `Negativo`, `Neutral`, `Positivo`, y `Muy Positivo`.

## Resultados y Observaciones

Al analizar los resultados, se observaron algunos problemas en las clasificaciones:

- **Faltas en la Comprensión del Contexto**: Algunos tuits claramente positivos fueron etiquetados como `Muy Negativo` y viceversa.
- **Clasificaciones Incorrectas**: El modelo puede malinterpretar el tono o el contexto de ciertos tuits, especialmente en temas complejos como el feminismo.

### Ejemplos de Clasificaciones Incorrectas

- Un tuit que afirmaba "SÍ. SOY FEMINISTA. #feminismo #igualdad #8Marzo #8M" fue etiquetado como `Muy Negativo`, lo cual es un error evidente.
- Otro tuit que criticaba el feminismo fue etiquetado como `Muy Positivo`.

## Posibles Mejoras

- **Ajuste Fino del Modelo**: Afinar el modelo con un conjunto de datos específico sobre feminismo podría mejorar significativamente la precisión de las clasificaciones.
- **Implementación de Reglas Heurísticas**: Podrían aplicarse reglas heurísticas para corregir automáticamente ciertas clasificaciones.
- **Revisión Manual**: Una revisión manual de las clasificaciones, como la realizada en este proyecto, ayuda a identificar y corregir errores, lo cual es crucial para proyectos con datos sensibles.

## Reflexión

Este proyecto muestra la importancia de entender las limitaciones de los modelos preentrenados y cómo los análisis automáticos pueden ser mejorados con revisiones manuales o ajustes específicos. Este enfoque es especialmente relevante cuando se trabaja con temas complejos y sensibles como el feminismo.

## Requerimientos

- Python 3.6+
- Bibliotecas:
  - `transformers`
  - `pandas`
  - `matplotlib`

## Cómo Ejecutar el Proyecto

1. Clona este repositorio.
2. Instala las dependencias con `pip install -r requirements.txt`.
3. Ejecuta el script `sentiment_analysis.py` para generar el análisis de sentimientos y las visualizaciones.

## Contacto

Si tienes alguna pregunta sobre este proyecto, no dudes en contactarme en [esparcia.beatriz@gmail.com].
