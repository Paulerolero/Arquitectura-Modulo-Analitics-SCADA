# Arquitectura-Modulo-Analytics-SCADA

<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
  </a>

  <h3 align="center">Arquitectura de Modulo de Analytics en para Sistema SCADA</h3>

  <p align="center">
    <small>Repositorio para el curso Arquitectura de Sistemas Complejo del magiester en informática de la UBO</small>
  </p>
</div>



<!-- tabla-de-contenidos -->
<details>
  <summary>Tabla de Contenidos</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del Proyecto</a>
      <ul>
        <li><a href="#objetivo">Objetivo</a></li>
        <li><a href="#alcance">Alcance</a></li>
        <li><a href="#supuestos">Supuestos</a></li>
      </ul>
    </li>
    <li><a href="#minutas">Minutas de Reunión</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
    <li><a href="#colaboradores">Colaboradores</a></li>Colaboradores
  </ol>
</details>



<!-- acerca-del-proyecto -->
## Acerca del Proyecto

El proyecto propuesto se centra en la construcción de un módulo avanzado de análisis para un sistema SCADA (Supervisory Control and Data Acquisition). Este módulo está diseñado para recolectar, procesar y analizar datos provenientes de los sistemas operativos en un ambiente dado. La finalidad es generar información significativa y aportar conocimientos valiosos que permitan predecir la vida útil de los sistemas de mantenimiento. Además, este módulo contribuirá a la toma de decisiones y a la optimización del rendimiento en los procesos de supervisión y control.

#### El Módulo de Análisis: Potenciando la Extracción de Valor a partir de los Datos

-Recopilación de Datos Eficiente: Nuestro módulo se integra directamente con la base de datos centralizada del sistema utilizando protocolos SQL Server. Esta funcionalidad garantiza una recopilación de datos oportuna y precisa, vital para cualquier análisis de alta calidad.

- Procesamiento y Transformación de Datos Robusta: Con la implementación de algoritmos de vanguardia, nuestro módulo transforma los datos brutos en información de alto valor. Las técnicas incorporadas incluyen el filtrado, la normalización y la corrección de datos, así como la generación de métricas a través de cálculos y agregaciones.

- Análisis Estadístico Avanzado: El módulo de análisis ofrece una variedad de técnicas estadísticas, desde análisis de regresión y análisis de series temporales hasta análisis de frecuencia y análisis de correlación. Estas capacidades proporcionan una comprensión profunda del comportamiento del sistema, permitiendo una identificación proactiva de problemas y una mejora continua de la eficiencia.

- Modelado Predictivo Preciso: El módulo cuenta con funcionalidades para desarrollar modelos matemáticos y algoritmos de aprendizaje automático con el fin de predecir el comportamiento futuro del sistema. Estos modelos predictivos facilitan la anticipación de fallas, la detección de condiciones anómalas y la realización de pronósticos de producción.

- Visualización y Reportes Intuitivos: La interfaz gráfica del módulo permite una visualización detallada y personalizable de los resultados del análisis. Los datos se presentan mediante gráficos interactivos, tablas y dashboards ajustables. Además, el módulo es capaz de generar reportes automatizados para facilitar la comunicación y la toma de decisiones basada en datos.

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

### Objetivo
Diseñar una arquitectura robusta y eficiente para un Módulo de Análisis que pueda soportar técnicas avanzadas de análisis predictivo con el objetivo de predecir la vida útil de los componentes individuales de los sistemas eléctricos. Esta arquitectura debe facilitar la integración y extracción de datos, el procesamiento y la visualización de los datos, así como la generación de modelos de predicción, permitiendo la futura implementación de un sistema de mantenimiento predictivo más eficiente.

### Alcance
Considerando las respuestas a las preguntas sobre la extracción de datos y la decisión entre un data warehouse y un data mart, el alcance del proyecto podría quedar de la siguiente manera:

El proyecto se centrará en diseñar una arquitectura robusta para un Módulo de Análisis que permita la recopilación, procesamiento, análisis y visualización de datos provenientes de los sistemas SCADA. Este módulo se enfocará en la predicción de la vida útil de componentes específicos de los sistemas eléctricos, como interruptores, transformadores y sistemas de alimentación.

La extracción de datos será un componente esencial de la arquitectura, y se desarrollará un mecanismo específico para este propósito. Los datos a extraer incluirán voltajes, amperajes y otros datos relevantes de los sistemas, y se establecerán protocolos para manejar problemas de calidad de datos durante la extracción.

El proyecto también incluirá el diseño de un data warehouse para almacenar y gestionar los datos recopilados. Este data warehouse estará diseñado para soportar el análisis avanzado de datos y la generación de modelos predictivos.

La seguridad y la privacidad de los datos serán una consideración importante en el diseño de la arquitectura, y se establecerán medidas para asegurar que los datos sean accesibles sólo por el sistema.

El proyecto no incluirá la implementación del Módulo de Análisis ni la creación de mockups del sistema. Estas tareas se contemplarán para una fase posterior. Finalmente, se planea una validación de la arquitectura mediante la aplicación de la metodología ATAM (Architecture Tradeoff Analysis Method).

### Supuestos

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

## Minutas de Reunión
<a href="https://docs.google.com/document/d/1Mbfo0DfpvxPdPaXzHG5i1hJdYeJ9zXHfTp3KL9THBFY/edit?usp=sharing" target="_blank">Documento Minutas</a>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Arquitectura

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Vista lógica


### Vista de procesos


### Vista de despliegue


### Vista Física


### Vista Física


## Colaboradores

- Nombre del colaborador 1
  - Email: correo@example.com
  - GitHub: [github.com/usuario1](https://github.com/usuario1)
  - LinkedIn: [linkedin.com/in/usuario1](https://linkedin.com/in/usuario1)

- Nombre del colaborador 2
  - Email: correo2@example.com
  - GitHub: [github.com/usuario2](https://github.com/usuario2)
  - LinkedIn: [linkedin.com/in/usuario2](https://linkedin.com/in/usuario2)
  
- Nombre del colaborador 1
  - Email: correo@example.com
  - GitHub: [github.com/usuario1](https://github.com/usuario1)
  - LinkedIn: [linkedin.com/in/usuario1](https://linkedin.com/in/usuario1)

- Nombre del colaborador 2
  - Email: correo2@example.com
  - GitHub: [github.com/usuario2](https://github.com/usuario2)
  - LinkedIn: [linkedin.com/in/usuario2](https://linkedin.com/in/usuario2)
  - [![LinkedIn](linkedin-icon.png)](https://linkedin.com/in/tu-perfil)

<!-- ROADMAP 
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish -->

