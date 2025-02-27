# Análisis de Géneros en Netflix

Este es un proyecto de análisis de datos en el que se explora el historial de películas y series vistas en Netflix, con el fin de identificar los géneros más vistos por el usuario. Para ello, utilicé Python, Google Colab y varias bibliotecas como *Pandas*, *Seaborn* y *Matplotlib*. El análisis se realiza mediante el cruce de dos conjuntos de datos:

1. Un *dataset de Kaggle* que contiene información sobre el catálogo de Netflix.
2. El *historial de visualización de Netflix* descargado directamente desde mi cuenta de Netflix.

## Descripción del Proyecto

El objetivo del proyecto es analizar las películas y series más vistas en Netflix, determinando cuáles son los géneros más populares basándonos en el historial de visualización personal del usuario. El análisis se realiza con las siguientes fases:

1. *Obtención del Dataset*:
   - Utilicé un dataset de Kaggle que contiene información sobre el catálogo de películas y series de Netflix. Este dataset no está completamente actualizado, ya que no incluye todas las películas y series que están actualmente en Netflix.
   
2. *Descarga del Historial de Netflix*:
   - Se debe descargar el historial de películas y series vistas desde la cuenta personal de Netflix. Es importante que este historial sea descargado con el idioma configurado en *inglés*, ya que los nombres de las películas y las categorías de género están en ese idioma.
   - Para descargarlo, ve a la sección de configuraciones de tu cuenta de Netflix y selecciona la opción para descargar el historial de visualización.
   
3. *Limpieza y Preparación de Datos*:
   - Los datos del historial de Netflix y el dataset de Kaggle fueron limpiados y procesados para asegurar que ambos conjuntos de datos pudieran ser combinados correctamente. Se unieron las dos tablas utilizando claves comunes, como el título de las películas y series.

4. *Análisis y Visualización*:
   - Utilizando *Pandas*, se realizó el análisis de los datos para identificar los géneros más vistos.
   - Se utilizó *Seaborn* y *Matplotlib* para crear visualizaciones que muestran la distribución de los géneros más populares entre las películas y series vistas por el usuario.

## Requisitos

- Python 3.x
- Google Colab (o Jupyter Notebook)
- Bibliotecas:
  - *Pandas*
  - *Seaborn*
  - *Matplotlib*
  - *Kaggle API* (opcional para descargar el dataset directamente desde Kaggle)

## Instrucciones

1. *Descargar el Dataset de Kaggle*:
   - Descarga el archivo CSV del repositorio con el dataset
   - O Dirígete al sitio web de Kaggle y descarga el dataset de Netflix [aquí](https://www.kaggle.com/datasets).
   
3. *Descargar tu Historial de Netflix*:
   - Ve a tu cuenta de Netflix y accede a las configuraciones de cuenta.
   - Busca la opción de "Descargar tu historial de visualización" y selecciona el idioma en *inglés*.
   
4. *Sube ambos archivos a Google Colab*:
   - Sube tanto el archivo del historial de Netflix como el dataset de Kaggle a tu entorno de Google Colab o Jupyter Notebook.

5. *Ejecutar el Script*:
   - Una vez los archivos estén cargados, ejecuta el script de análisis, el cual realizará las siguientes tareas:
     - Cargar ambos conjuntos de datos.
     - Limpiar y preparar los datos para análisis.
     - Generar un gráfico que muestre los géneros más vistos en tu historial.

## Script

El script principal se encuentra en el archivo netflix_user_data.ipynb. Asegúrate de seguir las instrucciones de carga de datos y ejecutar cada celda de Google Colab para obtener los resultados del análisis.

## Resultados

El análisis resultante mostrará un gráfico con la distribución de los géneros más vistos. Esto te ayudará a identificar tus preferencias de contenido en Netflix.

## Limitaciones

- El *dataset de Kaggle* no está completamente actualizado y no incluye todas las películas y series que actualmente están disponibles en Netflix por lo cual se tiene que hacer una limpieza de campos nulos.
- El *historial de visualización* descargado desde Netflix puede no ser 100% exacto debido a las limitaciones del servicio, como la falta de algunas visualizaciones.

## Contribuciones

Si deseas contribuir a este proyecto, puedes hacer un fork y enviar tus mejoras o sugerencias de cambios. Si tienes un dataset más actualizado o algún código que mejore el análisis, ¡será bienvenido!
