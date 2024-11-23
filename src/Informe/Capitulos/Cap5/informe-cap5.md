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
  \usepackage{morefloats}
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

# Capítulo V: Product Implementation & Validation

## *Software Configuration Management*

![Imagen extraída de Canva](src/img/Cap5/capitulo5.png)

En esta sección se resume toda la información recopilada y se analizan que pasos se realizarán en el
trayecto del proyecto:

### *Software Development Environment Configuration*

Esta sección recopila y resume toda la información obtenida, y se analizan los próximos pasos a seguir en el desarrollo del proyecto. Se detallan las acciones clave para asegurar un avance alineado con los objetivos establecidos.

- ***UXPressia:*** Plataforma  colaborativa que nos permitirá crear user personas e integrados con los múltiples mapas para evaluar sus prioridades.

- ***Figma:*** Herramienta colaborativa que nos permitirá desarrollar *Wireframes, Mockups, Wireflows, UsersFlows* y *Tags*. 

- ***Mermaid:*** Plataforma colaborativa que nos permitirá crear nuestro diagrama de base de datos.

- ***PlantUML:*** Plataforma que nos permitirá crear diagramas de clases.

- ***Webstorm:*** *IDE* que utilizaremos para trabajar con *javascript* y desarrollar la *landing page mobile*.

- ***IntelliJ IDEA:*** *IDE* que utilizaremos para trabajar con *Java* y desarrollar el *backend*.

- ***Android Studio/Visual Studio Code:*** *IDE* que utilizaremos para trabajar con *Kotlin/Flutter* y desarrollar el *frontend*.

### *Source Code Management*

Este proyecto se desarrolló en torno a cinco ramas principales:

- **Main:** Rama principal del proyecto, que contiene las publicaciones oficiales y actualizadas del mismo.

- **Ramas de integrantes del equipo:** Compuesto por un equipo de 4 miembros, cada integrante de CodeMinds trabajó de manera independiente en sus respectivas asignaciones. Además, se colaboró en conjunto para abordar los puntos que lo requerían.

::: warn
***Temporaly - Auth - Backend***
Para acceder al flujo del *backend*, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-Backend)
:::

::: warn
***Temporaly - Email Generate - Backend***
Para acceder al flujo del *backend*, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-Backend-GenerateMails-Python)
:::

::: warn
***Temporaly - Landing Page***
Para acceder al flujo de la *landing page*, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-LandingPage)
:::

::: warn
***Temporaly - Mobile App***
Para acceder al flujo del *mobile app*, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-MobileApp)
:::

### *Source Code Style Guide & Conventions*

Para el desarrollo de nuestros proyectos, hemos empleado diversas nomenclaturas, referencias y lenguajes que forman parte de la solución propuesta:

::: box
***Landing Page***
:::

- **Tecnologías:** Para el desarrollo de la landing page, utilizamos tecnologías como *HTML5*, *CSS* y *JavaScript*.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo web, tales como: *Visual Studio Code*, *WebStorm*, *GitHub*, *Git* y *Figma*.

- **Convenciones de idioma:** Adoptamos el uso del inglés como el idioma principal para la escritura de nuestro código. Sin embargo, la landing page admite *i18n* para usuarios de habla hispana.

- **Lenguaje Gherkin:** Empleamos Gherkin para diseñar las pruebas de cada historia de usuario, siguiendo su estructura básica.

::: box
***Auth - Backend***
:::

- **Tecnologías:** Para el desarrollo del *backend*, enfocado en el *auth service*, utilizamos tecnologías como *Java*, *Spring Boot* y *Spring Security*.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo *backend*, tales como: *Swagger*, *IntelliJ Idea*, *Github*, *Git* y *Docker*.

- **Convenciones de idioma:** Adoptamos el uso del inglés como el idioma principal para la escritura de nuestro código y la documentación de este en general.

- **Lenguaje Gherkin:** Empleamos Gherkin para diseñar las pruebas de cada historia de usuario, siguiendo su estructura básica.

::: box
***Email Generate - Backend***
:::

- **Tecnologías:** Para el desarrollo del backend, enfocado en el *generate temporary email service*, utilizamos tecnologías como *Python*, *Flask* y *TempMail*.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo backend, tales como: *Flasgger*, *Termux*, *Github*, *Git* y *Vim*.

- **Convenciones de idioma:** Adoptamos el uso del inglés como el idioma principal para la escritura de nuestro código y la documentación de este en general.

- **Lenguaje Gherkin:** Empleamos Gherkin para diseñar las pruebas de cada historia de usuario, siguiendo su estructura básica.

::: box
***Mobile App - Android***
:::

- **Tecnologías:** Para el desarrollo del *mobile app* utilizamos tecnologías como *Kotlin* y *Jetpack Compose* para el desarrollo nativo. Asimismo, para el desarrollo multiplataforma utilizaremos *Flutter*.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo *mobile android* y multiplataforma, tales como: *Android Studio*, *Visual Studio Code*, *Github* y *Git*

- **Convenciones de idioma:** Adoptamos el uso del inglés como el idioma principal para la escritura de nuestro código y la documentación de este en general.

- **Lenguaje Gherkin:** Empleamos *Gherkin* para diseñar las pruebas de cada historia de usuario, siguiendo su estructura básica.

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

\newpage

### *Software Deployment Configuration*

::: warn
Para acceder al flujo de trabajo, haga click a la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/repositories)
:::

**Desplegar** ***Landing Page***

1. Seleccionar el repositorio *CodeMinds-LandingPage*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

2. Abrir, descargar y ejecutar en *VSCode* o *WebsTorm* el archivo index.html

![Repositorio de la Landing Page, imagen extraída de Github](src/img/Cap4/git_repo_landing.png)

3. Visualización de la *Landing Page*

![Web Landing Page - CodeMinds, imagen extraída de Github](src/img/Cap4/desk_landing.png)

![Mobile Landing Page - CodeMinds, imagen extraída de Github](src/img/Cap4/mobile_landing.png)

\newpage

**Desplegar** ***Auth - Backend***

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

2. Abrir, descargar y ejecutar en *Intellij Idea*

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/auth-backend-configuration.png)

3. Visualización de la documentación *Swagger*

![Swagger, imagen extraída de Github](src/img/Cap5/auth-backend-swagger.png)

\newpage

**Desplegar** ***Email Generate - Backend***

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend-GenerateMails-Python*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

2. Abrir, descargar y ejecutar en *VSCode*, *Vim* o su editor de preferencia

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/generate-email-backend-configuration.png)

3. Visualización de la documentación *Flasgger*

![Flasgger, imagen extraída de Github](src/img/Cap5/generate-email-backend-flasgger.png)

\newpage

**Desplegar** ***Mobile App - Temporaly***

1. Seleccionar el repositorio *CodeMinds-Temporaly-MobileApp*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

2. Abrir, descargar y ejecutar en Android Studio 

::: important
 Asegurese de tener la version Android Studio Koala - 2024 - Patch 1 o 2
:::

![Repositorio del Mobile App, imagen extraída de Github](src/img/Cap5/mobile-app-configuration.png)

\newpage

3. Visualización de la aplicación *Temporaly*

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/temporaly-app.png}
    \caption{Flasgger, imagen extraída de Github}
    \label{fig:fimag}
\end{figure}

\newpage

## *Landing Page & Mobile Application Implementation*

### *Sprint 2*

#### *Sprint Planning 2*

\begin{longtable}{|p{5cm}|p{9cm}|}
\hline
\textbf{Sprint Planning Background} & \\ \hline
\endfirsthead
\hline
\textbf{Sprint} & \textbf{Sprint 2} \\ \hline
\endfoot
\hline
\textbf{Date} & 27/09/2024 \\ \hline
\textbf{Time} & 21:00 \\ \hline
\textbf{Location} & Discord Virtual Meeting \\ \hline
\textbf{Prepared By} & Ortega Huaraca, Abel Angel \\ \hline
\textbf{Attendees (to planning meeting)} & Ortega Huaraca, Abel Angel / Avila Asto, Alex Ramon / Vilchez Rios, Mateo Alejandro / Ramos Rios, Belen del Rocio \\ \hline
\textbf{Sprint 2 Review Summary} & Implementación de los User Stories e integración con el Backend (Cap 4 y 5) \\ \hline
\textbf{Sprint 2 Retrospective Summary} & El trabajo se realizó a tiempo, y cada integrante terminó lo que se le encomendó. Asimismo, se trabajó en equipo cuando la situación del proyecto lo requería. \\ \hline
\textbf{Sprint Goal \& User Stories} & Establecer una minidemo de la aplicación Temporaly, en donde se muestre la entrega y cumplimiento de los user stories para este sprint 2 \\ \hline
\textbf{Sprint 2 Velocity} & 1 Sprint cada semanas \\ \hline
\textbf{Sum of Story Points} & 106 \\ \hline
\end{longtable}

\newpage

#### *Sprint Backlog 2*

En este segundo sprint, el foco ha sido completar e integrar funcionalidades críticas dentro de la aplicación móvil de Temporaly, así como afianzar la conexión con el backend. Las historias de usuario incluidas en este sprint cubren tareas relacionadas con la creación y gestión de correos temporales, personalización de dominios, y optimización del proceso de generación y visualización de correos, asegurando que la experiencia de usuario sea intuitiva y eficiente.

Ademas, se ha priorizado garantizar una interacción fluida entre las interfaces móviles desarrolladas en Kotlin y las APIs del backend, permitiendo a los usuarios gestionar correos temporales de manera más personalizada. Además, se incluyeron optimizaciones en la API y el manejo de estado en la aplicación móvil.

A continuación, se detallan las Historias de Usuario, los Work Items (WI) asignados, las horas estimadas, los responsables y el estado de cada tarea.


\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline

\multirow{3}{*}{US38} & \multirow{3}{*}{\parbox[t]{2.5cm}{Descubrimiento intuitivo}} & WI01 & Diseño de la estructura HTML y navegación principal para facilitar el descubrimiento intuitivo en la landing page & 6 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI02 & Implementación de los elementos de navegación y estructura responsive & 4 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI03 & Pruebas de usabilidad para navegación y descubrimiento & 2 & Mateo Vílchez & Done \\ \hline

\multirow{2}{*}{US39} & \multirow{2}{*}{\parbox[t]{2.5cm}{Contenido informativo}} & WI04 & Redacción de todo el contenido informativo para la landing page & 3 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI05 & Implementación del contenido en la landing page & 2 & Belén Ramos & Done \\ \hline

\multirow{2}{*}{US40} & \multirow{2}{*}{\parbox[t]{2.5cm}{Compatibilidad móvil}} & WI06 & Desarrollo del diseño responsive para dispositivos móviles & 4 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI07 & Pruebas de responsividad en diferentes resoluciones & 3 & Belén Ramos & Done \\ \hline

\multirow{2}{*}{US41} & \multirow{2}{*}{\parbox[t]{2.5cm}{Formulario de contacto}} & WI08 & Diseño e implementación del formulario de contacto & 5 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI09 & Validación de formulario de contacto & 2 & Mateo Vílchez & Done \\ \hline

\multirow{2}{*}{US42} & \multirow{2}{*}{\parbox[t]{2.5cm}{Contenido multimedia}} & WI10 & Integración de imágenes, íconos y secciones visuales multimedia & 3 & Belén Ramos & Done \\ \cline{3-7}
 &  & WI11 & Optimización de recursos multimedia para tiempos de carga más rápidos & 2 & Mateo Vílchez & Done \\ \hline

US43 & \parbox[t]{2.5cm}{Call-to-action claro} & WI12 & Diseño y optimización de los botones de call-to-action (CTA) en la landing page & 3 & Mateo Vílchez & Done \\ \hline

\multirow{3}{*}{US32} & \multirow{3}{*}{\parbox[t]{2.5cm}{RESTful API Registro de usuario}} & WI13 & Implementación de la API para el registro de usuario & 6 & Alex Avila & Done \\ \cline{3-7}
 &  & WI14 & Añadir index para role seed en persistencia & 3 & Alex Avila & Done \\ \cline{3-7}
 &  & WI15 & Middleware para manejo de excepciones & 4 & Alex Avila & Done \\ \hline

\newpage

\multirow{2}{*}{US33} & \multirow{2}{*}{\parbox[t]{2.5cm}{RESTful API Inicio de sesión de usuario}} & WI16 & Implementación de la API para inicio de sesión & 5 & Alex Avila & Done \\ \cline{3-7}
 &  & WI17 & Implementación de pipeline de seguridad & 5 & Alex Avila & Done \\ \hline

\multirow{2}{*}{US34} & \multirow{2}{*}{\parbox[t]{2.5cm}{Autenticación basada en token JWT}} & WI18 & Implementación de autenticación JWT en backend & 6 & Alex Avila & Done \\ \cline{3-7}
 &  & WI19 & Configuración inicial de OpenAPI & 5 & Alex Avila & Done \\ \hline

US35 & \parbox[t]{2.5cm}{Recuperación de contraseña} & WI20 & Implementación de perfiles en Spring Boot & 4 & Alex Avila & Done \\ \hline

\multirow{3}{*}{US36} & \multirow{3}{*}{\parbox[t]{2.5cm}{RESTful API Creación de sesiones}} & WI21 & Implementación de la API para la creación de sesiones & 4 & Alex Avila & Done \\ \cline{3-7}
 &  & WI22 & Creación de Dockerfile para build y compose & 5 & Alex Avila & Done \\ \cline{3-7}
 &  & WI23 & Creación de Dockerfile para entorno de desarrollo & 4 & Alex Avila & Done \\ \hline

US37 & \parbox[t]{2.5cm}{Paginación y filtrado de resultados} & WI24 & Implementación de la paginación y filtrado & 5 & Alex Avila & In Process \\ \hline

\multirow{2}{*}{US05} & \multirow{2}{*}{\parbox[t]{2.5cm}{Generación de correo temporal con un clic}} & WI25 & Implementación del recurso POST para generar un correo temporal & 5 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI26 & Implementación del recurso GET para obtener la lista de correos temporales generados & 4 & Abel Ortega & Done \\ \hline

US06 & \parbox[t]{2.5cm}{Duración específica del correo temporal} & WI27 & Implementación del recurso PUT para actualizar la duración específica del correo temporal & 4 & Abel Ortega & Done \\ \hline

US07 & \parbox[t]{2.5cm}{Confirmación visual de creación de correo} & WI28 & Implementación del recurso GET para confirmar la creación visual del correo temporal & 3 & Abel Ortega & Done \\ \hline

US08 & \parbox[t]{2.5cm}{Personalización del dominio del correo temporal} & WI29 & Implementación del recurso PUT para personalizar el dominio del correo temporal & 5 & Abel Ortega & Done \\ \hline

\multirow{4}{*}{US01} & \multirow{4}{*}{\parbox[t]{2.5cm}{Registro de usuario}} & WI30 & Diseño de la pantalla de registro utilizando Jetpack Compose & 6 & Alex Avila & Done \\ \cline{3-7}
 &  & WI02 & Conectar la pantalla de registro con la API & 5 & Alex Avila & Done \\ \cline{3-7}
 &  & WI03 & Implementar validación de campos en la pantalla de registro & 4 & Alex Avila & Done \\ \cline{3-7}
 &  & WI04 & Pruebas de usabilidad para el registro de usuario & 3 & Alex Avila & Done \\ \hline

\multirow{3}{*}{US02} & \multirow{3}{*}{\parbox[t]{2.5cm}{Confirmación de creación de cuenta}} & WI05 & Implementar la funcionalidad de confirmación de cuenta con la API & 5 & Alex Avila & Done \\ \cline{3-7}
 &  & WI31 & Diseño de la pantalla de confirmación de cuenta en Compose & 4 & Alex Avila & Done \\ \cline{3-7}
 &  & WI32 & Pruebas para la confirmación de cuenta & 2 & Alex Avila & Done \\ \hline

\multirow{2}{*}{US03} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificación de cuenta}} & WI33 & Conectar la verificación de cuenta con la API & 4 & Alex Avila & Done \\ \cline{3-7}
 &  & WI34 & Implementar la pantalla de verificación de cuenta & 3 & Alex Avila & Done \\ \hline

\multirow{2}{*}{US04} & \multirow{2}{*}{\parbox[t]{2.5cm}{Inicio de sesión de cuenta}} & WI35 & Crear la pantalla de inicio de sesión en Compose & 5 & Alex Avila & Done \\ \cline{3-7}
 &  & WI36 & Conectar la pantalla de inicio de sesión con la API & 5 & Alex Avila & Done \\ \hline

