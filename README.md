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
          <ul>
            <li><a href="#el-módulo-de-análisis-potenciando-la-extracción-de-valor-a-partir-de-los-datos">El Módulo de Análisis</a></li>
          </ul>
        </li>
      </ul>
    </li>
    <li><a href="#requisitos">Requisitos</a>
      <ul>
        <li><a href="#requisitos-funcionales">Requisitos Fuincionales</a></li>
        <li><a href="#requisitos-no-funcionales">Requisitos no Fuincionales</a></li>
      </ul>
    </li>
    <li><a href="#minutas">Minutas de Reunión</a></li>
    <li><a href="#componentes-del-sistema">Componentes del Sistema</a>
      <ul>
        <li><a href="#componentes-del-sistema">Componentes del Sistema</a></li>
      </ul>
    </li>
    <li><a href="#arquitectura">Arquitectura</a>
      <ul>
        <li><a href="#vista-lógica">Vista lógica</a></li>
        <li><a href="#vista-de-procesos">Vista de procesos</a></li>
        <li><a href="#vista-de-desarrollo">Vista de Desarrollo</a></li>
        <li><a href="#vista-física">Vista Física</a></li>
        <li><a href="#vista-de-escenarios">Vista de Escenarios</a></li>
      </ul>
    </li>
    <li><a href="#roadmapa">Roadmap</a>
  </ol>
</details>



<!-- acerca-del-proyecto -->
## Acerca del Proyecto

En el presente documento se presenta una posible solución a la deducción de demanda energética, para el Coordinador Eléctrico Nacional, es de vital importancia ir automatizando sus procesos. Actualmente la estimación de demanda para el día siguiente se realiza de forma manual, en el departamento de estudios y ajustes.

#### INTRODUCCIÓN

Actualmente en Chile tiene una matriz energética instalada de 57.738 GWh, siendo el 53.3% corresponde a energías renovables, el otro 46.7% corresponde a generación a base de carbón y/o Diesel. Cabe destacar que el total de la matriz energética, 19.383 GWh corresponde a energías renovables nos convencionales (ERNC), las cuales corresponden a energía eólica, energía térmica y energía solar.

Cabe destacar, que actualmente Chile es pionero en energías renovables, de lo cual, cada año se van integrando mas proyectos solares y eólicos, aumentando la capacidad energética de Chile.
Para el año 2024 la empresa Colbún va a poner en servicio un parque eólico de 812 Mw instalados, produciendo anualmente 2700 GWh/año, lo cual implica que ese parque puede alimentar de energía eléctrica limpia a cerca de 700.000 hogares.

El ente regulador de todas las empresas de generación y transmisión a nivel nacional es el Coordinador Eléctrico Nacional (CEN). El CEN tiene la capacidad técnica de monitorear a todas las empresas del sector energético, esto gracias a su sistema SCADA que tiene instalado, cabe destacar, que el sistema SCADA instalado en el CEN es unió de los SCADA mas grandes a nivel nacional y regional (Latinoamérica), luego viene la empresa Transelec que tiene el 85% de la transmisión en Chile. Gracias al sistema SCADA el CEN puede monitorear toda la generación y transmisión a nivel nacional, a la vez, puede gestionar la generación, es decir, tiene la facultad de decirle a una empresa generadora cuanto debe general diariamente, suponiendo que una generadora tiene una capacidad instalada de 800 Mw, se le puede limitar la generación al 60% de su capacidad máxima, esto es acorde a las necesidades de la red eléctrica nacional.

### Antecedentes
El Coordinador Eléctrico Nacional ocupa un sistema SCADA, con el cual monitorizan toda la red eléctrica nacional, una de las principales desventajas de estos tipos de sistemas es no poder predecir la demanda energética.

Actualmente para ver el tema de generación diaria, el departamento de estudios y ajustes del CEN, diseñan un plan de generación diaria, este plan contempla la regulación de energía generada por cada central eléctrica (parques eólicos, parques solares, hidroeléctricas, etc.). cabe mencionar, que este plan de generación diaria se realiza de forma manual, en el cual el ingeniero eléctrico debe calcular e ingresar la data correspondiente al software EMS para desarrollar el informe, el cual es enviado a todas las empresas coordinadas.

Uno de los principales inconvenientes es la tardía respuesta por parte del coordinador hacia las empresas de generación, ya que le factor humano retrasa la operación, a la vez, se pueden cometer errores de cálculo.

Si bien los sistemas SCADA cuentan con el modulo EMS, con el cual desarrollan análisis de posibles fallas en el sistema de transmisión, además ver la demandan energética, estos análisis se realizan de forma periódica, pero se hacen de forma manual.

En el mundo SCADA eléctricos no existe algún modulo que sea capaz de predecir el comportamiento de la generación eléctrica, ya sea a mediana o gran escala. Esto es debido a que todo el desarrollo de softwares SCADA está pensado en operación en tiempo real y análisis de falla de forma offline, esto gracias a los sistemas historian, los cuales guardan la data histórica de forma automática. Según la regulación actual, todas las empresas de transmisión y/o generación por regulación deben guardar datos históricos de un año de antigüedad. 

Descrito lo anterior, en el presente trabajo se expone una posible solución en poder implementar un algoritmo de predicción, el cual sea capaz de predecir la demanda diaria, esto con el objetivo de optimizar los tiempos de predicción que realiza el departamento de estudios y ajustes.

El objetivo, como se describe anteriormente, es poder optimizar los tiempos de operación, con lo cual se busca dar respuestas claras y concisas a las empresas de generación, con lo cual se busca bajar los costos de operación y alargar la vida útil de las centrales eléctricas.

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

<p align="right">(<a href="#readme-top">Inicio</a>)</p>


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

## Casos de Uso

### General
![General](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-General.png)
### Obtencion promedio diario SCADA
![CU-01](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-01.png)
### Obtencion de temperatura diaria
![CU-02](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-02.png)
### Obtencion informacion de eventos
![CU-03](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-03.png)
### Generar la demanda de coordinados
![CU-04](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-04.png)
### Guardar la demanda de coordinados
![CU-05](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-05.png)
### Generar informes de demanda electrica
![CU-06](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-06.png)
### Enviar informes por correo electronico
![CU-07](https://github.com/Paulerolero/Arquitectura-Modulo-Analitics-SCADA/blob/main/Diagramas4%2B1/5-Vista%20Escenarios/CU-07.png)

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

<p align="right">(<a href="#readme-top">Inicio</a>)</p>
