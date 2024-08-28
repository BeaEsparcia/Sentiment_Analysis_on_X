# Análisis de sentimientos en X sobre feminismo

- Python 3.6+
- Transformers: latest
- Pandas: latest
- MatplobLib: latest

## Descripción del proyecto

Este proyecto realiza un análisis de sentimientos en una colección de tuits sobre el tema del feminismo. El objetivo principal es identificar y categorizar las emociones predominantes en estas publicaciones utilizando un modelo preentrenado de procesamiento de lenguaje natural (PLN).

## Características

- Utiliza el modelo preentrenado nlptown/bert-base-multilingual-uncased-sentiment para el análisis de sentimientos.
- Clasifica los tuits en cinco categorías: muy negativo, negativo, neutral, positivo y muy positivo.
- Visualiza la distribución de sentimientos mediante gráficos de barras.
- Incluye un análisis crítico de los resultados y posibles mejoras.

## Tecnologías utilizadas

- Python 3.6+
- Transformers (Hugging Face)
- Pandas
- Matplotlib

## Requisitos del sistema

- Python 3.6 o superior
- Jupyter Notebook o Google Colab
- Acceso a internet para descargar el modelo preentrenado

Nota: Si utiliza Google Colab, no necesita instalar nada localmente, ya que el entorno proporcionado ya incluye la mayoría de las bibliotecas necesarias.

## Instalación y uso

### Opción 1: ejecución local

1. Clone este repositorio: git clone https://github.com/tu-usuario/analisis-sentimientos-feminismo.git
cd analisis-sentimientos-feminismo
2. Instale las dependencias: pip install -r requirements.txt
3. Inicie Jupyter Notebook
4. Abra el archivo Analisis_Sentimientos_X.ipynb en la interfaz de Jupyter Notebook
5. Ejecute las celdas del notebook en orden

### Opción 2: Uso de Google Colab

1. Acceda a Google Colab
2. Seleccione "Archivo" > "Subir cuaderno" y suba el archivo Análisis_de_sentimientos_en_X_sobre_feminismo.ipynb
3. Una vez abierto, asegúrese de que el entorno de ejecución esté configurado para usar GPU:
  - Vaya a "Entorno de ejecución" > "Cambiar tipo de entorno de ejecución"
  - Seleccione "GPU" como tipo de hardware acelerador
4. Ejecuta las celdas del notebook en orden

Nota: Si ejecuta el notebook en Google Colab, es posible que necesite instalar algunas bibliotecas adicionales. Puede hacerlo añadiendo y ejecutando una celda con los siguientes comandos al principio del notebook: !pip install transformers pandas matplotlib

Asegúrese de reiniciar el entorno de ejecución después de instalar nuevas bibliotecas.

## Resultados y observaciones

Al analizar los resultados, se observaron algunos problemas en las clasificaciones:

- **Faltas en la Comprensión del Contexto**: algunos tuits claramente positivos fueron etiquetados como `Muy Negativo` y viceversa.
- **Clasificaciones Incorrectas**: el modelo puede malinterpretar el tono o el contexto de ciertos tuits, especialmente en temas complejos como el feminismo.

### Ejemplos de clasificaciones incorrectas

- Un tuit que afirmaba "SÍ. SOY FEMINISTA. #feminismo #igualdad #8Marzo #8M" fue etiquetado como `Muy Negativo`, lo cual es un error evidente.
- Otro tuit que criticaba el feminismo fue etiquetado como `Muy Positivo`.

## Limitaciones y posibles mejoras

- **Ajuste fino del modelo**: afinar el modelo con un conjunto de datos específico sobre feminismo podría mejorar significativamente la precisión de las clasificaciones.
- **Implementación de reglas heurísticas**: aplicar reglas basadas en palabras clave o frases para corregir automáticamente ciertas clasificaciones erróneas.
- **Revisión Manual**: incorporar una fase de revisión manual para corregir errores evidentes y mejorar la calidad general del análisis.
- **Ampliación del conjunto de datos**: aumentar la cantidad y diversidad de tuits analizados para obtener una visión más completa y representativa.
- **Análisis de subjetividad**: implementar un análisis adicional para distinguir entre opiniones subjetivas y hechos objetivos.

## Reflexión

Este proyecto demuestra la importancia de entender las limitaciones de los modelos preentrenados, especialmente cuando se aplican a temas complejos y sensibles como el feminismo. La combinación de análisis automático con revisión humana es crucial para obtener resultados más precisos y significativos.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abra un issue primero para discutir qué le gustaría cambiar o añadir.

## Licencia

Este proyecto está bajo la Licencia MIT. Vea el archivo LICENSE para más detalles.

## Contacto

Beatriz Esparcia - esparcia.beatriz@gmail.com
LinkedIn: Beatriz Esparcia
Link del Proyecto: https://github.com/tu-usuario/analisis-sentimientos-feminismo
