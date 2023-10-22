# Proyecto Data Lake para Datos de Zapatillas de Running

Este proyecto tiene como objetivo diseñar, especificar y desplegar un Data Lake para procesar datos no estructurados extraídos mediante técnicas de scraping/crawling de sitios web de dominio público. En particular, se enfoca en recopilar datos relacionados con zapatillas de running.

## Contenido

- [Archivos y Carpetas](#archivos-y-carpetas)
- [Brainstorm y Diseño DAaaS](#brainstorm-y-diseño-daaas)
- [Herramientas de Scraping](#herramientas-de-scraping)
- [Datasets](#datasets)
- [Imágenes de Google Cloud](#imágenes-de-google-cloud)
- [Memoria Descriptiva](#memoria-descriptiva)

## Archivos y Carpetas

- [Brainstorm, el diseño DAaaS y el Diagrama de flujo de datos](https://docs.google.com/document/d/1M1Q_gQkZJdXR44k0C5f7nL7Loerik3JTwy9DgdBsIOI/edit?usp=sharing) del proyecto.
- Los archivos utilizados se encuentran en la carpeta "csv" dentro de la carpeta "data".
- Los archivos JSON fueron obtenidos mediante técnicas de scraping pero no se incluyeron finalmente.
- En la carpeta "data" se muestra el uso de herramientas de scraping.
- La carpeta "dataset" incluye archivos que fueron revisados pero finalmente descartados.
- La carpeta "images_googlecloud" contiene capturas de pantalla de procesos seguidos en la plataforma de Google para crear la aplicación web del comparador de zapatillas. [Explicación de los pasos seguidos en Google Cloud Platgform](https://colab.research.google.com/drive/1nAFmdt4Wmwoc7VzNdYBFdJp6YHfU2jOm?usp=sharing)
- En "memoria-descriptiva.md" se resume el diseño DAaaS seguido en el proyecto.

## Objetivo

El objetivo principal de este proyecto es recopilar y procesar datos relacionados con zapatillas de running a partir de fuentes web de dominio público. Para lograrlo, se diseñó y desplegó un Data Lake que permite almacenar y analizar datos no estructurados, brindando así una plataforma para futuros análisis y aplicaciones relacionadas con zapatillas de running.

## Hadoop

El proceso de configuración y ejecución en Hadoop no se ha completado en este repositorio debido a limitaciones de tiempo. Sin embargo, se ha detallado un plan completo y los pasos específicos en el siguiente documento alojado en Google Colab, que se encuentra en [enlace al documento de Google Colab](https://colab.research.google.com/drive/1bdfkinQLwRmjWefGTs3zCEspDvgbTzov?usp=sharing).


## Scrapping

- [Scraping web runnea](https://colab.research.google.com/drive/1X0Pathnm0i354dAaWRYBtCppdiQWqP99?usp=sharing)
- [Scraping web asics](https://colab.research.google.com/drive/1b7WoZZHC_-rgi0PxajR70vAcyNDHgD2N?usp=sharing)
- [Scraping web nike](https://colab.research.google.com/drive/1Rx9DlkpwKtUY2ZTfNbF3m_YIjVHIntiT?usp=sharing)
- [Scraping web brooks](https://colab.research.google.com/drive/1yD_7XfKP6U4QENaBa_KdS2HSHMdnGhZc?usp=sharing)

Scraping que se intentaron sin éxito:
- [Scraping web bikila](https://colab.research.google.com/drive/1LASY5Al3a_zgZjcq_tqXUjKQIgPFx0M-?usp=sharing)
- [Scrapy Asics](https://colab.research.google.com/drive/12wU6dn1_HEajXDVyEFJww3HJsuo1w6Ck?usp=sharing)
