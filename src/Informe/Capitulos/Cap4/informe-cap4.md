---
title: "Universidad Peruana de Ciencias Aplicadas - Informe de Trabajo Final"
author: 
  - "Startup: CodeMinds"
  - "Producto: Temporaly"
  - "Profesor: Mayta Guillermo, Jorge Luis"
  - "Integrantes:"
  - "Ortega Huaraca, Abel Angel: U20201B380"
  - "Avila Asto, Alex Ramon: U20221A322"
  - "Vilchez Rios, Mateo Alejandro: U202210059"
  - "Ramos Rios, Belén del Rocio: U202216246"

date: "2024-02"
subject: "Markdown"
keywords: [Markdown, Report]
subtitle: "Aplicaciones para Dispositivos Móviles - SW65 - CC238"
lang: "es"
colorlinks: true
footer-left: "CodeMinds"
titlepage: true
titlepage-text-color: "FFFAFA"
titlepage-color: "DC143C"
titlepage-rule-height: 2
titlepage-rule-color: "FFFAFA"
titlepage-logo: "src/img/Logo/logo-upc.pdf"
logo-width: 30mm
book: true
classoption: oneside
code-block-font-size: \scriptsize
header-includes:
- |
  ```{=latex} 
  \usepackage{awesomebox}
  \usepackage{fontawesome5}
  \usepackage{tcolorbox}
  \usepackage{graphicx}
  \usepackage{parskip}
  \usepackage{xcolor}
  \usepackage{float} 
  \usepackage{longtable}
  \usepackage{array}
  \usepackage{lscape}
  \usepackage{multirow}
  \usepackage{longtable}
  \usepackage{geometry}
  \usepackage{booktabs}
 
  \newtcolorbox{info-box}{colback=cyan!5!white,arc=0pt,outer arc=0pt,colframe=cyan!60!black}
  \newtcolorbox{error-box}{colback=red!5!white,arc=0pt,outer arc=0pt,colframe=red!75!black}
  \newtcolorbox{norm-box}{colback=gray!5!white,arc=0pt,outer arc=0pt,colframe=gray!60!black}
  \newtcolorbox{warn-box}{colback=orange!5!white,arc=0pt,outer arc=0pt,colframe=orange!80!black}
  \newtcolorbox{attn-box}{colback=green!5!white,arc=0pt,outer arc=0pt,colframe=green!75!black}
  \newtcolorbox{code-box}{colback=pink!5!white,arc=0pt,outer arc=0pt,colframe=pink!80!black}
  \newtcolorbox{learn-box}{colback=blue!5!white,arc=0pt,outer arc=0pt,colframe=blue!40!black,title=\textbf{Objectives:}}
  \newtcolorbox{scenario-box}{colback=orange!5!white,arc=0pt,outer arc=0pt,colframe=orange!80!black,title=\textbf{Scenario:}}
  \newtcolorbox{outline-box}{colback=cyan!5!white,arc=0pt,outer arc=0pt,colframe=cyan!60!black,title=\textbf{Outline:}}
  \newtcolorbox{prereqs-box}{colback=red!5!white,arc=0pt,outer arc=0pt,colframe=red!60!black,title=\textbf{Prerequisites:}}
  \newtcolorbox{labtime-box}{colback=yellow!5!white,arc=0pt,outer arc=0pt,colframe=yellow!60!black,title=\textbf{Lab:}}
  \newcommand{\pandocbounded}[1]{#1} 
  ```
pandoc-latex-environment:
  tcolorbox: [box]
  info-box: [info]
  error-box: [error]
  norm-box: [norm]
  warn-box: [warn]
  attn-box: [attn]
  code-box: [code]
  learn-box: [learn]
  scenario-box: [scenario]
  outline-box: [outline]
  prereqs-box: [prereqs]
  labtime-box: [labtime]
  noteblock: [note]
  tipblock: [tip]
  warningblock: [warning]
  cautionblock: [caution]
  importantblock: [important]
---

# Capítulo IV: **Backend Configuration Management**

## ***Software Configuration Management***

En esta sección se resume toda la información recopilada y se analizan que pasos se realizarán en el
trayecto del proyecto:

### ***Software Development Environment Configuration***

Esta sección recopila y resume toda la información obtenida, y se analizan los próximos pasos a seguir en el desarrollo del proyecto. Se detallan las acciones clave para asegurar un avance alineado con los objetivos establecidos.