\multirow{3}{*}{US05} & \multirow{3}{*}{\parbox[t]{2.5cm}{Generación de correo temporal con un clic}} & WI37 & Diseño de la pantalla de generación de correos temporales & 4 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI38 & Implementar la funcionalidad de generación de correos con un clic & 5 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI39 & Pruebas de generación de correos temporales & 2 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US06} & \multirow{2}{*}{\parbox[t]{2.5cm}{Duración específica del correo temporal}} & WI40 & Implementar opción para seleccionar duración del correo & 4 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI41 & Conectar la opción de duración con la API & 4 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US07} & \multirow{2}{*}{\parbox[t]{2.5cm}{Confirmación visual de creación de correo}} & WI42 & Añadir confirmación visual en la pantalla de generación de correos & 3 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI43 & Pruebas de confirmación visual & 2 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US09} & \multirow{2}{*}{\parbox[t]{2.5cm}{Generación múltiple de correos temporales}} & WI44 & Implementar la opción para generar múltiples correos & 4 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI45 & Pruebas para la generación de múltiples correos & 3 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US10} & \multirow{2}{*}{\parbox[t]{2.5cm}{Copiar correo temporal al portapapeles}} & WI46 & Implementar la funcionalidad para copiar correos al portapapeles & 4 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI47 & Pruebas para la funcionalidad de copiar al portapapeles & 2 & Abel Ortega & Done \\ \hline

\multirow{3}{*}{US11} & \multirow{3}{*}{\parbox[t]{2.5cm}{Visualización de correos temporales activos}} & WI48 & Diseño de la interfaz de visualización de correos activos & 5 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI49 & Implementación de la funcionalidad de visualización de correos activos & 6 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI50 & Pruebas para la visualización de correos activos & 2 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US13} & \multirow{2}{*}{\parbox[t]{2.5cm}{Proceso de generación rápido y fluido}} & WI51 & Implementar un proceso rápido de generación de correos temporales & 4 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI52 & Pruebas del proceso rápido de generación & 2 & Abel Ortega & Done \\ \hline


\multirow{2}{*}{US15} & \multirow{2}{*}{\parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales}} & WI53 & Implementar la funcionalidad de acceso a la bandeja de entrada & 5 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI54 & Pruebas para el acceso a la bandeja de entrada & 2 & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US16} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos recibidos}} & WI55 & Implementar la funcionalidad de visualización de correos recibidos & 5 & Abel Ortega & Done \\ \cline{3-7}
 &  & WI56 & Pruebas para la visualización de correos recibidos & 2 & Abel Ortega & Done \\ \hline

\multirow{9}{*}{US32} & \multirow{9}{*}{\parbox[t]{2.5cm}{Manejo de consentimiento de usuario}} & WI57 & Implementación del manejo de estado del consentimiento de usuario en la app móvil & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI58 & Implementación de la lógica para mostrar/ocultar mensajes según aceptación del consentimiento & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI59 & Integración de la funcionalidad de "I Agree" con el flujo de consentimiento y su persistencia & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI60 & Implementación de la navegación entre la pantalla de consentimiento y la pantalla principal & 2h & Mateo Vilchez & In Process \\ \cline{3-7}
 &  & WI70 & Implementación del click handler para navegar a la sección completa de "Privacy Policy" & 2h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI71 & Pruebas unitarias para el componente de consentimiento y verificación de aceptación & 3h & Mateo Vilchez & To Do \\ \cline{3-7}
 &  & WI72 & Manejo de estados para permitir o deshabilitar interacciones con botones según el consentimiento & 2h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI73 & Pruebas de usabilidad para asegurar el flujo correcto en la sección de "Privacy Policy" & 2h & Mateo Vilchez & In Process \\ \cline{3-7}
 &  & WI74 & Validación de errores y feedback visual al usuario en caso de fallos en el consentimiento & 3h & Belen Ramos & Done \\ \hline

\end{longtable}

**Gestión del Sprint 2 (Tablero Kanban):**

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.

![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)

\newpage

#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence for Sprint Review*

***Landing US - Gherking***

```gherkin

US38 - Descubrimiento intuitivo

Feature: Descubrimiento intuitivo de la landing page

  As a user
  I want to navigate the landing page easily
  So that I can discover the content intuitively

  Scenario: User navigates the landing page smoothly
    Given the user is on the landing page
    When the user scrolls and clicks on navigation links
    Then the user should be able to access all sections of the page smoothly

  Examples:
    | section             |
    | Home                |
    | Features            |
    | Contact Information |

```


```gherkin

US39 - Contenido informativo

Feature: Contenido informativo en la landing page

  As a user
  I want to find clear and concise information
  So that I understand the purpose of the application

  Scenario: User reads about features and benefits
    Given the user is on the "Features" section of the landing page
    When the user reads through the content provided
    Then the user should understand the main features and benefits of the application

  Examples:
    | content_section   |
    | Application Uses  |
    | User Testimonials |
    | Pricing Options   |

```


```gherkin

US40 - Compatibilidad móvil

Feature: Compatibilidad móvil para la landing page

  As a mobile user
  I want to view the landing page responsively
  So that I can easily navigate on any device

  Scenario: User accesses the landing page on a mobile device
    Given the user opens the landing page on a smartphone
    When the page loads
    Then the content should adjust to fit the screen size without losing functionality

  Examples:
    | device         |
    | Smartphone     |
    | Tablet         |
    | Small Laptop   |

```


```gherkin

US41 - Formulario de contacto

Feature: Formulario de contacto en la landing page

  As a user
  I want to fill out a contact form
  So that I can get in touch with the team

  Scenario: User submits the contact form
    Given the user is on the "Contact" section of the landing page
    When the user fills out all required fields and clicks "Submit"
    Then the form should be successfully sent, and a confirmation message should appear

  Examples:
    | name       | email                  | message         |
    | John Doe   | john@example.com       | Hello!          |
    | Jane Smith | jane_smith@example.com | Need more info  |

```


```gherkin

US42 - Contenido multimedia

Feature: Contenido multimedia en la landing page

  As a user
  I want to see multimedia content like images and videos
  So that I can understand the information visually

  Scenario: User views images and videos on the landing page
    Given the user is navigating through different sections
    When multimedia content (images, videos) is present
    Then the user should be able to view the content clearly and it should load quickly

  Examples:
    | content_type |
    | Images       |
    | Videos       |
    | GIFs         |

```


```gherkin

US43 - Call-to-action claro

Feature: Call-to-action (CTA) en la landing page

  As a user
  I want to find clear CTA buttons
  So that I can take actions like sign-up or contact easily

  Scenario: User clicks on CTA buttons
    Given the user is on the landing page
    When the user sees a CTA button like "Sign Up Now"
    Then the button should be prominently displayed and redirect to the correct action page

  Examples:
    | button_text | action           |
    | Sign Up Now | Registration     |
    | Contact Us  | Contact Form     |
    | Learn More  | Features Section |

```

***Frontend US - Gherking***

```gherkin

US01 - Registro de usuario

Feature: Registro de un nuevo usuario
  As a user
  I want to register an account in the app
  So that I can access all its features

  Scenario: Registro exitoso
    Given the user is on the registration page
    When they fill out all required fields with valid information
    And click "Register"
    Then the system should create a new user account
    And display a success message

  Examples:
    | username     | email                | password |
    | user_one     | user1@example.com    | pass123  |
    | user_two     | user2@example.com    | pass456  |

```

```gherkin

US02 - Confirmación de creación de cuenta

Feature: Confirmación del registro de cuenta
  As a user
  I want to receive a confirmation email
  So that I can verify my account

  Scenario: Recepción de correo de confirmación
    Given a user registers successfully
    When the system creates the account
    Then a confirmation email should be sent to the user's email address

  Examples:
    | email                |
    | user1@example.com    |
    | user2@example.com    |

```


```gherkin

US03 - Verificación de cuenta

Feature: Verificación de cuenta por correo
  As a user
  I want to verify my account through email
  So that I can activate my access

  Scenario: Verificar cuenta exitosamente
    Given a user receives a confirmation email
    When they click on the verification link in the email
    Then the system should verify their account and display a success message

  Examples:
    | email                |
    | user1@example.com    |
    | user2@example.com    |

```

```gherkin

US04 - Inicio de sesión de cuenta

Feature: Iniciar sesión en la app
  As a user
  I want to log in to my account
  So that I can access personalized features

  Scenario: Inicio de sesión exitoso
    Given the user is on the login page
    When they provide valid credentials
    Then the system should log the user in and redirect to the dashboard

  Examples:
    | email                | password |
    | user1@example.com    | pass123  |
    | user2@example.com    | pass456  |

```

```gherkin

US05 - Generación de correo temporal con un clic

Feature: Generar correo temporal
  As a user
  I want to create a temporary email with one click
  So that I can use it quickly without hassle

  Scenario: Crear correo temporal
    Given the user is on the email generation page
    When they click the "Generate Email" button
    Then a new temporary email should be generated immediately

  Examples:
    | action        |
    | Generate Email |

```

```gherkin

US06 - Duración específica del correo temporal

Feature: Especificar duración del correo temporal
  As a user
  I want to set how long my temporary email will last
  So that I can control its expiration

  Scenario: Seleccionar duración del correo
    Given the user is creating a temporary email
    When they select a specific duration
    Then the system should set the expiration based on the chosen duration

  Examples:
    | duration  |
    | 10 minutes |
    | 30 minutes |

```

```gherkin

US07 - Confirmación visual de creación de correo

Feature: Confirmación visual de correo temporal
  As a user
  I want to receive visual feedback when my temporary email is created
  So that I can be sure of its creation

  Scenario: Mostrar confirmación
    Given a user generates a temporary email
    When the email is created successfully
    Then the system should display a confirmation message on the screen

  Examples:
    | status    |
    | created   |
    | failed    |

```

```gherkin

US08 - Personalización del dominio del correo temporal

Feature: Cambiar dominio del correo temporal
  As a user
  I want to choose a domain for my temporary email
  So that I can customize its address

  Scenario: Seleccionar dominio personalizado
    Given the user is on the email creation page
    When they choose a domain from the available options
    Then the temporary email should be created with the selected domain

  Examples:
    | domain        |
    | tempmail.com  |
    | example.net   |

```

```gherkin

US09 - Generación múltiple de correos temporales

Feature: Generar varios correos temporales
  As a user
  I want to create multiple temporary emails
  So that I can use different addresses for various purposes

  Scenario: Crear múltiples correos
    Given the user is on the email generation page
    When they click the "Generate Multiple Emails" button
    Then multiple temporary emails should be created

  Examples:
    | action          |
    | Generate Multiple |

```

```gherkin

US10 - Copiar correo temporal al portapapeles

Feature: Copiar correo al portapapeles
  As a user
  I want to copy my temporary email address to the clipboard
  So that I can paste it quickly where needed

  Scenario: Copiar correo al portapapeles
    Given a temporary email is displayed
    When the user clicks "Copy to Clipboard"
    Then the email address should be copied to the clipboard

  Examples:
    | button_text     |
    | Copy to Clipboard |

```

```gherkin

US11 - Visualización de correos temporales activos

Feature: Ver correos temporales activos
  As a user
  I want to see a list of my active temporary emails
  So that I can manage them effectively

  Scenario: Mostrar lista de correos activos
    Given the user has active temporary emails
    When they navigate to the "My Emails" section
    Then the system should display a list of all active temporary emails

  Examples:
    | section_name |
    | My Emails    |

```

```gherkin

US12 - Sugerencias automáticas de nombres

Feature: Sugerencias de nombres para correos temporales
  As a user
  I want the system to suggest names for my temporary emails
  So that I can choose a name quickly

  Scenario: Mostrar sugerencias de nombres
    Given a user is creating a temporary email
    When the system generates name suggestions
    Then the user should be able to select one of the suggested names

  Examples:
    | suggestion   |
    | random_name1 |
    | random_name2 |

```

```gherkin

US13 - Proceso de generación rápido y fluido

Feature: Rápida generación de correos
  As a user
  I want to create temporary emails quickly and smoothly
  So that I can avoid delays

  Scenario: Generar correo rápidamente
    Given a user wants to create a temporary email
    When they start the creation process
    Then the system should complete the email generation quickly

  Examples:
    | action       |
    | Generate Now |

```

```gherkin

US14 - Advertencia de expiración de correo temporal

Feature: Advertencia de expiración
  As a user
  I want to receive a warning before my temporary email expires
  So that I can take action if needed

  Scenario: Mostrar advertencia de expiración
    Given a temporary email is about to expire
    When the expiration time is near
    Then the system should display a warning message to the user

  Examples:
    | time_remaining |
    | 5 minutes      |
    | 1 minute       |

```

```gherkin

US15 - Acceso a bandeja de entrada de correos temporales

Feature: Ver bandeja de entrada de correos temporales
  As a user
  I want to access the inbox of my temporary email
  So that I can read incoming messages

  Scenario: Mostrar bandeja de entrada
    Given the user has an active temporary email
    When they click on the inbox icon
    Then the system should open the inbox view for that email

  Examples:
    | action         |
    | Open Inbox     |

```

```gherkin

US16 - Visualización de correos recibidos

Feature: Ver correos recibidos
  As a user
  I want to see all emails received in my temporary inbox
  So that I can manage my messages

  Scenario: Mostrar correos recibidos
    Given the user is in the inbox view
    When new emails are received

```

```gherkin

US32 - Manejo de consentimiento de usuario

Feature: Consent management for users
  As a user
  I want to give my consent to the platform
  So that I can use the service while agreeing to its policies

  Scenario: Accept user consent
    Given the user is presented with a consent form
    When they click on "I Agree"
    Then the user's consent should be recorded in the system
    And the user should be redirected to the main app page

  Examples:
    | consent_action |
    | I Agree        |
    | Accept Terms   |

```

***Backend US - Gherking***

```gherkin

US32 - RESTful API Registro de usuario

Feature: API de registro de usuario
  As a user
  I want to register to the system via the API
  So that I can have an account

  Scenario: Registro exitoso de un nuevo usuario
    Given a user provides valid registration details
    When the user submits their information to the "/register" endpoint
    Then a new user account should be created
    And the system should respond with status 201

  Examples:
    | email                | password |
    | user1@example.com    | pass123  |
    | user2@example.com    | pass456  |

```

```gherkin

US33 - RESTful API Inicio de sesión de usuario

Feature: API de inicio de sesión
  As a user
  I want to log into the system via the API
  So that I can access my account

  Scenario: Inicio de sesión exitoso
    Given a registered user provides valid credentials
    When the user submits their credentials to the "/login" endpoint
    Then the system should authenticate the user
    And respond with a JWT token and status 200

  Examples:
    | email                | password |
    | user1@example.com    | pass123  |
    | user2@example.com    | pass456  |

```

```gherkin

US34 - Autenticación basada en token JWT

Feature: Token JWT para autenticación
  As a developer
  I want to use JWT tokens
  So that the authentication is secure

  Scenario: Autenticación de usuario con JWT
    Given a user has logged in successfully
    When they access a protected resource
    Then the system should verify the JWT token
    And allow access to the resource if valid

  Examples:
    | token_status |
    | valid        |
    | expired      |

```

```gherkin

US35 - Recuperación de contraseña

Feature: Recuperación de contraseña de usuario
  As a user
  I want to recover my password
  So that I can regain access to my account

  Scenario: Solicitud de recuperación de contraseña
    Given a user has forgotten their password
    When they request a password reset via "/forgot-password"
    Then the system should send a password reset email

  Examples:
    | email                |
    | user1@example.com    |
    | user2@example.com    |

```

```gherkin

US36 - RESTful API Creación de sesiones

Feature: Creación de sesiones en el sistema
  As a user
  I want to create sessions via API
  So that I can interact with the system in a stateful way

  Scenario: Creación de sesión exitosa
    Given a user provides valid session data
    When they submit a request to "/create-session"
    Then the system should create a new session and return status 201

  Examples:
    | session_data     |
    | valid_session    |
    | invalid_session  |

```

```gherkin

US37 - Paginación y filtrado de resultados

Feature: Paginación y filtrado de resultados en API
  As a developer
  I want to paginate and filter results
  So that users can retrieve data efficiently

  Scenario: Paginación de resultados
    Given there are multiple users in the system
    When the user requests page 2 with 10 results per page
    Then the system should return the correct set of results

  Scenario: Filtrado de resultados por rol
    Given users with different roles exist
    When the user filters by role "admin"
    Then only users with the "admin" role should be returned

  Examples:
    | page | results_per_page | role   |
    | 1    | 10               | admin  |
    | 2    | 5                | user   |

```

