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

# Capítulo IV: *Backend Configuration Management*

## *Software Configuration Management*

En esta sección se resume toda la información recopilada y se analizan que pasos se realizarán en el
trayecto del proyecto:

### *Software Development Environment Configuration*

Esta sección recopila y resume toda la información obtenida, y se analizan los próximos pasos a seguir en el desarrollo del proyecto. Se detallan las acciones clave para asegurar un avance alineado con los objetivos establecidos.

- **UXPressia:** Plataforma  colaborativa que nos permitirá crear user personas e integrados con los múltiples mapas para evaluar sus prioridades.

- **Figma:** Herramienta colaborativa que nos permitirá desarrollar Wireframes, Mockups, Wireflows, UsersFlows y Tags. 

- **Mermaid:** Plataforma colaborativa que nos permitirá crear nuestro diagrama de base de datos.

- **PlantUML:** Plataforma que nos permitirá crear diagramas de clases.

- **Webstorm:** IDE que utilizaremos para trabajar con javascript y desarrollar la landing page mobile.

- **IntelliJ IDEA:** IDE que utilizaremos para trabajar con Java y desarrollar el backend.

- **Android Studio/Visual Studio Code:** IDE que utilizaremos para trabajar con Kotlin/Flutter y desarrollar el frontend.

### *Source Code Management*

Este proyecto se desarrolló en torno a cinco ramas principales:

- **Main:** Rama principal del proyecto, que contiene las publicaciones oficiales y actualizadas del mismo.

- **Ramas de integrantes del equipo:** Compuesto por un equipo de 4 miembros, cada integrante de CodeMinds trabajó de manera independiente en sus respectivas asignaciones. Además, se colaboró en conjunto para abordar los puntos que lo requerían.

::: note
Para acceder al flujo del backend, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-Backend)
:::

### *Source Code Style Guide & Conventions*

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


### *Software Deployment Configuration*

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

## *Software Development & Implementation*

### *Sprint 1*

#### *Sprint Planning 1*

#### *Sprint Backlog 1*

En este primer sprint, se estableció como prioridad el desarrollo de funcionalidades clave relacionadas con la landing page, el backend y la aplicación móvil de *Temporaly*. Estas tareas se organizaron en función de User Stories (Historias de Usuario) que representan los requisitos fundamentales para entregar una experiencia de usuario sólida y funcional.

En este Sprint Backlog se detalla los elementos de trabajo (Work Items) asignados a cada Historia de Usuario, así como el esfuerzo estimado en horas, los responsables y el estado de progreso de cada tarea. El enfoque de este sprint ha sido garantizar que tanto la landing page como el backend y las funcionalidades de la aplicación móvil estén bien estructurados y listos para futuras integraciones.

A continuación, se presentan las Historias de Usuario organizadas por áreas de desarrollo:


\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline
\multirow{3}{*}{US38} & \multirow{3}{*}{\parbox[t]{2.5cm}{Descubrimiento intuitivo \vspace{0.5cm}}} & WI01 & Diseño de la estructura HTML y navegación principal para facilitar el descubrimiento intuitivo en la landing page & 6h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI02 & Implementación de los elementos de navegación y estructura responsive & 4h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI03 & Pruebas de usabilidad para navegación y descubrimiento & 2h & Mateo Vílchez & Done \\ \hline
\multirow{2}{*}{US39} & \multirow{2}{*}{\parbox[t]{2.5cm}{Contenido informativo \vspace{0.5cm}}} & WI04 & Redacción de todo el contenido informativo para la landing page & 3h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI05 & Implementación del contenido en la landing page & 2h & Belén Ramos & Done \\ \hline
\multirow{2}{*}{US40} & \multirow{2}{*}{\parbox[t]{2.5cm}{Compatibilidad móvil \vspace{0.5cm}}} & WI06 & Desarrollo del diseño responsive para dispositivos móviles & 4h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI07 & Pruebas de responsividad en diferentes resoluciones & 3h & Belén Ramos & Done \\ \hline
\multirow{2}{*}{US41} & \multirow{2}{*}{\parbox[t]{2.5cm}{Formulario de contacto \vspace{0.5cm}}} & WI08 & Diseño e implementación del formulario de contacto & 5h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI09 & Validación de formulario de contacto & 2h & Mateo Vílchez & Done \\ \hline
\multirow{2}{*}{US42} & \multirow{2}{*}{\parbox[t]{2.5cm}{Contenido multimedia \vspace{0.5cm}}} & WI10 & Integración de imágenes, íconos y secciones visuales multimedia & 3h & Belén Ramos & Done \\ \cline{3-7} 
 &  & WI11 & Optimización de recursos multimedia para tiempos de carga más rápidos & 2h & Mateo Vílchez & Done \\ \hline
