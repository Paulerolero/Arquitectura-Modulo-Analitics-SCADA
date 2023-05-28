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
    <small>_Repositorio para el curso Arquitectura de Sistemas Complejo del magiester en informática de la UBO_</small>
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
        <li><a href="#alcance">Alcance</a>
          <li><a href="#el-módulo-de-análisis-potenciando-la-extracción-de-valor-a-partir-de-los-datos">El Módulo de Análisis</a></li>
        </li>
      </ul>
    </li>
    <li><a href="#requisitos">Requisitos</a>
        <li><a href="#requisitos-funcionales">Requisitos Fuincionales</a></li>
        <li><a href="#requisitos-no-funcionales">Requisitos no Fuincionales</a></li>
    </li>
    <li><a href="#minutas">Minutas de Reunión</a></li>
    <li><a href="#componentes-del-sistema">Componentes del Sistema</a>
        <li><a href="#componentes-del-sistema">Componentes del Sistema</a></li>
    </li>
    <li><a href="#arquitectura">Arquitectura</a>
        <li><a href="#vista-lógica">Vista lógica</a></li>
        <li><a href="#vista-de-procesos">Vista de procesos</a></li>
        <li><a href="#vista-de-desarrollo">Vista de Desarrollo</a></li>
        <li><a href="#vista-física">Vista Física</a></li>
        <li><a href="#vista-de-escenarios">Vista de Escenarios</a></li>
    </li>
    <li><a href="#roadmapa">Roadmap</a>
  </ol>
</details>



<!-- acerca-del-proyecto -->
## Acerca del Proyecto

El proyecto propuesto se centra en la construcción de un módulo avanzado de análisis para un sistema SCADA (Supervisory Control and Data Acquisition). Este módulo está diseñado para recolectar, procesar y analizar datos provenientes de los sistemas operativos en un ambiente dado. La finalidad es generar información significativa y aportar conocimientos valiosos que permitan predecir la vida útil de los sistemas de mantenimiento. Además, este módulo contribuirá a la toma de decisiones y a la optimización del rendimiento en los procesos de supervisión y control.

#### El Módulo de Análisis: Potenciando la Extracción de Valor a partir de los Datos

- Recopilación de Datos Eficiente: Nuestro módulo se integra directamente con la base de datos centralizada del sistema utilizando protocolos SQL Server. Esta funcionalidad garantiza una recopilación de datos oportuna y precisa, vital para cualquier análisis de alta calidad.

- Procesamiento y Transformación de Datos Robusta: Con la implementación de algoritmos de vanguardia, nuestro módulo transforma los datos brutos en información de alto valor. Las técnicas incorporadas incluyen el filtrado, la normalización y la corrección de datos, así como la generación de métricas a través de cálculos y agregaciones.

- Análisis Estadístico Avanzado: El módulo de análisis ofrece una variedad de técnicas estadísticas, desde análisis de regresión y análisis de series temporales hasta análisis de frecuencia y análisis de correlación. Estas capacidades proporcionan una comprensión profunda del comportamiento del sistema, permitiendo una identificación proactiva de problemas y una mejora continua de la eficiencia.

- Modelado Predictivo Preciso: El módulo cuenta con funcionalidades para desarrollar modelos matemáticos y algoritmos de aprendizaje automático con el fin de predecir el comportamiento futuro del sistema. Estos modelos predictivos facilitan la anticipación de fallas, la detección de condiciones anómalas y la realización de pronósticos de producción.

- Visualización y Reportes Intuitivos: La interfaz gráfica del módulo permite una visualización detallada y personalizable de los resultados del análisis. Los datos se presentan mediante gráficos interactivos, tablas y dashboards ajustables. Además, el módulo es capaz de generar reportes automatizados para facilitar la comunicación y la toma de decisiones basada en datos.

### Objetivo
Diseñar una arquitectura robusta y eficiente para un Módulo de Análisis que pueda soportar técnicas avanzadas de análisis predictivo con el objetivo de predecir la vida útil de los componentes individuales de los sistemas eléctricos. Esta arquitectura debe facilitar la integración y extracción de datos, el procesamiento y la visualización de los datos, así como la generación de modelos de predicción, permitiendo la futura implementación de un sistema de mantenimiento predictivo más eficiente.

### Alcance
Considerando las respuestas a las preguntas sobre la extracción de datos y la decisión entre un data warehouse y un data mart, el alcance del proyecto podría quedar de la siguiente manera:

El proyecto se centrará en diseñar una arquitectura robusta para un Módulo de Análisis que permita la recopilación, procesamiento, análisis y visualización de datos provenientes de los sistemas SCADA. Este módulo se enfocará en la predicción de la vida útil de componentes específicos de los sistemas eléctricos, como interruptores, transformadores y sistemas de alimentación.

La extracción de datos será un componente esencial de la arquitectura, y se desarrollará un mecanismo específico para este propósito. Los datos a extraer incluirán voltajes, amperajes y otros datos relevantes de los sistemas, y se establecerán protocolos para manejar problemas de calidad de datos durante la extracción.

El proyecto también incluirá el diseño de un data warehouse para almacenar y gestionar los datos recopilados. Este data warehouse estará diseñado para soportar el análisis avanzado de datos y la generación de modelos predictivos.