```gherkin

US05 - Generación de correo temporal con un clic

Feature: Generación de correos temporales
  As a user
  I want to generate a temporary email address with one click
  So that I can use it for short-term purposes

  Scenario: Generar correo temporal
    Given a user is on the email generation page
    When they click on "Generate"
    Then a new temporary email should be created instantly

  Examples:
    | action   |
    | Generate |

```

```gherkin

US06 - Duración específica del correo temporal

Feature: Especificar la duración de correos temporales
  As a user
  I want to specify the duration of my temporary email
  So that the email expires after a set period

  Scenario: Seleccionar duración de expiración personalizada
    Given a user is creating a temporary email
    When they select a duration of 30 minutes
    Then the system should set the email expiration time to 30 minutes

  Examples:
    | duration |
    | 10 min   |
    | 30 min   |

```

```gherkin

US07 - Confirmación visual de creación de correo

Feature: Confirmación visual de correos temporales
  As a user
  I want to see a visual confirmation when my temporary email is created
  So that I know the process was successful

  Scenario: Mostrar confirmación visual
    Given a user generates a temporary email
    When the email is created
    Then the system should display a visual confirmation message

  Examples:
    | status    |
    | created   |
    | failed    |

```

```gherkin

US08 - Personalización del dominio del correo temporal

Feature: Personalización del dominio de correos temporales
  As a user
  I want to personalize the domain of my temporary email
  So that I can use a domain of my choice

  Scenario: Cambiar el dominio del correo
    Given a user is creating a temporary email
    When they select a different domain from a list
    Then the email should be created with the chosen domain

  Examples:
    | domain        |
    | example.com   |
    | tempmail.net  |

```

\newpage

#### *Execution Evidence for Sprint Review*

Durante este primer sprint se realizó la implementación de las screen y la conexion con el backend desde la aplicacion movil.
features:
• Se implementó un sistema de inicio y registro de usuarios.
página.
• Se implemento el sistema de generacion de correos falsos
• Se implemento la vista de correos falsos y los mensajes de inbox.

En las imágenes y videos adjuntos se podrá apreciar de mejor manera los avances mencionados.

**Implementación del sistema de correos falso**

![Backend: Imagen extraída del navegador](src/img/Cap5/cap5_backend_1.png)

\newpage

**Implementacion de las pantallas**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/cap5_app_1.jpeg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:fimag}
\end{figure}

![App movil: Imagen extraída de Android Studio.](src/img/Cap5/cap5_app_2.jpeg)

![App movil: Imagen extraída de Android Studio.](src/img/Cap5/cap5_app_3.jpeg)

![App movil: Imagen extraída de Android Studio.](src/img/Cap5/cap5_app_4.jpeg)

![App movil: Imagen extraída de Android Studio.](src/img/Cap5/cap5_app_5.jpeg)

\newpage

#### *Services Documentation Evidence for Sprint Review*

En esta seccion, se muestra la documentacion de los servicios del *backend* de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken*, *Spring Data* y *Flask*

::: warn
**https://docs.spring.io/spring-boot/index.html**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation1.png)

\newpage

::: warn
**https://docs.spring.io/spring-boot/reference/web/spring-security.html#page-title**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation2.png)

::: warn
**https://www.npmjs.com/package/jsonwebtoken**
:::

![Imagen extraída de NPMjs](src/img/Cap5/documentation3.png)

\newpage

::: warn
**https://spring.io/projects/spring-data-jpa**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation4.png)

::: warn
**https://github.com/flasgger/flasgger**
:::

![Imagen extraída de la documentación de Flasgger](src/img/Cap5/documentation5.png)

\newpage

#### *Software Deployment Evidence for Sprint Review*

**Desplegar** ***Email Generate - Backend***

::: warn
Para acceder al despligue del Backend mediante *Flasgger*, haga click en la [URL](https://deploy-generate-email-temporaly-ldav.vercel.app/apidocs/)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend-GenerateMails-Python*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

2. Abrir, descargar y ejecutar en *VSCode*, *Vim* o su editor de preferencia

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/generate-email-backend-configuration.png)

3. Visualización de la documentación *Flasgger*

![Flasgger, imagen extraída de Github](src/img/Cap5/generate-email-backend-flasgger.png)

\newpage

**Desplegar** ***Mobile App - Temporaly***

::: warn
Para acceder al repositorio del FrontEnd, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-MobileApp)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-MobileApp*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

#### *Team Collaboration Insights during Sprint*

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-2.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-3.png)

\newpage

### *Sprint 3*

#### *Sprint Planning 3*

\begin{longtable}{|p{5cm}|p{9cm}|}
\hline
\textbf{Sprint Planning Background} & \\ \hline
\endfirsthead
\hline
\textbf{Sprint} & \textbf{Sprint 3} \\ \hline
\endfoot
\hline
\textbf{Date} & 18/10/2024 \\ \hline
\textbf{Time} & 21:00 \\ \hline
\textbf{Location} & Discord Virtual Meeting \\ \hline
\textbf{Prepared By} & Ortega Huaraca, Abel Angel \\ \hline
\textbf{Attendees (to planning meeting)} & Ortega Huaraca, Abel Angel / Avila Asto, Alex Ramon / Vilchez Rios, Mateo Alejandro / Ramos Rios, Belen del Rocio \\ \hline
\textbf{Sprint 3 Review Summary} & Aplicaciól de mejora continua (Cap 5) y reimplementación de la aplicación en Flutter \\ \hline
\textbf{Sprint 3 Retrospective Summary} & El trabajo se realizó a tiempo, y cada integrante terminó lo que se le encomendó. Asimismo, se trabajó en equipo cuando la situación del proyecto lo requería. \\ \hline
\textbf{Sprint Goal \& User Stories} & Establecer una minidemo de la aplicación Temporaly, en donde se muestre la entrega y cumplimiento de los user stories para este sprint 3 \\ \hline
\textbf{Sprint 3 Velocity} & 1 Sprint cada semanas \\ \hline
\textbf{Sum of Story Points} & 98 \\ \hline
\end{longtable}

\newpage

#### *Sprint Backlog 3*

En este tercer *sprint*, el objetivo ha sido continuar con la reimplementación de la aplicación móvil Temporaly de *Kotlin* a *Flutter*, manteniendo y mejorando las funcionalidades existentes. Este sprint se enfoca en la implementación de nuevas características clave para optimizar la experiencia de usuario, así como en la integración de la gestión de consentimientos, generación de correos temporales y visualización de correos activos.

Las historias de usuario incluidas en este sprint abarcan tareas críticas relacionadas con la reimplementación de la *UI*, la conexión a la *API* del *backend* y la optimización de la usabilidad en *Flutter*. Se han priorizado funcionalidades que impactan directamente la interacción del usuario con la app, como el registro, la personalización de dominios, y la duración específica de los correos temporales.

A continuación, se detallan las Historias de Usuario, los *Work Items* (WI) asignados, las horas estimadas, los responsables y el estado de cada tarea, destacando la colaboración del equipo en el proceso de reimplementación y pruebas para garantizar la fluidez en las nuevas implementaciones.

\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline

\multirow{4}{*}{US01} & \multirow{4}{*}{\parbox[t]{2.5cm}{Registro de usuario}} & WI01 & Diseño de la pantalla de registro utilizando Flutter, incluyendo inputs de usuario y contraseña & 6h & Alex Avila & Done \\ \cline{3-7}
 &  & WI02 & Implementación de la lógica de validación de campos de usuario y conexión con la API & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI03 & Desarrollo de validaciones en tiempo real para la pantalla de registro (usuario, email) & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI04 & Pruebas de usabilidad en la pantalla de registro en diferentes resoluciones móviles & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US02} & \multirow{3}{*}{\parbox[t]{2.5cm}{Confirmación de creación de cuenta}} & WI05 & Conectar la funcionalidad de confirmación de cuenta con la API para validación de correo & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI06 & Diseño de la pantalla de confirmación de cuenta con mensajes de éxito y error & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI07 & Pruebas de interacción con la API para confirmar la creación de cuenta con códigos de verificación & 2h & Alex Avila & Done \\ \hline

\multirow{2}{*}{US03} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificación de cuenta}} & WI08 & Implementar la pantalla de verificación de cuenta conectada con la API usando Flutter & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI09 & Diseñar un flujo para el reenvío de códigos de verificación en caso de error & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US05} & \multirow{3}{*}{\parbox[t]{2.5cm}{Generación de correo temporal con un click}} & WI12 & Implementar la funcionalidad de generación de correos temporales con un clic, mostrando un correo único & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI13 & Conectar la funcionalidad de generación de correo con la API para persistencia & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI14 & Pruebas de generación de correos temporales en diferentes dispositivos y navegadores & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US06} & \multirow{2}{*}{\parbox[t]{2.5cm}{Duración específica del correo temporal}} & WI15 & Añadir opciones en la UI para que el usuario seleccione la duración del correo generado (10, 30, 60 min) & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI16 & Implementar conexión de la opción de duración con la API para persistencia del tiempo del correo & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US07} & \multirow{2}{*}{\parbox[t]{2.5cm}{Confirmación visual de creación de correo}} & WI17 & Mostrar una confirmación visual clara (alerta o modal) cuando se haya generado un correo temporal & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI18 & Pruebas de confirmación visual en dispositivos móviles y navegadores & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US08} & \multirow{2}{*}{\parbox[t]{2.5cm}{Personalización del dominio de correo temporal}} & WI19 & Implementar un selector de dominio en la pantalla de generación de correo temporal & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI20 & Conectar el selector de dominio personalizado con la API para reflejar la opción en el correo generado & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US09} & \multirow{2}{*}{\parbox[t]{2.5cm}{Generación Múltiple de correos temporales}} & WI21 & Añadir una opción en la UI para generar múltiples correos temporales de manera consecutiva & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI22 & Pruebas para asegurar que la generación de múltiples correos no cause conflictos en la API & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US13} & \multirow{2}{*}{\parbox[t]{2.5cm}{Proceso de generación rápido y fluido}} & WI23 & Optimizar el flujo de generación de correos para reducir el tiempo de carga en la UI & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI24 & Pruebas del flujo de generación rápida en diferentes resoluciones y dispositivos & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US15} & \multirow{3}{*}{\parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales}} & WI25 & Implementar una bandeja de entrada para visualizar correos recibidos, con paginación & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI26 & Conectar la bandeja de entrada con la API para la persistencia de correos recibidos & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI27 & Pruebas de funcionalidad de la bandeja de entrada en Flutter & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US16} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos recibidos}} & WI28 & Reimplementación de la funcionalidad de visualización de correos recibidos a Flutter con formato responsive & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI29 & Pruebas de visualización de correos en Flutter para asegurar un diseño responsive y correcto renderizado & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US17} & \multirow{2}{*}{\parbox[t]{2.5cm}{Notificación de nuevos correos en la bandeja de entrada}} & WI30 & Implementación de notificaciones push para avisar al usuario de la llegada de nuevos correos & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI31 & Pruebas de funcionalidad de notificaciones en diferentes plataformas móviles & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US18} & \multirow{2}{*}{\parbox[t]{2.5cm}{Leer y responder correos temporales}} & WI32 & Añadir funcionalidad para que los usuarios puedan leer y responder correos temporales desde la app & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI33 & Pruebas de funcionalidad de lectura y respuesta de correos en Flutter & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US19} & \multirow{2}{*}{\parbox[t]{2.5cm}{Buscar correos en la bandeja de entrada}} & WI34 & Añadir funcionalidad de búsqueda avanzada de correos por remitente y asunto en la bandeja & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI35 & Pruebas de funcionalidad de búsqueda avanzada de correos en la UI en dispositivos móviles & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US20} & \multirow{2}{*}{\parbox[t]{2.5cm}{Eliminar correos temporales}} & WI36 & Implementar funcionalidad para eliminar correos seleccionados de la bandeja de entrada & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI37 & Pruebas de funcionalidad de eliminación de correos temporales en diferentes dispositivos & 2h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US22} & \multirow{2}{*}{\parbox[t]{2.5cm}{Filtrar correos por fecha o remitente}} & WI38 & Añadir la opción para filtrar correos por fecha o remitente en la bandeja de entrada & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI39 & Pruebas de funcionalidad de filtrado de correos en diferentes dispositivos & 3h & Belen Ramos & Done \\ \hline
 
\multirow{9}{*}{US32} & \multirow{9}{*}{\parbox[t]{2.5cm}{Manejo de consentimiento de usuario}} & WI40 & Reimplementación del manejo de estado del consentimiento de usuario a Flutter & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI41 & Reimplementación de la lógica para mostrar/ocultar mensajes según aceptación del consentimiento & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI42 & Reimplementación de la funcionalidad de "I Agree" con el flujo de consentimiento en Flutter & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI43 & Navegación entre la pantalla de consentimiento y la pantalla principal en Flutter & 2h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI44 & Implementación del click handler para "Privacy Policy" en Flutter & 2h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI45 & Pruebas unitarias para la verificación de aceptación en Flutter & 3h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI46 & Manejo de estados para botones según el consentimiento en Flutter & 2h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI47 & Pruebas de usabilidad del flujo de "Privacy Policy" en Flutter & 2h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI48 & Feedback visual en caso de fallos en el consentimiento en Flutter & 3h & Belen Ramos & Done \\ \hline

\end{longtable}

**Gestión del Sprint 3 (Tablero Kanban):**

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.

![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)

\newpage

#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence for Sprint Review*

***FrontEnd and Backend US - Gherking***

```gherkin

US01 - Registro de usuario

Feature: User Registration

  As a user
  I want to register on the app
  So that I can create an account and access the services

  Scenario: Successful registration
    Given the user is on the registration screen
    When the user enters valid credentials (username, password, email)
    Then the user should be registered successfully and redirected to the login page

  Examples:
    | username   | email               | password   |
    | test_user1 | test1@example.com    | password1  |
    | test_user2 | test2@example.com    | password2  |


```

```gherkin

US02 - Confirmación de creación de cuenta

Feature: Confirmación de cuenta
  As a registered user
  I want to confirm my account via email
  So that I can complete the registration process

  Scenario: Account confirmation via API
    Given the user has received an email with a verification code
    When the user enters the code
    Then the account should be confirmed with a success message

  Examples:
    | verification_code |
    | ABCD1234          |
    | XYZ7890           |

```

```gherkin

US03 - Verificación de cuenta

Feature: Verificación de cuenta
  As a user
  I want to verify my account with a code
  So that I can secure my account

  Scenario: Code re-sent after failure
    Given the user has not received a code
    When the user requests a new verification code
    Then the system should resend the code

  Examples:
    | action             |
    | Resend verification|
    | Contact support    |


```

```gherkin

US05 - Generación de correo temporal con un clic

Feature: Generación de correo temporal
  As a user
  I want to generate a temporary email address with one click
  So that I can use it for quick tasks

  Scenario: Generate a single-use email
    Given the user clicks on “Generate Email”
    Then the app should display a temporary email

  Examples:
    | button_clicks |
    | Single-click   |


```

```gherkin

US06 - Duración específica del correo temporal

Feature: Duración del correo temporal
  As a user
  I want to select the duration of my temporary email
  So that it expires after a set period

  Scenario: Set custom expiration time
    Given the user is on the email generation screen
    When the user selects a duration of 30 minutes
    Then the temporary email should expire in 30 minutes

  Examples:
    | duration |
    | 10 min   |
    | 30 min   |
    | 60 min   |


```

```gherkin

US07 - Confirmación visual de creación de correo

Feature: Confirmación de correo creado
  As a user
  I want to receive a visual confirmation for email generation
  So that I know my email is ready to use

  Scenario: Show confirmation alert
    Given the user generates an email
    Then the app should display a confirmation message

  Examples:
    | alert_type   |
    | Modal        |
    | Notification |


```

```gherkin

US08 - Personalización del dominio de correo temporal

Feature: Personalización del dominio
  As a user
  I want to choose the domain of my temporary email
  So that I can customize my email address

  Scenario: Domain selection
    Given the user is on the email options screen
    When the user selects a domain
    Then the generated email should display the chosen domain

  Examples:
    | domain      |
    | tempmail.com|
    | securemail.co|


```

```gherkin

US09 - Generación Múltiple de correos temporales

Feature: Generación múltiple de correos temporales
  As a user
  I want to generate multiple temporary emails
  So that I can use them for different tasks

  Scenario: Generate multiple emails consecutively
    Given the user is on the email generation screen
    When the user selects the option to generate multiple emails
    Then the app should display a list of temporary emails

  Examples:
    | number_of_emails |
    | 3                |
    | 5                |


```

