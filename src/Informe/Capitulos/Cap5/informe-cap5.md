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

- **Tecnologías:** Para el desarrollo del *mobile app* utilizamos tecnologías como *Kotlin* y *Jetpack Compose*.

- **Herramientas:** Nos apoyamos en herramientas ampliamente utilizadas y recomendadas para el desarrollo *mobile android*, tales como: *Android Studio*, *Github* y *Git*

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

2. Abrir, descargar y ejecutar en *VSCode*, *Vim* o su editor de preferencia

    ![Repositorio del backend, imagen extraída de Github](src/img/Cap5/generate-email-backend-configuration.png)

3. Visualización de la documentación *Flasgger*

    ![Flasgger, imagen extraída de Github](src/img/Cap5/generate-email-backend-flasgger.png)

\newpage

**Desplegar** ***Mobile App - Temporaly***

1. Seleccionar el repositorio *CodeMinds-Temporaly-MobileApp*

    ![Organización CodeMinds, imagen extraída de Github](src/img/Cap4/git_repo.png)

2. Abrir, descargar y ejecutar en Android Studio 

    ::: important
        Asegurese de tener la version Android Studio Koala - 2024 - Patch 1 o 2
    :::

    ![Repositorio del Mobile App, imagen extraída de Github](src/img/Cap5/mobile-app-configuration.png)

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
\textbf{Sum of Story Points} & - 106 \\ \hline
\end{longtable}

\newpage

#### *Sprint Backlog 2*

En este segundo sprint, se priorizó el desarrollo de funcionalidades esenciales relacionadas con la generación y gestión de correos temporales en la aplicación Temporaly. Estas funcionalidades están alineadas con los objetivos clave de la app, que incluyen la creación, personalización y manejo eficiente de correos temporales, brindando a los usuarios una experiencia fluida y segura.

A continuación, se presentan las Historias de Usuario organizadas según su funcionalidad dentro de la aplicación.

\begin{longtable}{|c|p{2.5cm}|p{1cm}|p{4cm}|p{2cm}|p{2cm}|p{1cm}|}
\hline
\textbf{ID} & \textbf{User Story} & \textbf{Work Item (WI)} & \textbf{Description} & \textbf{Estimation (Hours)} & \textbf{Assigned To} & \textbf{Status} \\ \hline

\multirow{4}{*}{US01} & \multirow{4}{*}{\parbox[t]{2.5cm}{Registro de usuario}} & WI01 & Diseño de la pantalla de registro utilizando Jetpack Compose & 6h & Alex Avila & Done \\ \cline{3-7}
 &  & WI02 & Conectar la pantalla de registro con la API & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI03 & Implementar validación de campos en la pantalla de registro & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI04 & Pruebas de usabilidad para el registro de usuario & 3h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US02} & \multirow{3}{*}{\parbox[t]{2.5cm}{Confirmación de creación de cuenta}} & WI05 & Implementar la funcionalidad de confirmación de cuenta con la API & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI06 & Diseño de la pantalla de confirmación de cuenta en Compose & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI07 & Pruebas para la confirmación de cuenta & 2h & Alex Avila & Done \\ \hline

\multirow{2}{*}{US03} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificación de cuenta}} & WI08 & Conectar la verificación de cuenta con la API & 4h & Alex Avila & Done \\ \cline{3-7}
 &  & WI09 & Implementar la pantalla de verificación de cuenta & 3h & Alex Avila & Done \\ \hline

\multirow{2}{*}{US04} & \multirow{2}{*}{\parbox[t]{2.5cm}{Inicio de sesión de cuenta}} & WI10 & Crear la pantalla de inicio de sesión en Compose & 5h & Alex Avila & Done \\ \cline{3-7}
 &  & WI11 & Conectar la pantalla de inicio de sesión con la API & 5h & Alex Avila & Done \\ \hline

\multirow{3}{*}{US05} & \multirow{3}{*}{\parbox[t]{2.5cm}{Generación de correo temporal con un clic}} & WI12 & Diseño de la pantalla de generación de correos temporales & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI13 & Implementar la funcionalidad de generación de correos con un clic & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI14 & Pruebas de generación de correos temporales & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US06} & \multirow{2}{*}{\parbox[t]{2.5cm}{Duración específica del correo temporal}} & WI15 & Implementar opción para seleccionar duración del correo & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI16 & Conectar la opción de duración con la API & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US07} & \multirow{2}{*}{\parbox[t]{2.5cm}{Confirmación visual de creación de correo}} & WI17 & Añadir confirmación visual en la pantalla de generación de correos & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI18 & Pruebas de confirmación visual & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US08} & \multirow{2}{*}{\parbox[t]{2.5cm}{Personalización del dominio del correo temporal}} & WI19 & Implementar la opción para personalizar el dominio del correo temporal & 5h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI20 & Conectar la opción de personalización de dominio con la API & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US09} & \multirow{2}{*}{\parbox[t]{2.5cm}{Generación Múltiple de correos temporales}} & WI21 & Implementar la opción para generar múltiples correos & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI22 & Pruebas para la generación de múltiples correos & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US10} & \multirow{2}{*}{\parbox[t]{2.5cm}{Copiar correo temporal al portapapeles}} & WI23 & Implementar botón de copiar al portapapeles en la pantalla de correos temporales & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI24 & Pruebas de funcionalidad de copiado al portapapeles & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US11} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos temporales activos}} & WI25 & Crear la pantalla de visualización de correos temporales activos & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI26 & Conectar la pantalla con la API & 4h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US12} & \multirow{2}{*}{\parbox[t]{2.5cm}{Sugerencias automáticas de nombres para correos}} & WI27 & Implementar sugerencias automáticas de nombres en la pantalla de generación de correos & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI28 & Pruebas de la funcionalidad de sugerencias de nombres & 2h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US13} & \multirow{2}{*}{\parbox[t]{2.5cm}{Proceso de generación rápido y fluido}} & WI29 & Optimización del proceso de generación de correos para mejorar el rendimiento & 4h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI30 & Pruebas de optimización del rendimiento & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US14} & \multirow{2}{*}{\parbox[t]{2.5cm}{Advertencia de expiración de correo temporal}} & WI31 & Implementar una advertencia visual cuando un correo temporal esté por expirar & 3h & Abel Ortega & Done \\ \cline{3-7}
 &  & WI32 & Conectar la advertencia con la API & 3h & Abel Ortega & Done \\ \hline

