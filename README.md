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
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
  </a>

  <h3 align="center">Arquitectura de Modulo de Analytics en para Sistema SCADA</h3>

  <p align="center">
    An awesome README template to jumpstart your projects!
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
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
  </ol>
</details>



<!-- acerca-del-proyecto -->
## Acerca del Proyecto

El proyecto propuesto se centra en la construcción de un módulo avanzado de análisis para un sistema SCADA (Supervisory Control and Data Acquisition). Este módulo está diseñado para recolectar, procesar y analizar datos provenientes de los sistemas operativos en un ambiente dado. La finalidad es generar información significativa y aportar conocimientos valiosos que permitan predecir la vida útil de los sistemas de mantenimiento. Además, este módulo contribuirá a la toma de decisiones y a la optimización del rendimiento en los procesos de supervisión y control.

#### El Módulo de Análisis: Potenciando la Extracción de Valor a partir de los Datos

-Recopilación de Datos Eficiente: Nuestro módulo se integra directamente con la base de datos centralizada del sistema utilizando protocolos SQL Server. Esta funcionalidad garantiza una recopilación de datos oportuna y precisa, vital para cualquier análisis de alta calidad.

-Procesamiento y Transformación de Datos Robusta: Con la implementación de algoritmos de vanguardia, nuestro módulo transforma los datos brutos en información de alto valor. Las técnicas incorporadas incluyen el filtrado, la normalización y la corrección de datos, así como la generación de métricas a través de cálculos y agregaciones.

-Análisis Estadístico Avanzado: El módulo de análisis ofrece una variedad de técnicas estadísticas, desde análisis de regresión y análisis de series temporales hasta análisis de frecuencia y análisis de correlación. Estas capacidades proporcionan una comprensión profunda del comportamiento del sistema, permitiendo una identificación proactiva de problemas y una mejora continua de la eficiencia.

-Modelado Predictivo Preciso: El módulo cuenta con funcionalidades para desarrollar modelos matemáticos y algoritmos de aprendizaje automático con el fin de predecir el comportamiento futuro del sistema. Estos modelos predictivos facilitan la anticipación de fallas, la detección de condiciones anómalas y la realización de pronósticos de producción.

-Visualización y Reportes Intuitivos: La interfaz gráfica del módulo permite una visualización detallada y personalizable de los resultados del análisis. Los datos se presentan mediante gráficos interactivos, tablas y dashboards ajustables. Además, el módulo es capaz de generar reportes automatizados para facilitar la comunicación y la toma de decisiones basada en datos.

<p align="right">(<a href="#readme-top">Volver al principio</a>)</p>

### Objetivo
Diseñar una arquitectura robusta y eficiente para un Módulo de Análisis que pueda soportar técnicas avanzadas de análisis predictivo con el objetivo de predecir la vida útil de los componentes individuales de los sistemas eléctricos. Esta arquitectura debe facilitar la integración y extracción de datos, el procesamiento y la visualización de los datos, así como la generación de modelos de predicción, permitiendo la futura implementación de un sistema de mantenimiento predictivo más eficiente.

### Alcance
El alcance de este proyecto se centra en el diseño de la arquitectura para un Módulo de Análisis predictivo que se enfocará en los interruptores, transformadores y sistemas de alimentación de un sistema eléctrico. Este diseño de arquitectura incluirá:

-La definición de los métodos de extracción de datos de las fuentes proporcionadas por los sistemas SCADA, que reportan datos en tiempo real como temperaturas, tensión, amperajes, entre otros.
-El diseño de los algoritmos de aprendizaje automático y técnicas estadísticas que se utilizarán para realizar el análisis predictivo de la vida útil de los componentes del sistema eléctrico.
-La identificación y definición de la tecnología que se utilizará para la interfaz de usuario para visualizar los datos y los resultados del análisis. No se incluirán mockups o la implementación de esta interfaz en el alcance de este proyecto.
-La integración con la base de datos del sistema SCADA existente.
-La validación de la arquitectura mediante la metodología ATAM (Architecture Tradeoff Analysis Method).
-Este proyecto no incluirá la implementación de los algoritmos de aprendizaje automático ni de la interfaz de usuario, así como tampoco la formación o el soporte para los usuarios finales. Estos aspectos se considerarán para futuras fases del desarrollo.

### Supuestos


### Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [![Next][Next.js]][Next-url]
* [![React][React.js]][React-url]
* [![Vue][Vue.js]][Vue-url]
* [![Angular][Angular.io]][Angular-url]
* [![Svelte][Svelte.dev]][Svelte-url]
* [![Laravel][Laravel.com]][Laravel-url]
* [![Bootstrap][Bootstrap.com]][Bootstrap-url]
* [![JQuery][JQuery.com]][JQuery-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Minutas de Reunión
<a href="https://docs.google.com/document/d/1Mbfo0DfpvxPdPaXzHG5i1hJdYeJ9zXHfTp3KL9THBFY/edit?usp=sharing" target="_blank">Documento Minutas</a>

<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