La seguridad y la privacidad de los datos serán una consideración importante en el diseño de la arquitectura, y se establecerán medidas para asegurar que los datos sean accesibles sólo por el sistema.

El proyecto no incluirá la implementación del Módulo de Análisis ni la creación de mockups del sistema. Estas tareas se contemplarán para una fase posterior. Finalmente, se planea una validación de la arquitectura mediante la aplicación de la metodología ATAM (Architecture Tradeoff Analysis Method).

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

## Requisitos

### Requisitos Funcionales
<a href="https://docs.google.com/document/d/1n1icxPZ6yP9V9wLhI1s7oLNpEvhD1sU8nt3Il-ZO1jM/edit?usp=sharing" target="_blank">Detalle de requisitos Funcionales </a>

### Requisitos No Funcionales
<a href="https://docs.google.com/document/d/1WfSEzJ0k1bJRqq1p42pyplcmrlwiRG6v4wzUJE7Gr4c/edit?usp=sharing" target="_blank">Detalle de requisitos No Funcionales</a>

<p align="right">(<a href="#readme-top">Inicio</a>)</p>


## Minutas de Reunión
<a href="https://docs.google.com/document/d/1Mbfo0DfpvxPdPaXzHG5i1hJdYeJ9zXHfTp3KL9THBFY/edit?usp=sharing" target="_blank">Documento Minutas</a>

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

## Componentes del Sistema
A continuación se datallaran los componentes que son parte de la solución

1.- **Sistema de extracción de datos:** Este componente será responsable de extraer datos del sistema SCADA. Esto incluirá la conexión a la base de datos del sistema SCADA, la ejecución de consultas para extraer los datos necesarios y la gestión de la transferencia de estos datos al siguiente componente del sistema. Este componente deberá ser capaz de manejar la extracción de datos de varias tablas relacionadas y de gestionar los datos en tiempo real y los datos históricos.

2.- **Data Warehouse:** Este componente almacenará los datos extraídos del sistema SCADA. Deberá diseñarse de acuerdo con un modelo de estrella o de copo de nieve, según sea apropiado, y deberá ser capaz de soportar las operaciones de análisis y procesamiento necesarias. Esto incluirá la gestión de la estructura de la base de datos, la organización y almacenamiento de los datos y el mantenimiento de los niveles de agregación o desagregación necesarios.

3.- **Procesamiento y Transformación de Datos:** Este componente será responsable de transformar los datos brutos en información significativa. Esto incluirá la limpieza de los datos, la validación, la estandarización, la implementación de un sistema de auditoría, la gestión de los datos faltantes y la revisión continua de los datos.

4.- **Análisis Estadístico y Modelado Predictivo:** Este componente llevará a cabo el análisis de los datos y generará predicciones. Deberá ser capaz de implementar técnicas de análisis estadístico como el análisis de regresión, el análisis de series de tiempo y el análisis de varianza. También deberá ser capaz de implementar modelos predictivos utilizando algoritmos de aprendizaje automático, como la regresión lineal o la regresión de bosques aleatorios.

5.- **Visualización y Generación de Informes:** Este componente será la interfaz de usuario del sistema. Deberá ser capaz de presentar los resultados del análisis de manera clara y útil, a través de gráficos interactivos, tableros de control e informes automatizados. También deberá permitir a los usuarios interactuar con los datos y explorarlos de manera más profunda si lo desean.

## Arquitectura.

![diagrama-41](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/assets/118944406/bd7a2408-55a9-4ff2-b233-fc9012180975)

### Vista lógica
Esta vista describirá cómo el Módulo de Análisis interactúa con los sistemas SCADA para recopilar datos. También detallará cómo se estructuran los datos recopilados y cómo se transforman para su análisis.

### Vista de procesos
 Esta vista se ocupará de cómo se manejarán las tareas concurrentes en el sistema, como la recopilación de datos en tiempo real de los sistemas SCADA y el análisis simultáneo de los datos recopilados.


### Vista de Desarrollo
 Esta vista proporcionará detalles sobre cómo se dividirá el Módulo de Análisis en componentes distintos para manejar tareas como la recopilación de datos, el procesamiento de datos, el análisis de datos y la visualización de datos. También describirá cómo se organizarán estos componentes en el sistema.

### Vista Física
Esta vista se ocupará de cómo se desplegará el Módulo de Análisis en la infraestructura de hardware existente. Describirá cómo los componentes del sistema se mapearán en el hardware y cómo se manejarán las interacciones entre el hardware y el software.

### Vista de Escenarios
Esta vista describirá varios escenarios de uso del Módulo de Análisis. Por ejemplo, podría haber un escenario en el que los datos recopilados de los sistemas SCADA se utilicen para predecir la vida útil de un componente eléctrico específico.

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

## Colaboradores

**Contreras, Sebastian**
- [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/) [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/)

**López, Hernán**
- [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/hernan-logo) [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/HernanLoGo)

  
**Mellado, Osvaldo**
- [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/) [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/)

**Salinas, Paulo**
- [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/) [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/)

<p align="right">(<a href="#readme-top">Inicio</a>)</p>

<!-- ROADMAP 
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish -->