```gherkin

US13 - Proceso de generación rápido y fluido

Feature: Generación rápida de correos temporales
  As a user
  I want the email generation process to be fast and smooth
  So that I can quickly access my temporary email

  Scenario: Generate email with optimized loading time
    Given the user initiates email generation
    Then the app should display the email within 2 seconds

  Examples:
    | load_time |
    | <2 sec    |
    | 1 sec     |


```

```gherkin

US15 - Acceso a bandeja de entrada de correos temporales

Feature: Acceso a la bandeja de entrada
  As a user
  I want to access my temporary email inbox
  So that I can view received messages

  Scenario: Access email inbox with pagination
    Given the user is viewing the inbox
    When the inbox has more than 10 emails
    Then the app should display paginated results

  Examples:
    | page_size |
    | 10        |
    | 20        |


```

```gherkin

US16 - Visualización de correos recibidos

Feature: Visualización de correos recibidos
  As a user
  I want to view received emails in my temporary inbox
  So that I can read messages sent to my temporary address

  Scenario: Display received emails
    Given the user has received emails
    When the user opens the inbox
    Then the app should list all received emails with the sender and subject

  Examples:
    | sender          | subject           |
    | example@test.com| Welcome to TempMail |
    | service@mail.com| Account Verification|


```

```gherkin

US32 - Manejo de consentimiento de usuario

Feature: Manejo de consentimiento de usuario
  As a user
  I want to provide consent for data usage
  So that I can control my privacy settings

  Scenario: Accept consent
    Given the user is on the consent screen
    When the user clicks "I Agree"
    Then the consent status should be saved and a success message shown

  Examples:
    | consent_action |
    | I Agree        |
    | I Decline      |


```

\newpage

#### *Execution Evidence for Sprint Review*

Durante este primer sprint se comenzo la reimplementacion en flutter, asi mismo se integro el sistema de generacion de correo y historial al backend.

• Se implementó un sistema de limite de correos por usuarios
• Se implemento el sistema de filtro de correo falso.
• Se historial de correos y expiracion de estos.

En las imágenes y videos adjuntos se podrá apreciar de mejor manera los avances mencionados.

**Implementación del sistema de correos falso**

![Backend: Imagen extraída del navegador](src/img/Cap5/temp_back_5_2.png)

\newpage

**Reimplementación en flutter.**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/flutter_cap_5.png}
    \caption{App movil: Imagen extraída de Visual Studio Code}
    \label{fig:rnf1}
\end{figure}

\newpage

#### *Services Documentation Evidence for Sprint Review*

En esta seccion, se muestra la documentacion de los servicios del *backend* de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken*, *Spring Data* y *Flask*

::: warn
**https://docs.spring.io/spring-boot/index.html**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation1.png)

\newpage

::: warn
**https://docs.spring.io/spring-boot/reference/web/spring-security.html#page-title**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation2.png)

::: warn
**https://www.npmjs.com/package/jsonwebtoken**
:::

![Imagen extraída de NPMjs](src/img/Cap5/documentation3.png)

\newpage

::: warn
**https://spring.io/projects/spring-data-jpa**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation4.png)

::: warn
**https://github.com/flasgger/flasgger**
:::

![Imagen extraída de la documentación de Flasgger](src/img/Cap5/documentation5.png)

\newpage

#### *Software Deployment Evidence for Sprint Review*

**Desplegar** ***Temporaly - Backend***

::: warn
Para acceder al despliegue del Backend de la aplicación, haga click en la [URL](https://temporally-api.ryzeon.me/swagger-ui/index.html)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap5/despliegue-backend-1.png)

2. Abrir, descargar y ejecutar en *IntelliJ IDEA* o su editor de preferencia para *Java*

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/despliegue-backend-2.png)

3. Visualización de la documentación *Swagger*

![Swagger UI, imagen extraída de la API](src/img/Cap5/despliegue-backend-3.png)

\newpage

**Desplegar** ***Mobile App - Temporaly - Flutter Version***

::: warn
Para acceder al repositorio del FrontEnd, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-FlutterApp)
:::

1. Seleccionar el repositorio CodeMinds-Temporaly-FlutterApp

![Organización CodeMinds, imagen extraída de Github](src/img/Cap5/despliegue-backend-1.png)

2. Abrir, descargar y ejecutar en *Visual Studio Code* o su editor de preferencia para *Flutter*

![Repositorio de la aplicación móvil, imagen extraída de Github](src/img/Cap5/despliegue-backend-4.png)

\newpage

3. Visualización de la aplicación

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/flutter_cap_5.png}
    \caption{App movil: Imagen extraída de Visual Studio Code}
    \label{fig:rnf2}
\end{figure}

\newpage

#### *Team Collaboration Insights During Sprint*

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-2.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-3.png)

\newpage

### *Sprint 4*

#### *Sprint Planning 4*

\begin{longtable}{|p{5cm}|p{9cm}|}
\hline
\textbf{Sprint Planning Background} & \\ \hline
\endfirsthead
\hline
\textbf{Sprint} & \textbf{Sprint 4} \\ \hline
\endfoot
\hline
\textbf{Date} & 01/11/2024 \\ \hline
\textbf{Time} & 21:00 \\ \hline
\textbf{Location} & Discord Virtual Meeting \\ \hline
\textbf{Prepared By} & Ortega Huaraca, Abel Angel \\ \hline
\textbf{Attendees (to planning meeting)} & Ortega Huaraca, Abel Angel / Avila Asto, Alex Ramon / Vilchez Rios, Mateo Alejandro / Ramos Rios, Belen del Rocio \\ \hline
\textbf{Sprint 4 Review Summary} & Aplicaciól de mejora continua (Cap 5) y reimplementación de la aplicación en Flutter \\ \hline
\textbf{Sprint 4 Retrospective Summary} & El trabajo se realizó a tiempo, y cada integrante terminó lo que se le encomendó. Asimismo, se trabajó en equipo cuando la situación del proyecto lo requería. \\ \hline
\textbf{Sprint Goal \& User Stories} & Establecer una minidemo de la aplicación Temporaly, en donde se muestre la entrega y cumplimiento de los user stories para este sprint 4 \\ \hline
\textbf{Sprint 4 Velocity} & 1 Sprint cada semanas \\ \hline
\textbf{Sum of Story Points} & 98 \\ \hline
\end{longtable}

\newpage

#### *Sprint Backlog 4*

En este cuarto *sprint*, el objetivo ha sido continuar con la reimplementación de la aplicación móvil Temporaly de *Kotlin* a *Flutter*, manteniendo y mejorando las funcionalidades existentes. Este sprint se enfoca en la implementación de nuevas características clave para optimizar la experiencia de usuario, así como en la integración de la gestión de consentimientos, generación de correos temporales y visualización de correos activos.

Las historias de usuario incluidas en este sprint abarcan tareas críticas relacionadas con la reimplementación de la *UI*, la conexión a la *API* del *backend* y la optimización de la usabilidad en *Flutter*. Se han priorizado funcionalidades que impactan directamente la interacción del usuario con la app, como el registro, la personalización de dominios, y la duración específica de los correos temporales.

A continuación, se detallan las Historias de Usuario, los *Work Items* (WI) asignados, las horas estimadas, los responsables y el estado de cada tarea, destacando la colaboración del equipo en el proceso de reimplementación y pruebas para garantizar la fluidez en las nuevas implementaciones.

\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline

\multirow{4}{*}{US01} & \multirow{4}{*}{\parbox[t]{2.5cm}{Registro de usuario}} & WI01 & Diseño de la pantalla de registro utilizando Flutter, incluyendo inputs de usuario y contraseña & 6h & Alex Avila & Done \\ \cline{3-7}
 &  & WI02 & Implementación de la lógica de validación de campos de usuario y conexión con la API & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI03 & Desarrollo de validaciones en tiempo real para la pantalla de registro (usuario, email) & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI04 & Pruebas de usabilidad en la pantalla de registro en diferentes resoluciones móviles & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US02} & \multirow{3}{*}{\parbox[t]{2.5cm}{Confirmación de creación de cuenta}} & WI05 & Conectar la funcionalidad de confirmación de cuenta con la API para validación de correo & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI06 & Diseño de la pantalla de confirmación de cuenta con mensajes de éxito y error & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI07 & Pruebas de interacción con la API para confirmar la creación de cuenta con códigos de verificación & 2h & Alex Avila & Done \\ \hline

\multirow{2}{*}{US03} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificación de cuenta}} & WI08 & Implementar la pantalla de verificación de cuenta conectada con la API usando Flutter & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI09 & Diseñar un flujo para el reenvío de códigos de verificación en caso de error & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US05} & \multirow{3}{*}{\parbox[t]{2.5cm}{Generación de correo temporal con un click}} & WI12 & Implementar la funcionalidad de generación de correos temporales con un clic, mostrando un correo único & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI13 & Conectar la funcionalidad de generación de correo con la API para persistencia & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI14 & Pruebas de generación de correos temporales en diferentes dispositivos y navegadores & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US06} & \multirow{2}{*}{\parbox[t]{2.5cm}{Duración específica del correo temporal}} & WI15 & Añadir opciones en la UI para que el usuario seleccione la duración del correo generado (10, 30, 60 min) & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI16 & Implementar conexión de la opción de duración con la API para persistencia del tiempo del correo & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US07} & \multirow{2}{*}{\parbox[t]{2.5cm}{Confirmación visual de creación de correo}} & WI17 & Mostrar una confirmación visual clara (alerta o modal) cuando se haya generado un correo temporal & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI18 & Pruebas de confirmación visual en dispositivos móviles y navegadores & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US08} & \multirow{2}{*}{\parbox[t]{2.5cm}{Personalización del dominio de correo temporal}} & WI19 & Implementar un selector de dominio en la pantalla de generación de correo temporal & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI20 & Conectar el selector de dominio personalizado con la API para reflejar la opción en el correo generado & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US09} & \multirow{2}{*}{\parbox[t]{2.5cm}{Generación Múltiple de correos temporales}} & WI21 & Añadir una opción en la UI para generar múltiples correos temporales de manera consecutiva & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI22 & Pruebas para asegurar que la generación de múltiples correos no cause conflictos en la API & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US13} & \multirow{2}{*}{\parbox[t]{2.5cm}{Proceso de generación rápido y fluido}} & WI23 & Optimizar el flujo de generación de correos para reducir el tiempo de carga en la UI & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI24 & Pruebas del flujo de generación rápida en diferentes resoluciones y dispositivos & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US15} & \multirow{3}{*}{\parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales}} & WI25 & Implementar una bandeja de entrada para visualizar correos recibidos, con paginación & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI26 & Conectar la bandeja de entrada con la API para la persistencia de correos recibidos & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI27 & Pruebas de funcionalidad de la bandeja de entrada en Flutter & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US16} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos recibidos}} & WI28 & Reimplementación de la funcionalidad de visualización de correos recibidos a Flutter con formato responsive & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI29 & Pruebas de visualización de correos en Flutter para asegurar un diseño responsive y correcto renderizado & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US17} & \multirow{2}{*}{\parbox[t]{2.5cm}{Notificación de nuevos correos en la bandeja de entrada}} & WI30 & Implementación de notificaciones push para avisar al usuario de la llegada de nuevos correos & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI31 & Pruebas de funcionalidad de notificaciones en diferentes plataformas móviles & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US18} & \multirow{2}{*}{\parbox[t]{2.5cm}{Leer y responder correos temporales}} & WI32 & Añadir funcionalidad para que los usuarios puedan leer y responder correos temporales desde la app & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI33 & Pruebas de funcionalidad de lectura y respuesta de correos en Flutter & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US19} & \multirow{2}{*}{\parbox[t]{2.5cm}{Buscar correos en la bandeja de entrada}} & WI34 & Añadir funcionalidad de búsqueda avanzada de correos por remitente y asunto en la bandeja & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI35 & Pruebas de funcionalidad de búsqueda avanzada de correos en la UI en dispositivos móviles & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US20} & \multirow{2}{*}{\parbox[t]{2.5cm}{Eliminar correos temporales}} & WI36 & Implementar funcionalidad para eliminar correos seleccionados de la bandeja de entrada & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI37 & Pruebas de funcionalidad de eliminación de correos temporales en diferentes dispositivos & 2h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US22} & \multirow{2}{*}{\parbox[t]{2.5cm}{Filtrar correos por fecha o remitente}} & WI38 & Añadir la opción para filtrar correos por fecha o remitente en la bandeja de entrada & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI39 & Pruebas de funcionalidad de filtrado de correos en diferentes dispositivos & 3h & Belen Ramos & Done \\ \hline
 
\multirow{9}{*}{US32} & \multirow{9}{*}{\parbox[t]{2.5cm}{Manejo de consentimiento de usuario}} & WI40 & Reimplementación del manejo de estado del consentimiento de usuario a Flutter & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI41 & Reimplementación de la lógica para mostrar/ocultar mensajes según aceptación del consentimiento & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI42 & Reimplementación de la funcionalidad de "I Agree" con el flujo de consentimiento en Flutter & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI43 & Navegación entre la pantalla de consentimiento y la pantalla principal en Flutter & 2h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI44 & Implementación del click handler para "Privacy Policy" en Flutter & 2h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI45 & Pruebas unitarias para la verificación de aceptación en Flutter & 3h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI46 & Manejo de estados para botones según el consentimiento en Flutter & 2h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI47 & Pruebas de usabilidad del flujo de "Privacy Policy" en Flutter & 2h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI48 & Feedback visual en caso de fallos en el consentimiento en Flutter & 3h & Belen Ramos & Done \\ \hline

\end{longtable}

**Gestión del Sprint 4 (Tablero Kanban):**

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.

![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)

\newpage

#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence for Sprint Review*

***FrontEnd and Backend US - Gherking***

```gherkin

US01 - Registro de usuario

Feature: User Registration

  As a user
  I want to register on the app
  So that I can create an account and access the services

  Scenario: Successful registration
    Given the user is on the registration screen
    When the user enters valid credentials (username, password, email)
    Then the user should be registered successfully and redirected to the login page

  Examples:
    | username   | email               | password   |
    | test_user1 | test1@example.com    | password1  |
    | test_user2 | test2@example.com    | password2  |


```

```gherkin

US02 - Confirmación de creación de cuenta

Feature: Confirmación de cuenta
  As a registered user
  I want to confirm my account via email
  So that I can complete the registration process

  Scenario: Account confirmation via API
    Given the user has received an email with a verification code
    When the user enters the code
    Then the account should be confirmed with a success message

  Examples:
    | verification_code |
    | ABCD1234          |
    | XYZ7890           |

```

```gherkin

US03 - Verificación de cuenta

Feature: Verificación de cuenta
  As a user
  I want to verify my account with a code
  So that I can secure my account

  Scenario: Code re-sent after failure
    Given the user has not received a code
    When the user requests a new verification code
    Then the system should resend the code

  Examples:
    | action             |
    | Resend verification|
    | Contact support    |


```

```gherkin

US05 - Generación de correo temporal con un clic

Feature: Generación de correo temporal
  As a user
  I want to generate a temporary email address with one click
  So that I can use it for quick tasks

  Scenario: Generate a single-use email
    Given the user clicks on “Generate Email”
    Then the app should display a temporary email

  Examples:
    | button_clicks |
    | Single-click   |


```

```gherkin

US06 - Duración específica del correo temporal

Feature: Duración del correo temporal
  As a user
  I want to select the duration of my temporary email
  So that it expires after a set period

  Scenario: Set custom expiration time
    Given the user is on the email generation screen
    When the user selects a duration of 30 minutes
    Then the temporary email should expire in 30 minutes

  Examples:
    | duration |
    | 10 min   |
    | 30 min   |
    | 60 min   |


```

```gherkin

US07 - Confirmación visual de creación de correo

Feature: Confirmación de correo creado
  As a user
  I want to receive a visual confirmation for email generation
  So that I know my email is ready to use

  Scenario: Show confirmation alert
    Given the user generates an email
    Then the app should display a confirmation message

  Examples:
    | alert_type   |
    | Modal        |
    | Notification |


```

```gherkin

US08 - Personalización del dominio de correo temporal

Feature: Personalización del dominio
  As a user
  I want to choose the domain of my temporary email
  So that I can customize my email address

  Scenario: Domain selection
    Given the user is on the email options screen
    When the user selects a domain
    Then the generated email should display the chosen domain

  Examples:
    | domain      |
    | tempmail.com|
    | securemail.co|


```

```gherkin

US09 - Generación Múltiple de correos temporales

Feature: Generación múltiple de correos temporales
  As a user
  I want to generate multiple temporary emails
  So that I can use them for different tasks

  Scenario: Generate multiple emails consecutively
    Given the user is on the email generation screen
    When the user selects the option to generate multiple emails
    Then the app should display a list of temporary emails

  Examples:
    | number_of_emails |
    | 3                |
    | 5                |


```