- **UXPressia:** Plataforma  colaborativa que nos permitirá crear user personas e integrados con los múltiples mapas para evaluar sus prioridades.

- **Figma:** Herramienta colaborativa que nos permitirá desarrollar Wireframes, Mockups, Wireflows, UsersFlows y Tags. 

- **Mermaid:** Plataforma colaborativa que nos permitirá crear nuestro diagrama de base de datos.

- **PlantUML:** Plataforma que nos permitirá crear diagramas de clases.

- **Webstorm:** IDE que utilizaremos para trabajar con javascript y desarrollar la landing page mobile.

- **IntelliJ IDEA:** IDE que utilizaremos para trabajar con Java y desarrollar el backend.

- **Android Studio/Visual Studio Code:** IDE que utilizaremos para trabajar con Kotlin/Flutter y desarrollar el frontend.

### ***Source Code Management***

Este proyecto se desarrolló en torno a cinco ramas principales:

- **Main:** Rama principal del proyecto, que contiene las publicaciones oficiales y actualizadas del mismo.

- **Ramas de integrantes del equipo:** Compuesto por un equipo de 4 miembros, cada integrante de CodeMinds trabajó de manera independiente en sus respectivas asignaciones. Además, se colaboró en conjunto para abordar los puntos que lo requerían.

::: note
Para acceder al flujo del backend, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-Backend)
:::

### ***Source Code Style Guide & Conventions***

Para el desarrollo de nuestro proyecto, hemos empleado diversas nomenclaturas, referencias y lenguajes que forman parte de la solución propuesta:

- **Tecnologías:** Para el desarrollo de la aplicación, utilizamos tecnologías como HTML5, CSS y JavaScript.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo, tales como Android Studio, Visual Studio Code, IntelliJ IDEA, WebStorm, GitHub, Git y Figma.

- **Convenciones de idioma:** Adoptamos el uso del inglés como el idioma principal para la escritura de nuestro código, incluyendo la parte correspondiente a la landing page.

- **Lenguaje Gherkin:** Empleamos Gherkin para diseñar las pruebas de cada historia de usuario, siguiendo su estructura básica.

Convenciones de Commits: Nuestro equipo de desarrollo sigue las pautas establecidas por las Convenciones de Commits, adoptando el formato "Conventional Commits" en su versión 1.0.0 (disponible en [URL](https://www.conventionalcommits.org/en/v1.0.0/)). Esto nos permite mantener un historial de cambios claro y comprensible. Nos guiamos por la siguiente estructura:

Donde:

::: code
```
<type>[scope opcional]: <description>
```
:::

- ***type:*** Indica el tipo de modificación realizada, como feat, fix, docs, entre otros.
  
- ***scope:*** Define opcionalmente el alcance del cambio en el código.

- ***description:*** Proporciona un resumen breve y claro de los cambios implementados.

**Convenciones de versionado de lanzamientos**

Para la gestión de versiones, seguimos el estándar "Semantic Versioning 2.0.0". En este formato, las versiones se presentan como (X.Y.Z), con las siguientes interpretaciones:

- **X:** Indica una versión principal que introduce cambios incompatibles con versiones anteriores. Comenzamos en 0 durante la fase de desarrollo inicial y pasamos a 1 cuando la versión está lista para su lanzamiento público. Por convención, los números Y y Z se reinician a 0 cada vez que X aumenta.

- **Y:** Representa una versión secundaria que incluye cambios compatibles con versiones anteriores. También abarca los commits de las "release branches" cuando se agregan nuevas funcionalidades. Al igual que con X, Z se reinicia a 0 cuando Y aumenta.

- **Z:** Refleja parches o correcciones de errores menores. Se integra con commits provenientes de la "rama de corrección" y se fusiona con la rama principal.


### ***Software Deployment Configuration***

::: note
Para acceder al flujo de trabajo, haga click a la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/repositories)
:::

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

Seleccionar el repositorio CodeMinds-LandingPage

![Repositorio de la Landing Page, imagen extraída de Github](src/img/Cap4/git_repo_landing.png)

Abrir, descargar y ejecutar en VSCode o WebsTorm

![Index de la Landing Page, imagen extraída de Github](src/img/Cap4/index_landing.png)


![Web Landing Page - CodeMinds, imagen extraída de Github](src/img/Cap4/desk_landing.png)

![Mobile Landing Page - CodeMinds, imagen extraída de Github](src/img/Cap4/mobile_landing.png)

## ***Software Development & Implementation***
