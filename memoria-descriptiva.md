# Memoria Descriptiva

## Procesos de Diseño del DAaaS (Data Analytics as a Service)

Este documento describe los procesos de diseño del servicio DAaaS (Data Analytics as a Service). En particular, se enfoca en la arquitectura, la identificación de fuentes de datos, el proceso de web scraping/crawling, el análisis de datos, y la ejecución de Proofs-of-Concept (PoC) para demostrar la viabilidad del enfoque DAaaS.

### Comprender los Requisitos y Objetivos

Para diseñar el DAaaS, es fundamental comprender los requisitos y objetivos del proyecto. Estos son algunos de los puntos clave que se deben abordar:

- ¿Qué tipo de datos no estructurados se recopilarán y de dónde?
- ¿Cuáles son los objetivos de este proyecto?
- ¿Cuáles son las fuentes, como sitios web o aplicaciones, que proporcionarán estos datos?
- ¿Qué tipo de análisis o procesamiento se realizará en estos datos?
- ¿Cuántos datos se esperan procesar y almacenar?
- ¿Cuántos usuarios finales se espera que utilicen el DAaaS?
- ¿Necesita cumplir con regulaciones de privacidad de datos?
- ¿Tiene permiso para extraer datos de las fuentes identificadas?

### Arquitectura DAaaS

El DAaaS se basa en la siguiente arquitectura:

- **Identificación de Fuentes de Datos:** Se identifican fuentes de datos en sitios web de dominio público. Factores como la legalidad y los términos de servicio de cada sitio se consideran al seleccionar fuentes.

    - Fuentes de datos identificadas:
        - Brooks
        - Asics
        - Nike
        - Runnea

- **Web Scraping/Crawling:** Se utilizan técnicas de web scraping/crawling para extraer datos de las fuentes identificadas. Las técnicas incluyen BeautifulSoup y Scrapy. También se exploran oportunidades adicionales de scraping, como YouTube y Amazon.

- **Análisis de Datos:** Los datos extraídos se limpian y transforman para su posterior análisis. Esto incluye análisis descriptivo de los datos y análisis de correlaciones entre las características de las zapatillas de running.

- **Desarrollo de PoC:** Se diseñan y ejecutan PoCs para demostrar la viabilidad del enfoque DAaaS. Se crean comparadores de zapatillas de running basados en características y comentarios de usuarios.

- **Anexo:** Se revisan otros conjuntos de datos y enlaces, aunque finalmente se decide no utilizarlos debido a motivos como la idoneidad del proyecto y la relevancia de los datos.

### Componentes de la Arquitectura DAaaS

La arquitectura DAaaS se compone de los siguientes elementos:

- **Hadoop para Procesamiento y Análisis de Datos:** Se utiliza Hadoop, junto con Hadoop Distributed File System (HDFS) y Apache MapReduce, para almacenar y procesar datos estáticos, como información de productos y precios.

- **Google Cloud Storage:** Google Cloud Storage se utiliza para almacenar archivos de datos y los datos recopilados por crawlers y scrapers. Es una solución escalable y segura para el almacenamiento en la nube.

- **Servidor Web:** Un servidor web se emplea para alojar la aplicación web. Se pueden utilizar servidores web como Apache o servicios en la nube como Google App Engine o Google Compute Engine.

- **API de Python:** La API de Python permite la interacción con los datos, la realización de análisis y la provisión de resultados a través de endpoints de API. Debe ser capaz de acceder a los datos almacenados en Google Cloud Storage, procesarlos y devolver los resultados necesarios para la aplicación web.

- **Cliente en ReactJS:** Para desarrollar la interfaz de usuario de la aplicación web, se utiliza ReactJS. Esta tecnología es adecuada para la creación de componentes que consumen datos de la API y muestran información de las zapatillas, incluyendo la capacidad de compararlas.

- **Base de Datos Google Cloud SQL:** Google Cloud SQL se emplea para almacenar datos estructurados, información de usuarios y otros datos relacionados con la aplicación.

- **Cloud Functions:** Cloud Functions se utilizan para ejecutar crawlers y scrapers.

## Conclusiones

El diseño del DAaaS se basa en la identificación de fuentes de datos, el uso de técnicas de web scraping/crawling, el análisis de datos, y la demostración de la viabilidad del enfoque mediante PoCs. La arquitectura incluye componentes clave para el almacenamiento, procesamiento y presentación de datos.

Este enfoque busca proporcionar a los usuarios una plataforma de acceso a datos analíticos en el contexto de las zapatillas de running.