```gherkin

US13 - Proceso de generación rápido y fluido

Feature: Generación rápida de correos temporales
  As a user
  I want the email generation process to be fast and smooth
  So that I can quickly access my temporary email

  Scenario: Generate email with optimized loading time
    Given the user initiates email generation
    Then the app should display the email within 2 seconds

  Examples:
    | load_time |
    | <2 sec    |
    | 1 sec     |


```

```gherkin

US15 - Acceso a bandeja de entrada de correos temporales

Feature: Acceso a la bandeja de entrada
  As a user
  I want to access my temporary email inbox
  So that I can view received messages

  Scenario: Access email inbox with pagination
    Given the user is viewing the inbox
    When the inbox has more than 10 emails
    Then the app should display paginated results

  Examples:
    | page_size |
    | 10        |
    | 20        |


```

```gherkin

US16 - Visualización de correos recibidos

Feature: Visualización de correos recibidos
  As a user
  I want to view received emails in my temporary inbox
  So that I can read messages sent to my temporary address

  Scenario: Display received emails
    Given the user has received emails
    When the user opens the inbox
    Then the app should list all received emails with the sender and subject

  Examples:
    | sender          | subject           |
    | example@test.com| Welcome to TempMail |
    | service@mail.com| Account Verification|


```

```gherkin

US32 - Manejo de consentimiento de usuario

Feature: Manejo de consentimiento de usuario
  As a user
  I want to provide consent for data usage
  So that I can control my privacy settings

  Scenario: Accept consent
    Given the user is on the consent screen
    When the user clicks "I Agree"
    Then the consent status should be saved and a success message shown

  Examples:
    | consent_action |
    | I Agree        |
    | I Decline      |


```

\newpage

#### *Execution Evidence for Sprint Review*

Durante este cuarto sprint se comenzo la reimplementacion en flutter, asi mismo se integro el sistema de generacion de correo y historial al backend.

• Se implementó un sistema de limite de correos por usuarios
• Se implemento el sistema de filtro de correo falso.
• Se historial de correos y expiracion de estos.

En las imágenes y videos adjuntos se podrá apreciar de mejor manera los avances mencionados.

**Implementación del sistema de correos falso**

![Backend: Imagen extraída del navegador](src/img/Cap5/temp_back_5_2.png)

\newpage

**Reimplementación en flutter.**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/flutter_cap_5.png}
    \caption{App movil: Imagen extraída de Visual Studio Code}
    \label{fig:rnf1}
\end{figure}

\newpage

#### *Services Documentation Evidence for Sprint Review*

En esta seccion, se muestra la documentacion de los servicios del *backend* de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken*, *Spring Data* y *Flask*

::: warn
**https://docs.spring.io/spring-boot/index.html**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation1.png)

\newpage

::: warn
**https://docs.spring.io/spring-boot/reference/web/spring-security.html#page-title**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation2.png)

::: warn
**https://www.npmjs.com/package/jsonwebtoken**
:::

![Imagen extraída de NPMjs](src/img/Cap5/documentation3.png)

\newpage

::: warn
**https://spring.io/projects/spring-data-jpa**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation4.png)

::: warn
**https://github.com/flasgger/flasgger**
:::

![Imagen extraída de la documentación de Flasgger](src/img/Cap5/documentation5.png)

\newpage

#### *Software Deployment Evidence for Sprint Review*

**Desplegar** ***Temporaly - Backend***

::: warn
Para acceder al despliegue del Backend de la aplicación, haga click en la [URL](https://temporally-api.ryzeon.me/swagger-ui/index.html)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap5/despliegue-backend-1.png)

2. Abrir, descargar y ejecutar en *IntelliJ IDEA* o su editor de preferencia para *Java*

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/despliegue-backend-2.png)

3. Visualización de la documentación *Swagger*

![Swagger UI, imagen extraída de la API](src/img/Cap5/despliegue-backend-3.png)

\newpage

**Desplegar** ***Mobile App - Temporaly - Flutter Version***

::: warn
Para acceder al repositorio del FrontEnd, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-FlutterApp)
:::

1. Seleccionar el repositorio CodeMinds-Temporaly-FlutterApp

![Organización CodeMinds, imagen extraída de Github](src/img/Cap5/despliegue-backend-1.png)

2. Abrir, descargar y ejecutar en *Visual Studio Code* o su editor de preferencia para *Flutter*

![Repositorio de la aplicación móvil, imagen extraída de Github](src/img/Cap5/despliegue-backend-4.png)

\newpage

3. Visualización de la aplicación

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/flutter_cap_5.png}
    \caption{App movil: Imagen extraída de Visual Studio Code}
    \label{fig:rnf2}
\end{figure}

\newpage

#### *Team Collaboration Insights During Sprint*

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-2.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-3.png)

\newpage

### *Sprint 5*

#### *Sprint Planning 5*

\begin{longtable}{|p{5cm}|p{9cm}|}
\hline
\textbf{Sprint Planning Background} & \\ \hline
\endfirsthead
\hline
\textbf{Sprint} & \textbf{Sprint 4} \\ \hline
\endfoot
\hline
\textbf{Date} & 11/11/2024 \\ \hline
\textbf{Time} & 21:00 \\ \hline
\textbf{Location} & Discord Virtual Meeting \\ \hline
\textbf{Prepared By} & Ortega Huaraca, Abel Angel \\ \hline
\textbf{Attendees (to planning meeting)} & Ortega Huaraca, Abel Angel / Avila Asto, Alex Ramon / Vilchez Rios, Mateo Alejandro / Ramos Rios, Belen del Rocio \\ \hline
\textbf{Sprint 5 Review Summary} & Consolidación de funcionalidades clave y mejoras de rendimiento en Kotlin \\ \hline
\textbf{Sprint 5 Retrospective Summary} & Trabajo coordinado y mayor optimización en la entrega de tareas críticas. Aumento en la velocidad del equipo. \\ \hline
\textbf{Sprint Goal \& User Stories} & Finalizar integración de todas las funcionalidades clave, asegurar pruebas finales de QA y preparar la app para producción. \\ \hline
\textbf{Sprint 5 Velocity} & 1 Sprint cada semanas \\ \hline
\textbf{Sum of Story Points} & 120 \\ \hline
\end{longtable}

\newpage

#### *Sprint Backlog 5*

En este quinto y último *sprint*, el objetivo principal ha sido completar todas las funcionalidades pendientes de la aplicación móvil *Temporaly* en *Flutter*, incluyendo la implementación de mejoras y optimizaciones clave. Este sprint se ha centrado en finalizar tareas relacionadas con la gestión de correos temporales, la bandeja de entrada, y el historial de sesiones, garantizando que todas las funcionalidades estén completamente operativas y probadas.

Las historias de usuario incluidas en este sprint abarcan tareas críticas para la experiencia del usuario, como el acceso y manejo de correos temporales, notificaciones, filtros avanzados, y funcionalidades relacionadas con el historial. También se ha trabajado en pruebas exhaustivas para asegurar la calidad del producto final, priorizando aspectos como la integración de la API, la estabilidad de las nuevas características y la usabilidad en diferentes dispositivos.

A continuación, se detallan las Historias de Usuario, los *Work Items* (WI) asignados, las horas estimadas, los responsables y el estado de cada tarea, resaltando la colaboración del equipo en este cierre del proyecto:


\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline

\multirow{3}{*}{US15} & \multirow{3}{*}{\parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales}} & WI01 & Crear la pantalla para visualizar la bandeja de entrada con paginación y diseño responsive & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI02 & Conectar la funcionalidad de acceso a la bandeja con la API para obtener datos actualizados & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI03 & Pruebas de funcionalidad para acceso y navegación en la bandeja de entrada & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US16} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos recibidos}} & WI04 & Diseñar y construir la pantalla de correos recibidos con formato adecuado & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI05 & Implementar conexión con la API para actualizar los correos recibidos en tiempo real & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US17} & \multirow{2}{*}{\parbox[t]{2.5cm}{Notificación de nuevos correos}} & WI06 & Implementar notificaciones push para avisar al usuario sobre nuevos correos & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI07 & Pruebas para validar el envío y recepción de notificaciones en dispositivos móviles & 3h & Abel Ortega & Done \\ \hline

\multirow{3}{*}{US18} & \multirow{3}{*}{\parbox[t]{2.5cm}{Leer y responder correos temporales}} & WI08 & Diseñar la pantalla para lectura y respuesta de correos, con editor de texto básico & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI09 & Implementar funcionalidad para responder correos directamente desde la bandeja & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI10 & Pruebas de funcionalidad para lectura y respuesta en dispositivos móviles & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US19} & \multirow{2}{*}{\parbox[t]{2.5cm}{Buscar correos en la bandeja de entrada}} & WI11 & Crear un buscador avanzado para localizar correos por remitente o asunto & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI12 & Pruebas de funcionalidad de búsqueda en distintos escenarios y casos de uso & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US20} & \multirow{2}{*}{\parbox[t]{2.5cm}{Eliminar correos temporales}} & WI13 & Implementar funcionalidad para eliminar correos seleccionados de la bandeja de entrada & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI14 & Pruebas de funcionalidad de eliminación de correos temporales seleccionados & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US21} & \multirow{2}{*}{\parbox[t]{2.5cm}{Marcar correos como importantes}} & WI15 & Diseñar funcionalidad para marcar correos importantes con una estrella o marcador visual & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI16 & Pruebas de funcionalidad para verificar el correcto marcado y persistencia en la API & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US22} & \multirow{2}{*}{\parbox[t]{2.5cm}{Filtrar correos por fecha o remitente}} & WI17 & Crear filtros avanzados para clasificar correos por fecha y remitente desde la bandeja & 4h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI18 & Pruebas para validar los filtros en diferentes combinaciones y dispositivos & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US23} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificar correos temporales usados recientemente}} & WI19 & Implementar sección para mostrar correos usados recientemente con etiquetas temporales & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI20 & Pruebas para verificar el correcto manejo de la lista de correos usados & 3h & Alex Avila & Done \\ \hline

\multirow{2}{*}{US24} & \multirow{2}{*}{\parbox[t]{2.5cm}{Adjuntar archivos en respuestas}} & WI21 & Diseñar funcionalidad para adjuntar archivos a respuestas de correos, con validaciones & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI22 & Pruebas para verificar la subida y manejo de archivos adjuntos & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US25} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización del historial de sesiones}} & WI23 & Diseñar la pantalla para mostrar un historial detallado de sesiones previas & 4h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI24 & Implementar conexión con la API para obtener datos del historial en tiempo real & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US26} & \multirow{2}{*}{\parbox[t]{2.5cm}{Buscar en historial de sesiones}} & WI25 & Crear funcionalidad de búsqueda avanzada para localizar sesiones específicas por fecha o remitente & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI26 & Pruebas de funcionalidad para asegurar la precisión de los resultados de búsqueda & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US27} & \multirow{2}{*}{\parbox[t]{2.5cm}{Acceso detallado a correos temporales anteriores}} & WI27 & Implementar pantalla con detalles de correos anteriores, incluyendo metadatos & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI28 & Pruebas para validar el correcto acceso y presentación de correos del historial & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US28} & \multirow{2}{*}{\parbox[t]{2.5cm}{Eliminar entradas del historial de sesiones}} & WI29 & Implementar funcionalidad para eliminar entradas seleccionadas del historial de sesiones & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI30 & Pruebas para validar la eliminación de entradas en distintos casos de uso & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US29} & \multirow{2}{*}{\parbox[t]{2.5cm}{Exportar el historial de sesiones}} & WI31 & Diseñar una funcionalidad para exportar el historial de sesiones a formatos como CSV o PDF & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI32 & Pruebas para asegurar la correcta exportación del historial en diferentes formatos & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US30} & \multirow{2}{*}{\parbox[t]{2.5cm}{Restaurar correos temporales del historial}} & WI33 & Diseñar funcionalidad para restaurar correos seleccionados desde el historial & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI34 & Pruebas para verificar la restauración en diferentes casos de uso & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US31} & \multirow{2}{*}{\parbox[t]{2.5cm}{Filtrar historial por fecha}} & WI35 & Implementar filtros avanzados por fecha y remitente en la pantalla de historial & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI36 & Pruebas de funcionalidad de los filtros en diferentes combinaciones & 3h & Abel Ortega & Done \\ \hline

\end{longtable}



#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence for Sprint Review*

***EP03 (Access and Management of an Inbox)***

```gherkin
US15 - Access to Temporary Email Inbox

Feature: Access temporary email inbox
  As a user
  I want to access an inbox for my temporary emails
  So that I can view and manage received emails securely

  Scenario: Access the temporary email inbox
    Given the user has generated a temporary email
    When the user navigates to the inbox
    Then the system should display all emails associated with the temporary address

```

```gherkin
US16 - View Received Emails

Feature: View received temporary emails
  As a user
  I want to see the emails received in my temporary inbox
  So that I can read them without revealing my real email

  Scenario: Display received emails
    Given the user has received emails in the temporary inbox
    When the user opens the inbox
    Then the system should show a list of all received emails

```

```gherkin
US17 - Notification for New Emails

Feature: Notify user about new emails
  As a user
  I want to receive notifications when new emails arrive in my temporary inbox
  So that I am informed promptly of any updates

  Scenario: Notify on email reception
    Given the user has enabled notifications
    When a new email arrives in the inbox
    Then the system should send a push notification to the user

```

```gherkin
US18 - Read and Respond to Temporary Emails

Feature: Read and respond to temporary emails
  As a user
  I want to read and reply to emails in my temporary inbox
  So that I can interact with the sender

  Scenario: Read and respond to an email
    Given the user has an email in the temporary inbox
    When the user opens the email and writes a response
    Then the system should send the response from the temporary address

```

```gherkin
US19 - Search Emails in Inbox

Feature: Search emails in the inbox
  As a user
  I want to search emails by sender or subject
  So that I can quickly locate specific emails

  Scenario: Search for an email
    Given the user has multiple emails in the inbox
    When the user searches by sender or subject
    Then the system should filter and display matching emails

```

```gherkin
US20 - Delete Temporary Emails

Feature: Delete emails from the inbox
  As a user
  I want to delete specific emails from my temporary inbox
  So that I can manage my inbox efficiently

  Scenario: Delete an email
    Given the user has selected an email
    When the user confirms the deletion
    Then the system should remove the email from the inbox

```

```gherkin
US21 - Mark Emails as Important

Feature: Mark temporary emails as important
  As a user
  I want to mark specific emails as important
  So that I can easily identify and prioritize them

  Scenario: Mark an email as important
    Given the user has an email in the temporary inbox
    When the user selects the "Mark as Important" option
    Then the system should label the email as important

```

```gherkin
US22 - Filter Emails by Date or Sender

Feature: Filter emails by date or sender
  As a user
  I want to filter emails based on date or sender
  So that I can easily locate specific emails

  Scenario: Filter emails by sender
    Given the user has multiple emails in the inbox
    When the user applies a filter for a specific sender
    Then the system should display only the emails from that sender

  Scenario: Filter emails by date
    Given the user has multiple emails in the inbox
    When the user applies a filter for a specific date range
    Then the system should display only the emails within that range

```

```gherkin
US23 - Verify Recently Used Temporary Emails

Feature: Verify recently used temporary emails
  As a user
  I want to see a list of recently used temporary emails
  So that I can track and manage previously used addresses

  Scenario: View recently used emails
    Given the user has generated multiple temporary emails
    When the user navigates to the history section
    Then the system should display a list of recently used temporary emails

```

```gherkin
US24 - Attach Files to Email Responses

Feature: Attach files to email responses
  As a user
  I want to attach files when replying to emails
  So that I can share necessary documents

  Scenario: Attach a file to a response
    Given the user is replying to an email
    When the user selects a file to attach
    Then the system should include the file in the email response

```

***EP03 (Access and Management of an Inbox)***

```gherkin
US25 - View Session History

Feature: View session history
  As a user
  I want to view the history of my generated temporary emails
  So that I can review emails and sessions I have used in the past

  Scenario: Display session history
    Given the user has generated multiple temporary email sessions
    When the user navigates to the session history section
    Then the system should display a chronological list of all past sessions

```

```gherkin
US26 - Search Session History

Feature: Search within session history
  As a user
  I want to search through my session history
  So that I can quickly find a specific email session

  Scenario: Search for a session by email address
    Given the user has multiple entries in the session history
    When the user enters an email address in the search bar
    Then the system should display only the sessions related to that email

```