US43 & \parbox[t]{2.5cm}{Call-to-action claro \vspace{0.5cm}} & WI12 & Diseño y optimización de los botones de call-to-action (CTA) en la landing page & 3h & Mateo Vílchez & Done \\ \hline
\multirow{3}{*}{US32} & \multirow{3}{*}{\parbox[t]{2.5cm}{RESTful API Registro de usuario \vspace{0.5cm}}} & WI13 & Implementación de la API para el registro de usuario & 6h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI14 & Añadir index para role seed en persistencia & 3h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI15 & Middleware para manejo de excepciones & 4h & Alex Avila & Done \\ \hline
\multirow{2}{*}{US33} & \multirow{2}{*}{\parbox[t]{2.5cm}{RESTful API Inicio de sesión de usuario \vspace{0.5cm}}} & WI16 & Implementación de la API para inicio de sesión & 5h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI17 & Implementación de pipeline de seguridad & 5h & Alex Avila & Done \\ \hline
\multirow{2}{*}{US34} & \multirow{2}{*}{\parbox[t]{2.5cm}{Autenticación basada en token JWT \vspace{0.5cm}}} & WI18 & Implementación de autenticación JWT en backend & 6h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI19 & Configuración inicial de OpenAPI & 5h & Alex Avila & Done \\ \hline
US35 & \parbox[t]{2.5cm}{Recuperación de contraseña \vspace{0.5cm}} & WI20 & Implementación de perfiles en Spring Boot & 4h & Alex Avila & Done \\ \hline
\multirow{3}{*}{US36} & \multirow{3}{*}{\parbox[t]{2.5cm}{RESTful API Creación de sesiones \vspace{0.5cm}}} & WI21 & Implementación de la API para la creación de sesiones & 4h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI22 & Creación de Dockerfile para build y compose & 5h & Alex Avila & Done \\ \cline{3-7} 
 &  & WI23 & Creación de Dockerfile para entorno de desarrollo & 4h & Alex Avila & Done \\ \hline
US37 & \parbox[t]{2.5cm}{Paginación y filtrado de resultados \vspace{0.5cm}} & WI24 & Implementación de la paginación y filtrado & 5h & Alex Avila & In-Process \\ \hline
\multirow{2}{*}{US01} & \multirow{2}{*}{\parbox[t]{2.5cm}{Registro de usuario \vspace{0.5cm}}} & WI025 & Diseño del mockup de la pantalla de registro de usuario & 4h & Abel Ortega & Done \\ \cline{3-7} 
 &  & WI26 & Implementación de la funcionalidad de registro en la app & 6h & Abel Ortega & In Process \\ \hline
\multirow{2}{*}{US02} & \multirow{2}{*}{\parbox[t]{2.5cm}{Confirmación de creación de cuenta \vspace{0.5cm}}} & WI27 & Diseño del correo de confirmación (mockup) & 3h & Abel Ortega & Done \\ \cline{3-7} 
 &  & WI28 & Implementación del inicio de sesión con Google y Facebook & 3h & Abel Ortega & In Process \\ \hline
\multirow{2}{*}{US03} & \multirow{2}{*}{\parbox[t]{2.5cm}{Historial de correos \vspace{0.5cm}}} & WI29 & Diseño del mockup de la interfaz de historial de correos activos e inactivos & 3h & Abel Ortega & Done \\ \cline{3-7} 
 &  & WI30 & Implementación de la visualización del historial de correos & 6h & Abel Ortega & To Do \\ \hline
US04 & \parbox[t]{2.5cm}{Eliminación de cuenta \vspace{0.5cm}} & WI31 & Diseño del mockup de la pantalla de eliminación de cuenta & 2h & Abel Ortega & Done \\ \hline
\multirow{2}{*}{US08} & \multirow{2}{*}{\parbox[t]{2.5cm}{Personalización del dominio de correo \vspace{0.5cm}}} & WI32 & Diseño del mockup para personalización del correo & 3h & Abel Ortega & Done \\ \cline{3-7} 
 &  & WI33 & Implementar la funcionalidad de personalización de correos & 5h & Abel Ortega & To-Do \\ \hline
US10 & \parbox[t]{2.5cm}{Copiar correo temporal al portapapeles \vspace{0.5cm}} & WI34 & Diseño del mockup de la función copiar al portapapeles & 3h & Abel Ortega & Done \\ \hline
US11 & \parbox[t]{2.5cm}{Visualización de correos temporales activos \vspace{0.5cm}} & WI35 & Diseño del mockup para la visualización de correos activos & 3h & Abel Ortega & Done \\ \hline
US12 & \parbox[t]{2.5cm}{Sugerencias automáticas de nombres \vspace{0.5cm}} & WI36 & Diseño del mockup para las sugerencias de nombres & 3h & Abel Ortega & Done \\ \hline
US13 & \parbox[t]{2.5cm}{Proceso de generación rápido y fluido \vspace{0.5cm}} & WI37 & Diseño del mockup del proceso rápido de generación de correos & 3h & Abel Ortega & Done \\ \hline
US14 & \parbox[t]{2.5cm}{Advertencia de expiración de correo temporal \vspace{0.5cm}} & WI38 & Diseño del mockup de la advertencia de expiración de correos & 2h & Abel Ortega & Done \\ \hline
US15 & \parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales \vspace{0.5cm}} & WI39 & Diseño de la bandeja de entrada en el mockup & 3h & Abel Ortega & Done \\ \hline
US16 & \parbox[t]{2.5cm}{Visualización de correos recibidos \vspace{0.5cm}} & WI40 & Diseño del mockup de la interfaz de visualización de correos recibidos & 3h & Abel Ortega & Done \\ \hline
\end{longtable}

\vspace{1cm}

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.


![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)