\multirow{2}{*}{US15} & \multirow{2}{*}{\parbox[t]{2.5cm}{Acceso a bandeja de entrada de correos temporales}} & WI33 & Implementar la pantalla de la bandeja de entrada & 5h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI34 & Conectar la bandeja de entrada con la API & 4h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US16} & \multirow{2}{*}{\parbox[t]{2.5cm}{Visualización de correos recibidos}} & WI35 & Implementar la pantalla de visualización de correos recibidos & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI36 & Conectar la visualización de correos con la API & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US17} & \multirow{2}{*}{\parbox[t]{2.5cm}{Notificación de nuevos correos en la bandeja de entrada}} & WI37 & Implementar notificaciones push para la llegada de nuevos correos temporales & 4h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI38 & Pruebas de funcionalidad de notificaciones push & 3h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US18} & \multirow{2}{*}{\parbox[t]{2.5cm}{Leer y responder correos temporales}} & WI39 & Implementar la funcionalidad de lectura y respuesta en la pantalla de correos temporales & 5h & Mateo Vilchez & Done \\ \cline{3-7} 
 &  & WI40 & Conectar la funcionalidad de respuesta con la API & 4h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US19} & \multirow{2}{*}{\parbox[t]{2.5cm}{Buscar correos en la bandeja de entrada}} & WI41 & Implementar barra de búsqueda en la bandeja de entrada & 3h & Mateo Vilchez & Done \\ \cline{3-7}
 &  & WI42 & Pruebas de la funcionalidad de búsqueda & 2h & Mateo Vilchez & Done \\ \hline

\multirow{2}{*}{US20} & \multirow{2}{*}{\parbox[t]{2.5cm}{Eliminar correos temporales}} & WI43 & Implementar opción para eliminar correos temporales desde la bandeja de entrada & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI44 & Pruebas de la funcionalidad de eliminación de correos & 2h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US21} & \multirow{2}{*}{\parbox[t]{2.5cm}{Marcar correos como importantes}} & WI45 & Implementar opción para marcar correos como importantes & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI46 & Conectar la funcionalidad de marcar como importantes con la API & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US22} & \multirow{2}{*}{\parbox[t]{2.5cm}{Filtrar correos por fecha o remitente}} & WI47 & Implementar filtros por fecha o remitente en la bandeja de entrada & 4h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI48 & Pruebas de la funcionalidad de filtrado & 3h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US23} & \multirow{2}{*}{\parbox[t]{2.5cm}{Verificar correos temporales usados recientemente}} & WI49 & Implementar una sección de correos temporales usados recientemente & 3h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI50 & Pruebas de la funcionalidad de correos usados recientemente & 2h & Belen Ramos & Done \\ \hline

\multirow{2}{*}{US24} & \multirow{2}{*}{\parbox[t]{2.5cm}{Adjuntar archivos en respuestas}} & WI51 & Implementar la opción de adjuntar archivos en respuestas de correos temporales & 5h & Belen Ramos & Done \\ \cline{3-7}
 &  & WI52 & Pruebas de la funcionalidad de adjuntar archivos & 3h & Belen Ramos& Done \\ \hline

\end{longtable}

**Gestión del Sprint 2 (Tablero Kanban):**

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.

![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)

\newpage

#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/Cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence For Sprint Review*

#### *Execution Evidence for Sprint Review*

#### *Services Documentation Evidence for Sprint Review*

En esta seccion, se muestra la documentacion de los servicios del *backend* de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken*, *Spring Data* y *Flask*

* https://docs.spring.io/spring-boot/index.html

* https://docs.spring.io/spring-boot/reference/web/spring-security.html#page-title

* https://www.npmjs.com/package/jsonwebtoken

* https://spring.io/projects/spring-data-jpa

* https://github.com/flasgger/flasgger

#### *Software Deployment Evidence for Sprint Review*

\newpage

#### *Team Collaboration Insights during Sprint*

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1/views/2)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-2.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-3.png)

\newpage

## *Validation Interviews*

Las entrevistas de validación son una herramienta clave en el proceso de diseño centrado en el usuario. A través de estas entrevistas, se busca obtener información directa de los usuarios sobre cómo interactúan con el producto, lo que permite validar su usabilidad y funcionalidad. Este método es esencial para identificar problemas, detectar oportunidades de mejora y asegurar que el producto final cumpla con las expectativas del público objetivo. Las entrevistas de validación no solo ayudan a mejorar la experiencia del usuario, sino que también garantizan que las decisiones de diseño estén basadas en datos reales y no en suposiciones.

A continuación, exploraremos cómo se diseñaron las entrevistas, cómo se llevó a cabo el registro de las mismas y las evaluaciones realizadas basadas en principios heurísticos.

### Diseño de entrevistas

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


### Registro de entrevistas

### Evualuaciones segun heuristicas