```gherkin
US27 - Access Details of a Temporary Email

Feature: Access detailed information of a temporary email session
  As a user
  I want to access details of a specific session
  So that I can retrieve information about my past temporary email usage

  Scenario: View detailed session information
    Given the user is in the session history section
    When the user selects a specific session entry
    Then the system should display details such as email address, creation date, and expiration time

```

```gherkin
US28 - Delete Session History Entries

Feature: Delete entries from session history
  As a user
  I want to delete specific entries from my session history
  So that I can manage and clean up my session records

  Scenario: Delete a session history entry
    Given the user is in the session history section
    When the user selects the delete option for an entry
    Then the system should remove the entry from the history

```

```gherkin
US29 - Export Session History

Feature: Export session history
  As a user
  I want to export my session history
  So that I can keep an offline record of my email usage

  Scenario: Export session history as a CSV file
    Given the user is in the session history section
    When the user selects the "Export" option
    Then the system should generate a downloadable CSV file containing the session history

```

```gherkin
US30 - Restore Temporary Emails from History

Feature: Restore expired temporary emails from session history
  As a user
  I want to restore an expired temporary email
  So that I can access important information linked to it

  Scenario: Restore a temporary email
    Given the user is in the session history section
    When the user selects the restore option for an expired email
    Then the system should reactivate the email and allow access to its inbox

```

```gherkin
US31 - Filter Session History by Date

Feature: Filter session history by date
  As a user
  I want to filter my session history based on dates
  So that I can easily locate sessions from a specific time period

  Scenario: Filter history by date range
    Given the user is in the session history section
    When the user applies a date range filter
    Then the system should display only the sessions within the specified date range

```

\newpage


#### Execution Evidence for Sprint Review

Durante este quinto sprint se completo la implementacion en Kotlin de las funciones de nuestra aplicacíon, asi mismo se integro el video about-the-team y el video about-the-product en la landing page.

• Se implemento el sistema de filtro de correo falso.
• Se implemento el historial de correos y expiracion de estos.
• Se implemento un dominio personalizado.
• Se implementaron las barras de navegación dentro de la aplicación.
• Se implemento poder borrar un correo temporal y los correos asociados a este.


**Implementación del sistema de correos falso**

![Backend: Imagen extraída del navegador](src/img/Cap5/temp_back_5_2.png)

\newpage

**Implementación en Kotlin.**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/demo01.jpg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:rnf1}
\end{figure}

\newpage

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/demo02.jpg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:rnf1}
\end{figure}

\newpage

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/demo03.jpg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:rnf1}
\end{figure}

\newpage

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/demo04.jpg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:rnf1}
\end{figure}

**Implementación de videos en la landing Page**

![Imagen extraída de la Landing Page](src/img/Cap5/aboutUsLanding.png)


\newpage

#### Services Documentation Evidence for Sprint Review
En esta seccion, se muestra la documentacion de los servicios del *backend* de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken*, *Spring Data* y *Flask*

::: warn
**https://docs.spring.io/spring-boot/index.html**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation1.png)

\newpage

::: warn
**https://docs.spring.io/spring-boot/reference/web/spring-security.html#page-title**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation2.png)

::: warn
**https://www.npmjs.com/package/jsonwebtoken**
:::

![Imagen extraída de NPMjs](src/img/Cap5/documentation3.png)

\newpage

::: warn
**https://spring.io/projects/spring-data-jpa**
:::

![Imagen extraída de la documentación de Spring](src/img/Cap5/documentation4.png)

::: warn
**https://github.com/flasgger/flasgger**
:::

![Imagen extraída de la documentación de Flasgger](src/img/Cap5/documentation5.png)

\newpage

#### Software Deployment Evidence for Sprint Review
**Desplegar** ***Temporaly - Backend***

::: warn
Para acceder al despliegue del Backend de la aplicación, haga click en la [URL](https://temporally-api.ryzeon.me/swagger-ui/index.html)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-Backend*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap5/despliegue-backend-1.png)

2. Abrir, descargar y ejecutar en *IntelliJ IDEA* o su editor de preferencia para *Java*

![Repositorio del backend, imagen extraída de Github](src/img/Cap5/despliegue-backend-2.png)

3. Visualización de la documentación *Swagger*

![Swagger UI, imagen extraída de la API](src/img/Cap5/despliegue-backend-3.png)

\newpage

**Desplegar** ***Mobile App - Temporaly - Flutter Version***

::: warn
Para acceder al repositorio del FrontEnd, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-FlutterApp)
:::

1. Seleccionar el repositorio *CodeMinds-Temporaly-MobileApp*

![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

\newpage

2. Abrir, descargar y ejecutar en Android Studio 

::: important
 Asegurese de tener la version Android Studio Koala - 2024 - Patch 1 o 2
:::

![Repositorio del Mobile App, imagen extraída de Github](src/img/Cap5/mobile-app-configuration.png)

\newpage

3. Visualización de la aplicación

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap5/demo01.jpg}
    \caption{App movil: Imagen extraída de Android Studio}
    \label{fig:rnf2}
\end{figure}

\newpage

#### Team Collaboration Insights during Sprint

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-2.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-3.png)

\newpage


## *Validation Interviews*

Las entrevistas de validación son una herramienta clave en el proceso de diseño centrado en el usuario. A través de estas entrevistas, se busca obtener información directa de los usuarios sobre cómo interactúan con el producto, lo que permite validar su usabilidad y funcionalidad. Este método es esencial para identificar problemas, detectar oportunidades de mejora y asegurar que el producto final cumpla con las expectativas del público objetivo. Las entrevistas de validación no solo ayudan a mejorar la experiencia del usuario, sino que también garantizan que las decisiones de diseño estén basadas en datos reales y no en suposiciones.

A continuación, exploraremos cómo se diseñaron las entrevistas, cómo se llevó a cabo el registro de las mismas y las evaluaciones realizadas basadas en principios heurísticos.

### Diseño de entrevistas Landing Page

::: box 
**Segmento Objetivo 1:** Estudiantes de nivel escolar 
:::


**Evaluar la claridad del mensaje y propósito de la app:**

1) ¿Qué te transmite el mensaje "Crea, Usa y Olvida ;)"?
   
2) ¿Comprendes lo que significa proteger tu privacidad en línea con Temporaly? ¿Qué crees que hace la app al ver la primera sección?
   
3) Si tuvieras que explicar esta app a un amigo, ¿cómo lo harías?
   
4) ¿Cómo usarías Temporaly en tu vida diaria?

**Encontrar fácilmente las funcionalidades clave:**

1) ¿Sabes cómo crear un correo temporal rápidamente? ¿Te resulta claro cómo funciona?
   
2) ¿Te parece fácil entender los diferentes planes que ofrece la app (Básico, Pro, Master)?
   
3) Confianza en la seguridad que ofrece la app:
   
4) Después de ver la página, ¿sientes que tus datos estarían seguros si usas esta app? ¿Qué parte te hace sentir más seguro o inseguro?

**Sugerencias para mejorar el diseño o la usabilidad:**

1) ¿El diseño de la página es claro y fácil de navegar?
   
2) ¿Qué cambiarías para hacer la página más comprensible o atractiva para ti?

\newpage

::: box 
**Segmento Objetivo 2:** Estudiantes de nivel universitario y superior (pregrado - postgrado) 
:::

**Evaluar la claridad del mensaje y propósito de la app:**

1) ¿El mensaje "Protege tu Privacidad en Línea con Temporaly" te da una idea clara de lo que hace la app? ¿Por qué sí o por qué no?
   
2) ¿Cómo relacionarías esta funcionalidad con situaciones como registrar correos en plataformas académicas o eventos?
   
3) ¿Qué tipo de problemas crees que resuelve Temporaly? ¿Es claro para ti cómo usarla?
   
4) ¿Cómo te imaginas utilizando Temporaly para proteger tu información personal en situaciones reales (registro de eventos, estudios, etc.)?

**Encontrar fácilmente las funcionalidades clave:**

1) ¿Es fácil para ti entender cómo crear un correo temporal y gestionar tu historial? ¿Consideras útil la barra lateral que menciona el historial de correos usados?
   
2) ¿Te parece clara la diferencia entre los planes de pago y el plan gratuito?

**Confianza en la seguridad que ofrece la app:**

1) Después de navegar por la página, ¿qué tan seguro te sientes respecto a la protección de tu información personal?
   
2) ¿Consideras que hay elementos adicionales que podrían incrementar tu confianza en la seguridad de la app?

**Sugerencias para mejorar el diseño o la usabilidad:**

1) ¿Cómo valorarías el diseño en cuanto a facilidad de uso y navegación?
   
2) ¿Agregarías o cambiarías algo en la estructura o la interfaz para hacerla más efectiva?

\newpage


### Registro de entrevistas

::: warn
Para acceder al video de las entrevistas, haga click en la [URL](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210059_upc_edu_pe/ER-HaJJcUCxGhHOERY7D_r8B_lIO8pODYqcrZlTF8wnYoQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=VWGIGs)
:::

\vspace{0.4cm}

::: box
**Segmento Objetivo 1:** Estudiantes de nivel escolar
:::

**Entrevista #1**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Pol Adriano Ramos Rios \\ \hline
\textbf{Edad}                 & 14 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & inicio - fin           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

En la entrevista con Adriano Ramos Ríos sobre la aplicación *Temporaly*, se le pidió que evaluara distintos aspectos clave de la landing page, centrada en la creación de correos electrónicos temporales para proteger la privacidad en línea. Durante la entrevista, Adriano expresó que el eslogan principal de la aplicación, *"Crea, Usa y Olvida"*, le transmitía la idea de generar correos temporales para usarlos en situaciones donde no se desea emplear el correo personal, lo que le resultaba útil para evitar el riesgo de utilizar su correo personal en sitios web de dudosa confianza. En su opinión, la idea de usar correos momentáneos para verificar cuentas era clara y directa.

Adriano manifestó que entendía bien el propósito de la aplicación y que estaba diseñada para proteger la privacidad en línea, algo que considera que la landing page comunica de manera efectiva. Sin embargo, sugirió que sería útil agregar una descripción más detallada para los usuarios que no estén familiarizados con conceptos relacionados a la privacidad digital, de manera que el mensaje sea aún más claro para todos los públicos. Al preguntársele cómo explicaría la aplicación a un amigo, mencionó que la describiría como una herramienta útil para acceder a sitios web sin comprometer la información personal. Específicamente, explicó que *Temporaly* permite la creación de correos momentáneos que ayudan a verificar cuentas sin necesidad de exponer el correo principal, algo que él mismo usaría para obtener descuentos o probar aplicaciones sin tener que proporcionar información personal.

En cuanto a la usabilidad, Adriano indicó que le resultaría muy fácil usar la aplicación para crear correos temporales, pues ya tiene experiencia previa en el uso de servicios similares. No tuvo dificultades para comprender esta funcionalidad, lo que sugiere que el diseño es lo suficientemente intuitivo para usuarios con conocimientos básicos. Respecto a los planes de pago (Básico, Pro y Máster), destacó que entendía bien las diferencias entre ellos, comentando que el plan Básico tiene un tiempo limitado de uso, mientras que los planes Pro y Máster ofrecen mayores ventajas como tiempos más largos y la posibilidad de crear un número ilimitado de correos. Esto le pareció claro y considera que la elección del plan depende de las necesidades particulares de cada usuario.

Cuando se abordó el tema de la seguridad, Adriano manifestó que, tras revisar la página, sentía un alto nivel de confianza en la aplicación, especialmente al ver que está asociada con entidades reconocidas como *Gmail*, *LinkedIn* y la Universidad Privada de Ciencias Aplicadas (UPC). Estas asociaciones le transmitieron una sensación de seguridad, ya que para él son indicativos de que *Temporaly* es una aplicación seria y confiable. A pesar de esta confianza inicial, comentó que preferiría probar la aplicación antes de confiar completamente en ella. En cuanto a los elementos que más le transmitieron seguridad, destacó la sección donde se mencionan las asociaciones con empresas y universidades, lo cual le generó una impresión positiva. No identificó ninguna parte de la página que le hiciera sentir inseguro.

Finalmente, en relación al diseño de la página, Adriano opinó que es claro y fácil de navegar, tanto en su versión para escritorio como en dispositivos móviles. Afirmó que no tuvo dificultades para encontrar las secciones clave, como los testimonios, los precios y el apartado de contacto. Sin embargo, sugirió incluir un video explicativo que guíe a los usuarios a través de las funcionalidades de la app, especialmente a aquellos que no son tan tecnológicos, ya que un recurso visual podría facilitar la comprensión de cómo utilizar Temporaly y sacarle el máximo provecho. 

En resumen, Adriano considera que la aplicación tiene un buen nivel de claridad en cuanto a su mensaje y propósito, además de ser fácil de usar para aquellos con algo de experiencia. La confianza que genera la app es alta, aunque recomendó probarla para asegurarse de su eficacia. Su única sugerencia significativa fue agregar un video tutorial para mejorar la accesibilidad y la comprensión de la herramienta para todo tipo de usuarios.

![Imagen extraída del video de entrevistas](src/img/Cap5/AdrianoRamos_LandingPage.png)

\newpage

::: box
**Segmento Objetivo 2:** Estudiantes de Pregrado/Postgrado
:::

**Entrevista #1**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Kiomara Gil Olivera \\ \hline
\textbf{Edad}                 & 21 años                \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & inicio - fin           \\ \hline
\end{tabular}
\end{center}
\end{table}

En la entrevista con Kiomara Gil Olivera, se evaluó la landing page y funcionalidades de la aplicación Temporaly, enfocada en la creación de correos temporales para proteger la privacidad en línea. Kiomara comentó que el mensaje principal de la aplicación, "protege tu privacidad en línea", le daba una idea básica de lo que hace la aplicación, y que el tamaño de las letras era adecuado para captar la atención del usuario.

Cuando se le preguntó cómo relacionaría la funcionalidad de la aplicación con situaciones cotidianas, como el registro en plataformas académicas o eventos, expresó que Temporaly sería una forma confiable de proteger su información mientras está en línea. Además, mencionó que, dada la facilidad con la que los estudiantes pueden acceder a diversas páginas, Temporaly ayudaría a evitar que su información personal sea mal utilizada.

En cuanto a la usabilidad, Kiomara señaló que, tras leer toda la información de la aplicación, le sería fácil crear y gestionar correos temporales. Considera útil la barra lateral que muestra el historial de correos usados, y cree que la diferencia entre los planes de pago y el plan gratuito es clara, ya que cada uno menciona los beneficios específicos que ofrecen.

Respecto a la seguridad, Kiomara expresó que la aplicación le da confianza, especialmente porque cuenta con una oficina física y un número telefónico, lo que le permite sentir que no todo es virtual. Además, los comentarios de otros usuarios contribuyen a reforzar su confianza en Temporaly. No cree que sea necesario agregar más elementos para mejorar la seguridad de la aplicación.

Sobre el diseño, Kiomara considera que es atractivo y fácil de navegar. Los colores utilizados son llamativos sin ser molestos a la vista, y cada sección está bien organizada y es comprensible. Como sugerencia de mejora, mencionó que sería útil agregar una sección con inteligencia artificial para resolver preguntas frecuentes, lo que mejoraría la experiencia del usuario al proporcionar respuestas inmediatas sobre el funcionamiento de la aplicación.

En resumen, Kiomara valoró positivamente la aplicación y expresó que le daría una oportunidad debido a la confianza que le genera, tanto por sus funcionalidades como por la seguridad que transmite.


![Imagen extraída del video de entrevistas](src/img/Cap5/KiomaraOlivera_LandingPage.png)


\newpage

### Evualuaciones segun heuristicas

\begin{center}
\textbf{UX Heuristics \& Principles Evaluation} \\
\textbf{Usability – Inclusive Design – Information Architecture}
\end{center}

\vspace{10pt}

\begin{tabbing}
\hspace{5cm} \= \kill
\textbf{CARRERA:} \> Ingeniería de Software \\
\textbf{CURSO:} \> Aplicaciones para Dispositivos Móviles \\
\textbf{SECCIÓN:} \>  SW65 \\
\textbf{PROFESORES:} \> Jorge Luis Mayta Guillermo \\
\textbf{AUDITOR:} \> CodeMinds \\
\textbf{CLIENTE(S):} \> Estudiantes de nivel escolar y estudiantes de Pregrado/Postgrado \\
\end{tabbing}
\hrule

\vspace{10pt}

**SITE o APP A EVALUAR:** *Temporaly*

\vspace{10pt}

\textbf{TAREAS A EVALUAR:}  
El alcance de esta evaluación incluye la revisión de la usabilidad de la \textbf{landing page} de Temporaly, con foco en los siguientes elementos:

\begin{enumerate}
    \item \textbf{Comunicación del propósito de la app}: Claridad del mensaje en cuanto a la creación de correos temporales.
    \item \textbf{Acceso a planes de pago}: Evaluación de la presentación y diferencias entre los planes (Básico, Pro y Máster).
    \item \textbf{Confianza y seguridad}: Percepción de seguridad en la landing page.
    \item \textbf{Accesibilidad para usuarios nuevos}: Comprensión de la información por parte de usuarios no técnicos.
    \item \textbf{Diseño visual y navegación}: Facilidad para encontrar secciones clave.
\end{enumerate}

\newpage

**ESCALA DE SEVERIDAD**

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad:

\begin{table}[H]
\begin{center}
\begin{tabular}{|c|p{12cm}|}
\hline
\textbf{Nivel} & \textbf{Descripción} \\ \hline
1 & Problema superficial: puede ser fácilmente superado por el usuario o ocurre con muy poca frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo. \\ \hline
2 & Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se debería asignar una prioridad baja resolverlo de cara al siguiente release. \\ \hline
3 & Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlo. Es importante que sean corregidos y se les debe asignar una prioridad alta. \\ \hline
4 & Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento. \\ \hline
\end{tabular}
\end{center}
\end{table}

\vspace{10pt}


**TABLA RESUMEN**


\begin{table}[H]
\begin{center}
\begin{tabular}{|c|p{5cm}|c|p{6cm}|}
\hline
\textbf{\#} & \textbf{Problema} & \textbf{Escala de severidad} & \textbf{Heurística/Principio violado} \\ \hline
1 & Falta de descripción detallada sobre privacidad & 2 & Usabilidad: Concordancia entre el sistema y el mundo real \\ \hline
2 & Dificultad para entender los planes de pago & 3 & Usabilidad: Simplicidad y naturalidad de uso \\ \hline
3 & Ausencia de video tutorial en la landing page & 2 & Usabilidad: Ayuda y documentación \\ \hline
4 & Falta de elementos de confianza visual & 3 & Usabilidad: Confianza y seguridad \\ \hline
\end{tabular}
\end{center}
\end{table}

\newpage

**DESCRIPCIÓN DE PROBLEMAS**

- **PROBLEMA \#1: Falta de descripción detallada sobre privacidad**
  
  **Severidad:** 2 
  
  **Heurística violada:** Usabilidad – Concordancia entre el sistema y el mundo real 

  **Problema:** Aunque el mensaje principal es claro, falta una explicación más detallada sobre cómo la app protege la privacidad de los usuarios, lo que puede generar dudas en personas menos familiarizadas con estos temas. 

  **Recomendación:** Añadir una sección que explique en detalle la importancia de la privacidad y cómo Temporaly la garantiza.

\vspace{1cm}

- **PROBLEMA \#2: Dificultad para entender los planes de pago**
  
  **Severidad:** 3 

  **Heurística violada:** Usabilidad – Simplicidad y naturalidad de uso 

  **Problema:** Las diferencias entre los planes de pago no son suficientemente claras para los usuarios nuevos, lo que puede llevar a confusión al elegir entre el plan Básico, Pro y Máster. 
  **Recomendación:** Clarificar las ventajas de cada plan mediante comparaciones visuales, destacando las diferencias clave de forma más evidente.

\vspace{1cm}

- **PROBLEMA \#3: Ausencia de video tutorial en la landing page**
  
  **Severidad:** 2 

  **Heurística violada:** Usabilidad – Ayuda y documentación 

  **Problema:** Adriano sugirió que un video tutorial ayudaría a usuarios menos experimentados a entender mejor cómo funciona Temporaly, especialmente para aquellos que no están familiarizados con la creación de correos temporales. 

  **Recomendación:** Incluir un breve video explicativo en la landing page que muestre cómo usar la app paso a paso.

\vspace{1cm}


- **PROBLEMA \#4: Falta de elementos de confianza visual**
  **Severidad:** 3 

  **Heurística violada:** Usabilidad – Confianza y seguridad 

  **Problema:** Aunque se mencionan asociaciones con entidades como Gmail, LinkedIn y la UPC, falta un uso más prominente de estos elementos en la landing page para transmitir mayor confianza a usuarios nuevos. 

  **Recomendación:** Mostrar de manera más destacada los logos y asociaciones de seguridad con terceros en la landing page, asegurando que estos elementos visuales refuercen la confianza del usuario.

\vspace{1cm}


##  Video App Validation

Esta sección documenta el proceso de validación de la aplicación Temporaly a través de entrevistas en video realizadas con usuarios pertenecientes a los segmentos objetivo: estudiantes de nivel escolar y estudiantes de pregrado/postgrado. 

El objetivo de estas entrevistas fue evaluar la claridad del propósito de la aplicación, la facilidad de uso de sus funcionalidades clave, y la percepción de confianza y seguridad que genera. 
Además, se recopilaron observaciones y sugerencias para mejorar la experiencia de usuario.

### Diseño de entrevistas para la aplicación

::: box 
**Segmento Objetivo 1:** Estudiantes de nivel escolar 
:::

**Evaluar la claridad del propósito y funcionalidades principales de la app:**

1) ¿Qué impresión te da la app al abrirla por primera vez?
   
2)  Si tuvieras que explicar qué hace esta app, ¿cómo lo describirías a un amigo?
   
3)  ¿Encuentras útil poder crear un correo temporal para usarlo en situaciones específicas (por ejemplo, registro en juegos, promociones, etc.)? ¿Por qué?
   
**Evaluar la facilidad de uso de las funcionalidades clave:**

4) ¿Fue fácil entender cómo generar un correo temporal? Si no, ¿qué fue confuso?
   
5)  ¿Qué tan intuitivo te parece visualizar el historial de correos usados en la app?
  
6)   ¿Te resulta sencillo abrir un correo y leer los detalles dentro de la app?
   
7)   ¿Consideras útil poder responder correos desde la misma app? ¿Lo usarías?
   
**Confianza en la seguridad y experiencia general:**

8) ¿Sientes que tus datos están protegidos al usar Temporaly? ¿Qué te hace sentir seguro o inseguro?
   
9)  ¿Crees que esta app es confiable para manejar información personal?

**Sugerencias para mejorar la experiencia:**

10) ¿Te gusta el diseño de la app? ¿Qué cambiarías para hacerlo más atractivo?
    
11) Si pudieras agregar alguna funcionalidad nueva, ¿qué sería?

\newpage

::: box 
**Segmento Objetivo 2:** Estudiantes de nivel universitario y superior (pregrado - postgrado) 
:::


**Evaluar la claridad del propósito y funcionalidades principales de la app:**


1) ¿Te queda claro cómo proteger tu privacidad con esta app en situaciones como registros en plataformas académicas o eventos?
   
2) ¿Encuentras útil la funcionalidad de historial de correos? ¿Cómo lo usarías en tu día a día?
   
3) ¿Cómo describirías el propósito de Temporaly a alguien que no la conoce?
   
**Evaluar la facilidad de uso de las funcionalidades clave:**

4) ¿Qué tan fácil es para ti generar un correo temporal en la app?
   
5) ¿Encuentras intuitiva la manera de navegar entre los correos recibidos, el historial y las demás secciones?
   
6) ¿Cómo valorarías la opción de responder correos directamente desde la app? ¿Es claro el proceso?
   
7) ¿La opción de organizar o eliminar correos desde el historial te resulta útil?
   
**Confianza en la seguridad y experiencia general:**

8) ¿Qué tan seguro te sientes al usar esta app para proteger tu información personal?
   
9)  ¿Hay algo que podríamos mejorar para aumentar tu confianza en Temporaly?

**Sugerencias para mejorar la experiencia:**

10) ¿Te parece atractivo el diseño de la interfaz? ¿Qué cambiarías para mejorar la experiencia?
 
12) ¿Qué funcionalidad extra te gustaría ver en la app para que sea más útil para ti?
  

\newpage

### Registro de Entrevistas (App Validation)

::: warn
Para acceder al video de las entrevistas, haga click en la [URL](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210059_upc_edu_pe/EVPpQxXcLJJDnOCqWeLUuiYB7Ts1CDl75PiiycnrxtprCw?e=WLvBE0&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

Link acortado: https://n9.cl/temporalyappvalidation

:::

\vspace{0.4cm}

::: box
**Segmento Objetivo 1:** Estudiantes de nivel escolar
:::

**Entrevista #1**

\begin{table}[H]
\begin{center} 
\begin{tabular}{|p{5cm}|p{6cm}|}  
\hline
\textbf{Nombre y Apellido}    & Carlet Gil Olivera \\ \hline
\textbf{Edad}                 & 17 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & 06:00 - 08:57          \\ \hline
\end{tabular}
\end{center}
\end{table}


**Resumen de la entrevista**

En la entrevista con Carlet Gil Olivera, se le mostró y pidió evaluar la aplicación Temporaly, una herramienta para generar correos electrónicos temporales con el objetivo de proteger la privacidad y evitar el spam. Durante la conversación, Carlet expresó una impresión inicial de curiosidad por tratarse de una aplicación novedosa y práctica.

Carlet entendió que el principal objetivo de Temporaly es facilitar la creación de correos electrónicos temporales para situaciones como registros en plataformas y aplicaciones, evitando el uso del correo personal. Expresó que encuentra útil esta herramienta para separar correos importantes de los que no lo son, y consideró que su propósito está bien definido y es fácil de explicar a otras personas.
Destacó que Temporaly resulta ideal para situaciones donde, por apuro, se podría registrar en sitios web que luego envían spam, valorando que la aplicación permite mantener la privacidad y organización de la bandeja de entrada.
Por otro lado, Carlet encontró la aplicación intuitiva y sencilla de usar. Logró comprender cómo generar un correo temporal, personalizarlo, gestionar el historial de correos y eliminar los que ya no son útiles. Además, mencionó que la interfaz visual es clara y funcional, sin elementos innecesarios, lo que contribuye a una experiencia fluida.
Durante la demostración, destacó lo fácil que fue abrir correos desde la aplicación y utilizar las funcionalidades principales. También consideró útil la posibilidad de responder correos directamente desde Temporaly.
Asimismo, Carlet manifestó sentirse segura al usar Temporaly. Percibió la aplicación como confiable para manejar información personal, al transmitir un enfoque claro en la protección de datos y evitar riesgos de spam. Comentó que el diseño minimalista y directo contribuye a generar confianza en los usuarios.

Aunque valoró positivamente las funcionalidades actuales, Carlet sugirió incorporar una opción para clasificar correos en leídos y no leídos, y añadió que sería práctico incluir una función que elimine automáticamente los correos ya revisados.
Finalmente, Carlet Gil Olivera evaluó Temporaly como una aplicación útil, confiable y fácil de usar, con un diseño claro que facilita su funcionalidad. Destacó su utilidad para mantener la privacidad en línea y evitar el desorden en la bandeja de entrada. Sus sugerencias, centradas en clasificaciones y automatizaciones, apuntan a mejorar aún más la experiencia del usuario y hacer la aplicación aún más versátil.


![Imagen extraída del video de entrevistas](src/img/Cap5/entrevista01_Segmento01.png)

\newpage

**Entrevista #2**

\begin{table}[H]
\begin{center}  
\begin{tabular}{|p{5cm}|p{6cm}|}  
\hline
\textbf{Nombre y Apellido}    & Pol Adriano Ramos Rios \\ \hline
\textbf{Edad}                 & 14 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & 08:57 - 19:17          \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

En la entrevista con Pol Adriano Ramos Ríos, se le presentó la aplicación Temporaly, una herramienta diseñada para generar correos electrónicos temporales que protegen la privacidad y evitan el spam. Pol expresó una primera impresión positiva, destacando el diseño minimalista y funcional de la aplicación. Desde su perspectiva, Temporaly es ideal para registros en páginas web de dudosa confianza o para utilizarla como una cuenta secundaria temporalmente.

Durante la demostración, se le mostró cómo personalizar un correo temporal con su nombre y cómo usarlo para registros en plataformas como Duolingo o Pinterest. Pol comprobó que la aplicación permite enviar y recibir correos de manera efectiva y gestionar un historial de correos temporales, lo cual consideró práctico para evitar el desorden en la bandeja de entrada. Además, destacó la posibilidad de borrar correos antiguos y generar nuevos automáticamente, lo que consideró una funcionalidad útil para mantener la organización.

En cuanto a su utilidad, Pol señaló que Temporaly es una herramienta efectiva para evitar usar el correo personal en situaciones donde podría recibir spam o para pruebas temporales, como juegos o promociones. Indicó que fue muy fácil entender cómo generar un correo temporal y calificó la aplicación como intuitiva y sencilla. No obstante, mencionó que podría ser útil ofrecer soporte en varios idiomas, ya que algunas personas podrían no sentirse cómodas con una interfaz solo en inglés.

Respecto a la seguridad, Pol manifestó sentirse tranquilo al usar la aplicación, ya que un correo temporal minimiza el riesgo de exponer datos personales o cuentas privadas. En cuanto al diseño, valoró el enfoque minimalista y funcional, mencionando que no haría cambios importantes. Sin embargo, sugirió agregar una funcionalidad de traducción automática para los correos recibidos en otros idiomas, lo que facilitaría su uso en un contexto global.

En resumen, Pol evaluó Temporaly como una herramienta práctica, segura y fácil de usar. Reconoció su utilidad para proteger la privacidad y destacó la claridad de su diseño e interfaz. Como mejora, sugirió incluir opciones multilingües y un traductor para los correos, lo que aumentaría su accesibilidad y versatilidad.


![Imagen extraída del video de entrevistas](src/img/Cap5/entrevista02_Segmento01.png)



\newpage



::: box
**Segmento Objetivo 2:** Estudiantes de Pregrado/Postgrado
:::

**Entrevista #1**

\begin{table}[H]
\begin{center}  
\begin{tabular}{|p{5cm}|p{6cm}|}  
\hline
\textbf{Nombre y Apellido}    & Carlos Sanchez \\ \hline
\textbf{Edad}                 & 20            \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & 19:19 - 28:03        \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

En la entrevista con Carlos Sánchez, se le presentó la aplicación Temporaly, una herramienta para generar correos electrónicos temporales que permite proteger la privacidad y gestionar registros en sitios web de manera segura. Carlos describió la aplicación como una solución innovadora y útil para proteger la identidad digital, especialmente al interactuar con plataformas de baja confianza.

Durante la demostración, se creó un correo temporal personalizado con su nombre, que se utilizó para registrarse en Medium y enviar mensajes de prueba. Carlos destacó la facilidad para generar correos y valoró la posibilidad de personalizarlos, lo que añadió un nivel de comodidad al proceso. Además, comprobó la utilidad del historial de correos, una función que permite revisar, organizar y eliminar los correos usados previamente, lo cual consideró esencial para mantener control y orden en su uso.

Carlos mencionó que la aplicación es intuitiva y sencilla, con un diseño minimalista que facilita su navegación. Apreció que las funcionalidades están claramente indicadas mediante botones simples, lo que la hace accesible incluso para usuarios menos experimentados. También indicó que la posibilidad de responder correos desde la aplicación sería un añadido valioso para casos específicos, como comunicaciones legales.

En términos de seguridad, Carlos afirmó sentirse confiado al usar Temporaly, ya que no solicita datos personales ni credenciales sensibles, lo que refuerza su confianza en la herramienta. No obstante, sugirió que incluir documentación adicional sobre los protocolos de seguridad utilizados podría aumentar aún más su confianza. Además, propuso una funcionalidad extra que registre los sitios web donde se ha utilizado un correo temporal, para mantener un control más detallado de las actividades realizadas con la aplicación.

En resumen, Carlos evaluó positivamente Temporaly, destacando su utilidad, facilidad de uso y diseño atractivo. Sus sugerencias para mejorar la aplicación incluyen opciones para responder correos, mayor transparencia sobre su seguridad y un registro detallado de los sitios donde se han utilizado los correos temporales. Consideró que la herramienta es efectiva para proteger la privacidad y mantener la organización en actividades online.


![Imagen extraída del video de entrevistas](src/img/Cap5/entrevista01_Segmento02.jpg)

\newpage


**Entrevista #2**

\begin{table}[H]
\begin{center}  
\begin{tabular}{|p{5cm}|p{6cm}|}  
\hline
\textbf{Nombre y Apellido}    & Mateo Daniel Del Castillo \\ \hline
\textbf{Edad}                 & 20            \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & 28:03 - 40:52          \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

En la entrevista con Mateo Daniel Del Castillo, se le presentó la aplicación Temporaly, una herramienta para la creación de correos electrónicos temporales, diseñada para proteger la privacidad y evitar el spam en registros en plataformas o servicios online. Mateo destacó que la aplicación le parece una solución eficiente y clara para proteger la identidad digital, especialmente útil en situaciones donde no se desea utilizar un correo personal.

Durante la demostración, Mateo pudo observar cómo se generaba un correo temporal personalizado con su nombre y un dominio predeterminado, comprobando su funcionalidad al enviarse correos y registrarse en aplicaciones como Medium o Trello. Aunque tuvo algunos inconvenientes iniciales con un captcha, confirmó que el proceso era sencillo y que la aplicación cumplía con su propósito principal. Además, valoró la funcionalidad del historial para revisar o eliminar correos, resaltando que las cuentas creadas con los correos temporales se mantienen activas en las plataformas externas.

Mateo describió la aplicación como una forma rápida y segura de generar un correo temporal sin necesidad de procesos de autenticación complejos. Esto, según él, es especialmente útil para recibir spam o registrarse en sitios de dudosa confianza. La generación del correo le resultó intuitiva, destacando la facilidad de uso del botón “New” y la selección automática de dominios, lo que optimiza el proceso.

En cuanto a la interfaz, Mateo la encontró minimalista, bien organizada y visualmente atractiva. Comentó que los elementos de diseño, como las animaciones y los colores, le parecieron llamativos y bien ejecutados. En términos de seguridad, expresó sentirse totalmente tranquilo, ya que la aplicación no solicita datos personales ni requiere autenticación adicional, lo que considera fundamental para un servicio de este tipo.

Como sugerencia, Mateo propuso implementar un historial organizado por fechas, que permita buscar correos antiguos de manera más eficiente. También consideró valiosa la posibilidad de responder correos desde la aplicación en casos específicos, aunque reconoce que el propósito principal de un correo temporal no es necesariamente la comunicación bidireccional.

En conclusión, Mateo evaluó Temporaly como una aplicación útil, confiable y fácil de usar, con un diseño atractivo y funcionalidades claras. Destacó su utilidad para proteger la identidad digital y gestionar correos temporales, proponiendo mejoras enfocadas en la organización del historial y posibles funciones adicionales para responder correos de manera ocasional.

![Imagen extraída del video de entrevistas](src/img/Cap5/entrevista02_Segmento02.jpg)


\newpage


### Evaluaciones según heuristicas (App Validation)

\begin{center}
\textbf{UX Heuristics \& Principles Evaluation} \\
\textbf{Usability – Inclusive Design – Information Architecture}
\end{center}

\vspace{10pt}

\begin{tabbing}
\hspace{5cm} \= \kill
\textbf{CARRERA:} \> Ingeniería de Software \\
\textbf{CURSO:} \> Aplicaciones para Dispositivos Móviles \\
\textbf{SECCIÓN:} \>  SW65 \\
\textbf{PROFESORES:} \> Jorge Luis Mayta Guillermo \\
\textbf{AUDITOR:} \> CodeMinds \\
\textbf{CLIENTE(S):} \> Estudiantes de nivel escolar y estudiantes de Pregrado/Postgrado \\
\end{tabbing}
\hrule

\vspace{10pt}

**SITE o APP A EVALUAR:** *Temporaly*

\vspace{10pt}

\textbf{TAREAS A EVALUAR:}  

El alcance de esta evaluación incluye las siguientes áreas de la aplicación Temporaly, basadas en las entrevistas realizadas:


\begin{enumerate}
    \item \textbf{Comunicación del propósito de la app:} Claridad sobre la utilidad de Temporaly como generador de correos temporales.
    \item \textbf{Usabilidad y flujo de funcionalidades:} Facilidad para crear correos temporales, gestionar el historial, personalizar y eliminar correos.
    \item \textbf{Confianza y seguridad:} Percepción de seguridad por parte de los usuarios.
    \item \textbf{Accesibilidad visual y funcional:} Comprensión de la interfaz y navegación, especialmente para usuarios nuevos.
    \item \textbf{Sugerencias de mejoras:} Inclusión de nuevas funcionalidades y soporte multilingüe.
\end{enumerate}


\newpage


**Escala de Severidad de Problemas**

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad:

\begin{table}[H] 
\begin{center} 
\begin{tabular}{|c|p{12cm}|} \\ \hline 
\textbf{Nivel} & \textbf{Descripción} \\ \hline 
1 & Problema superficial: se supera fácilmente o rara vez ocurre. Solución opcional. \\ \hline 
2 & Problema menor: ocurre ocasionalmente o requiere más esfuerzo del usuario. Prioridad baja. \\ \hline 
3 & Problema mayor: ocurre frecuentemente o impide un flujo fluido. Prioridad alta. \\ \hline 
4 & Problema crítico: afecta significativamente la experiencia o impide continuar. Prioridad inmediata. \\ \hline 
\end{tabular} 
\end{center} 
\end{table}


**Tabla Resumen de Problemas Identificados**

\begin{table}[H] 
\begin{center}
\begin{tabular}{|c|p{5cm}|c|p{6cm}|} 
\hline 
\textbf{\#} & \textbf{Problema} & \textbf{Escala de Severidad} & \textbf{Heurística/Principio Violado} \\ \hline 
1 & Falta de clasificación de correos en leídos/no leídos & 2 & Usabilidad: Flexibilidad y eficiencia de uso \\ \hline 
2 & Ausencia de traducción de correos y soporte multilingüe & 3 & Usabilidad: Reconocimiento en lugar de recuerdo \\ \hline 
3 & Necesidad de una función de eliminación automática de correos revisados & 2 & Usabilidad: Diseño minimalista y eficiente \\ \hline 
4 & Inexistencia de indicadores visuales para reforzar confianza & 3 & Usabilidad: Confianza y seguridad \\ \hline 
\end{tabular} 
\end{center} 
\end{table}

\newpage

**Descripción de Problemas Identificados**


- **PROBLEMA \#1: Ausencia de traducción de correos y soporte multilingüe**
  
  **Severidad:** 3
  
  **Heurística violada:** Usabilidad – Reconocimiento en lugar de recuerdo
  
  **Problema:** Pol sugirió que algunos usuarios podrían enfrentar dificultades al recibir correos en idiomas extranjeros o interactuar con una interfaz solo en inglés.
  
  **Recomendación:** Incorporar soporte multilingüe para la interfaz y un traductor automático para correos recibidos, mejorando la accesibilidad para usuarios globales.

- **PROBLEMA \#2: Necesidad de una función de eliminación automática de correos revisados**
  
  **Severidad:** 2
  
  **Heurística violada:** Usabilidad – Diseño minimalista y eficiente
  
  **Problema:** La gestión manual de correos puede volverse tediosa para usuarios frecuentes.
  
  **Recomendación:** Agregar una opción de eliminación automática para correos marcados como leídos o con un tiempo de expiración definido.

- **PROBLEMA \#3: Inexistencia de indicadores visuales para reforzar confianza**
  
  **Severidad:** 3
  
  **Heurística violada:** Usabilidad – Confianza y seguridad
  
  **Problema:** Aunque los entrevistados consideraron a Temporaly confiable, sugirieron que incluir elementos visuales como certificados o asociaciones destacadas mejoraría la percepción de seguridad.
  
  **Recomendación:** Incorporar elementos visuales en la landing page, como iconos de certificados de seguridad, sellos de confianza o referencias a empresas asociadas.


\newpage





##  Video About the product

En esta sección, se presenta un video que ofrece una visión general sobre Temporaly, destacando su propósito, principales funcionalidades y beneficios para los usuarios. Este video tiene como objetivo comunicar de manera clara y atractiva las características clave del producto, mostrando cómo puede ser utilizado para proteger la privacidad y optimizar la gestión de correos temporales.

El video está diseñado para proporcionar una experiencia visual que complemente la documentación escrita y permita a los usuarios potenciales comprender rápidamente el valor que Temporaly aporta en contextos cotidianos.

::: warn
Para acceder al video  about the product, haga click en la [URL](https://youtu.be/VEjg2eKx958)

Link acortado: https://youtu.be/VEjg2eKx958

:::

![Imagen extraída del video about the product](src/img/Cap5/about-the-product.jpg)

\newpage


# Conclusiones

##  Conclusiones y recomendaciones
 
- **Conclusiones**
  
  - Como equipo, concluimos que Temporaly ha logrado cumplir su propósito principal: ofrecer una herramienta confiable y accesible para generar correos electrónicos temporales, lo que permite a los usuarios proteger su privacidad y evitar el spam. La implementación de funcionalidades clave como la gestión del historial y la eliminación automática de correos revisados ha optimizado la experiencia del usuario.
  
  - El uso de metodologías ágiles y la implementación de tecnología avanzada han sido claves para optimizar la experiencia del usuario. Este enfoque nos ha permitido asegurar que las funcionalidades de Temporaly sean relevantes y efectivas para el segmento objetivo, manteniéndonos competitivos en un mercado en constante evolución.
  
  - Nuestro enfoque en la segmentación por nivel educativo (estudiantes de secundaria, pregrado y postgrado) ha garantizado que cada funcionalidad esté alineada con las necesidades específicas de cada grupo. Esto fortalece la propuesta de valor de Temporaly y asegura una experiencia personalizada para diferentes tipos de usuarios.
  
  - Con Temporaly, ofrecemos una solución que puede impactar positivamente la vida digital de los usuarios, especialmente estudiantes que buscan proteger su información personal al interactuar con plataformas académicas y sociales. Esto refuerza el valor del proyecto y su relevancia en un contexto de creciente preocupación por la privacidad digital.

- **Recomendaciones**
  
  - Sugerimos desarrollar campañas educativas dirigidas a estudiantes, padres y educadores para promover un mejor entendimiento de la seguridad digital. Esto permitirá maximizar el impacto de Temporaly como herramienta de protección en línea y fomentar su uso consciente.
  
  - Recomendamos integrar nuevas funcionalidades, como soporte multilingüe, traducción automática de correos, opciones avanzadas de personalización y tiempos de expiración más largos. Estas características pueden aumentar el atractivo de la aplicación para diferentes segmentos y mejorar la retención de usuarios.
  
  - Proponemos realizar pruebas de usabilidad periódicas y encuestas a los usuarios para identificar áreas de mejora. La implementación de estos ajustes debe realizarse mediante iteraciones ágiles para mantener la relevancia y eficiencia del producto.
  
  - Para asegurar el éxito a largo plazo, es esencial implementar un plan de mantenimiento que incluya monitoreo continuo de la infraestructura, actualizaciones regulares y escalabilidad de los servicios para manejar el crecimiento de usuarios.
  

##  Video App Validation

::: warn
Para acceder al video de las entrevistas, haga click en la [URL](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210059_upc_edu_pe/EVPpQxXcLJJDnOCqWeLUuiYB7Ts1CDl75PiiycnrxtprCw?e=WLvBE0&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

Link acortado: https://n9.cl/temporalyappvalidation

:::

![Imagen extraída del video de entrevistas](src/img/Cap5/entrevista01_Segmento02.jpg)

\newpage

##  Video About the product

::: warn
Para acceder al video  about the product, haga click en la [URL](https://youtu.be/VEjg2eKx958)

Link acortado: https://youtu.be/VEjg2eKx958

:::

![Imagen extraída del video about the product](src/img/Cap5/about-the-product.jpg)


##  Video About the team

::: warn
Para acceder al video de las entrevistas, haga click en la [URL]()

Link acortado: 

:::

![Imagen extraída del video about the team](src/img/Cap5/about-the-team.png)

\newpage

# Glosario

1. **API (Application Programming Interface):**
Conjunto de definiciones y protocolos que permiten la comunicación entre diferentes sistemas o aplicaciones, facilitando el intercambio de datos y la integración de funcionalidades.

2. **Correo Temporal:**
Dirección de correo electrónico creada con un propósito específico y por un tiempo limitado. Se utiliza para proteger la privacidad y evitar el spam al registrarse en plataformas o servicios.

3. **Flutter:**
Framework de desarrollo de código abierto creado por Google, utilizado para crear aplicaciones móviles, web y de escritorio desde una base de código única.

4. **Metodologías Ágiles:**
Conjunto de principios y prácticas para la gestión de proyectos y desarrollo de software que enfatizan la colaboración, la flexibilidad y la entrega continua de valor.

5. **Privacidad Digital:**
Derecho de los usuarios a proteger su información personal en línea, controlando quién tiene acceso a sus datos y cómo se utilizan.

6. **Segmentación de Usuarios:**
Proceso de dividir una audiencia en grupos más pequeños con características similares (por ejemplo, nivel educativo) para personalizar los productos y servicios ofrecidos.

7. **Seguridad Digital:**
Conjunto de medidas diseñadas para proteger los sistemas informáticos y los datos contra accesos no autorizados, ataques o pérdida de información.

8. **Sprint:**
Unidad de trabajo en las metodologías ágiles, generalmente de 1 a 4 semanas, durante la cual se desarrolla y entrega un conjunto específico de funcionalidades o mejoras.

9.  **Swagger:**
Herramienta para diseñar, construir y documentar APIs de manera interactiva, proporcionando una interfaz amigable para explorar y probar los endpoints.

10. **Temporaly:**
Aplicación desarrollada para la creación y gestión de correos electrónicos temporales, enfocada en proteger la privacidad de los usuarios y evitar el spam en registros en línea.

11. ***Testing (Pruebas):***
Proceso de evaluación de una aplicación o sistema para garantizar que las funcionalidades cumplan con los requisitos y que el software sea estable y confiable.

12. ***UI/UX (User Interface/User Experience):***
Diseño de la interfaz y experiencia del usuario en un producto o aplicación, enfocado en la facilidad de uso, la funcionalidad y la satisfacción del usuario.

13. ***Work Item (WI):***
Unidad de trabajo específica dentro de un sprint, que representa una tarea o funcionalidad a desarrollar, asignada a un miembro del equipo.

14. **Repositorio:**
Espacio centralizado donde se almacena, gestiona y comparte el código fuente de un proyecto, a menudo utilizado en plataformas como GitHub.

15. **Notificaciones Push:**
Mensajes enviados desde una aplicación a los dispositivos de los usuarios para informarles sobre eventos o actualizaciones importantes en tiempo real.

16. **Historial de Sesiones:**
Registro de las actividades realizadas en una aplicación, que en el caso de Temporaly, permite a los usuarios revisar y gestionar correos electrónicos temporales usados previamente.

17. **Microservicios:**
Arquitectura de software donde las aplicaciones se estructuran como un conjunto de servicios pequeños e independientes que se comunican entre sí, típicamente mediante APIs.

18. ***Mockup:***
Representación visual de un diseño que muestra cómo se verá la interfaz de usuario sin detallar su funcionalidad.

19. **Prototipo:**
Modelo preliminar de un producto o sistema que permite probar y evaluar sus funcionalidades antes del desarrollo final.

20. ***Sprint Backlog:***
Lista de tareas o actividades que un equipo debe completar durante un sprint, alineada con los objetivos del proyecto.

21. ***Wireframe:***
Esquema o representación básica de la estructura de una interfaz, que sirve para planificar el diseño y funcionalidad de una página o aplicación.

22. ***Lean UX:***
Metodología de diseño centrada en el usuario que busca reducir el tiempo de desarrollo mediante iteraciones rápidas y retroalimentación constante.

23. ***Testing Suite:***
Conjunto de pruebas diseñadas para evaluar la funcionalidad, rendimiento y seguridad de un software.

24. ***Empathy Mapping:***
Herramienta para entender las necesidades, pensamientos y emociones de los usuarios, basada en sus experiencias y puntos de vista.

25. ***Bounded Context:***
Término de diseño de software que define un límite dentro del cual un modelo específico es válido, usado comúnmente en la arquitectura orientada a dominios.

26. ***SEO (Search Engine Optimization):***
Estrategias y prácticas diseñadas para mejorar la visibilidad de un sitio web en los resultados orgánicos de los motores de búsqueda.

27. ***CI/CD (Integración Continua/Despliegue Continuo):***
Práctica de desarrollo que automatiza la integración de código y su despliegue, asegurando actualizaciones rápidas y sin errores.

28. ***User Journey Mapping:***
Técnica para visualizar el recorrido completo que realiza un usuario al interactuar con un producto o servicio, identificando puntos de mejora.

29. ***RESTful:***
Estilo arquitectónico para sistemas de software que utiliza operaciones HTTP estándar, como GET, POST, PUT y DELETE, para interactuar con recursos web.

30. ***Cloud Deployment:***
Proceso de implementar aplicaciones y servicios en servidores remotos en la nube, accesibles a través de internet.