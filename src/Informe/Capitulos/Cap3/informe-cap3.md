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

# Capítulo III: **Arquitectura**

## ***Product design***

El diseño de producto es un aspecto fundamental que influye directamente en la percepción, usabilidad y éxito de cualquier aplicación o solución tecnológica. A través de un enfoque cuidadoso en los principios del diseño, buscamos crear un producto que no solo cumplan con las necesidades funcionales de los usuarios, sino que también brinde una experiencia visualmente atractiva y consistente. En las siguientes secciones, se detallan las pautas específicas que seguimos para garantizar la coherencia en el diseño.

### **Style Guidelines**

![Artefacto creado en Figma](src/img/Cap3/Style_Guidelines.png)

Las directrices de estilo juegan un rol crucial en la creación de una identidad visual sólida y coherente en el diseño de productos. Estas guías permiten establecer estándares comunes que aseguran que todos los elementos visuales sigan un patrón uniforme. A continuación, se presentan las pautas generales que seguimos para mantener una coherencia visual en nuestros productos.


#### **General Style Guidelines**


El diseño visual es uno de los aspectos fundamentales para crear una experiencia de usuario coherente, intuitiva y atractiva. Establecer pautas claras sobre la identidad de marca, la paleta de colores, la tipografía y el tono de comunicación es esencial para garantizar que cada interacción con el producto sea consistente y efectiva. 

\begin{quote}
Según Goodwin (2019), un diseño claro y sencillo facilita que los usuarios se enfoquen en sus objetivos sin encontrarse con obstáculos innecesarios, lo que optimiza la usabilidad del producto.
\end{quote}

\vspace{1em}

Estas guías no solo refuerzan los valores de simplicidad y accesibilidad, sino que también aseguran que el diseño sea flexible, adaptable y atractivo para una amplia variedad de usuarios. A continuación, se explicarán los elementos clave de diseño que sustentan nuestra visión de ofrecer una experiencia de usuario impecable y una identidad visual sólida.

\vspace{2em}

**Branding:**

*Temporaly* es una herramienta diseñada específicamente para proteger la información de los estudiantes en el mundo digital. Su principal objetivo es proporcionar una solución práctica y temporal que ofrezca a los usuarios la tranquilidad de que sus datos están seguros en todo momento. Nos enfocamos en simplificar la complejidad de la protección de datos, haciendo que Temporaly sea fácil de usar, accesible y altamente eficaz, sin comprometer la seguridad. La esencia de Temporaly radica en combinar tecnología avanzada con una experiencia fluida que resuelva un problema crucial en el día a día de nuestros usuarios: la privacidad.

\vspace{2em}


**Logotipo:**

El logotipo de *Temporaly* captura la simplicidad y la seguridad que representan nuestra app. Su diseño moderno y minimalista refleja el enfoque directo que tenemos para proteger la información de los usuarios sin complicaciones. El color azul vibrante simboliza la confianza y la estabilidad, mientras que la estructura del logotipo transmite una sensación de innovación tecnológica accesible para todos. La elección de colores y formas refuerza el mensaje de una app joven, práctica y confiable que resuelve de manera eficiente las necesidades de seguridad de nuestros usuarios.

![Artefacto creado en Figma](src/img/Cap3/Logos.png)

\vspace{1em}

**Iconografía de la Aplicación**

La iconografía de *Temporaly* incluye el imagotipo de la marca, compuesto por una "T" estilizada en forma de rayo, que simboliza rapidez, eficiencia y la temporalidad de los correos electrónicos temporales que ofrece la app. Este imagotipo se utiliza de manera flexible, tanto en el logo completo de la aplicación como en su icono para dispositivos móviles.


![Artefacto creado en Figma](src/img/Cap3/Icon_App.png)

\vspace{1em}


**Colores**

La paleta de colores de *Temporaly* ha sido seleccionada cuidadosamente para garantizar coherencia visual en toda la interfaz y en las variantes del logotipo y los iconos. Todos los colores utilizados forman parte de la misma paleta, conocida como *Hailey Blue*, lo que asegura una identidad visual armónica.

- **Colores Principales (Interfaz de la Aplicación)**
  
  - **Azul #2979FF (600):** Este es el color principal de la aplicación, utilizado en los botones, la barra de navegación y otros elementos interactivos. Su tono vibrante refuerza la identidad tecnológica y moderna de *Temporaly*, destacando las acciones clave del usuario.
  
  - **Blanco #FFFFFF:** Se utiliza como fondo de los botones y otros elementos de la interfaz, asegurando contraste y legibilidad. Este color permite que el azul principal destaque con claridad.
  
  - **Gris #93868A:** Un tono gris medio transparente que se utiliza para textos sobre fondos semi-transparentes, aportando un estilo moderno y minimalista.
  
  - **Negro #000000:** Utilizado para textos en algunas secciones clave de la interfaz, proporciona contraste y asegura la legibilidad en los elementos más importantes.
  
  ![Artefacto creado en Figma](src/img/Cap3/PrimaryColors.png)


- **Colores Secundarios (Variantes de Logos e Iconos)**
  Las variantes del logotipo e icono utilizan otros tonos dentro de la misma paleta *Hailey Blue*, lo que refuerza la cohesión visual de la marca:

  - **Azul #256CE4 (700):** Este tono complementa al color principal en algunas versiones del logotipo, proporcionando flexibilidad visual en distintas situaciones.
  
  - **Azul #205EC6 (800):** Un tono más profundo utilizado en algunas variantes del logotipo y los iconos. Ofrece una opción más seria y formal sin perder la relación visual con el color principal.
  
  - **Azul Oscuro #123672 (1000):** Este tono de azul oscuro se utiliza en otras variantes del logotipo, aportando un contraste elegante y sofisticado en ciertas aplicaciones gráficas.
  
  ![Artefacto creado en Figma](src/img/Cap3/SecondColors.png)

\vspace{1em}

**Tipografía**

La tipografía en *Temporaly* es clave para asegurar una experiencia visual coherente, moderna y fácil de leer. Cada fuente seleccionada cumple una función específica en la aplicación y en la landing page, aportando claridad y accesibilidad.

- ***Urbanist* (Google Fonts)**
  
  - Peso utilizado: *Medium*
  
  La tipografía *Urbanist* se utiliza principalmente en los títulos, encabezados y secciones destacadas dentro de la app. Su estilo moderno y minimalista asegura que los elementos clave de la interfaz sean reconocibles y accesibles, reforzando la identidad tecnológica y accesible de *Temporaly*.

  ![Artefacto creado en Figma](src/img/Cap3/Typography_Urbanist.png)


- ***Work Sans* (Google Fonts)**
  
  - Pesos utilizados: *Bold* y *Regular*
  
  Work Sans es la tipografía utilizada en el cuerpo del texto y en los botones de acción dentro de la app. La versión Bold se usa para resaltar acciones clave, mientras que la versión Regular asegura una legibilidad fluida en el contenido principal.

  ![Artefacto creado en Figma](src/img/Cap3/Typography_WorkSans.png)

- ***Inter* (Google Fonts)**
  
  - Pesos utilizados: Variantes de *Regular* y *Bold*
  
  Para la landing page de *Temporaly*, se utiliza Inter, una tipografía altamente funcional y legible en entornos web. Su estilo limpio y moderno garantiza que la información en la landing page sea clara, accesible y alineada con el diseño general de la marca.

  ![Artefacto creado en Figma](src/img/Cap3/Typography_Inter.png)

\vspace{1em}

**Tonos de Comunicación**

El tono de voz de *Temporaly* está diseñado para alinearse con su audiencia principal, compuesta por estudiantes de distintos niveles educativos, y reflejar los valores de la aplicación: simplicidad, accesibilidad y confianza. A continuación, se describen las características principales del tono de comunicación:

- **Casual:** El tono empleado en las comunicaciones de Temporaly es cercano y accesible, permitiendo que los estudiantes se sientan cómodos al interactuar con la app sin una formalidad excesiva.

- **Respetuoso:** A pesar de su naturaleza casual, Temporaly mantiene un tono respetuoso, reconociendo la importancia de la privacidad y seguridad de los datos personales de los usuarios.

- **Relajado:** El uso de un tono relajado busca transmitir tranquilidad y eliminar cualquier complejidad innecesaria, facilitando que los usuarios utilicen la app sin preocupaciones.

- **Amigable:** La aplicación utiliza un lenguaje amigable para generar una conexión cercana y confiable con los usuarios, lo que les anima a explorar y utilizar la app de manera eficiente.

- **Neutral:** En comunicaciones más informativas, como explicaciones técnicas o detalles sobre seguridad, se emplea un tono neutral para mantener la claridad y objetividad.

Estas características del tono de voz han sido diseñadas para generar confianza en los usuarios, manteniendo un equilibrio entre cercanía y profesionalismo. El tono de comunicación es consistente en todas las plataformas de Temporaly, desde la app hasta la landing page, asegurando una experiencia homogénea.

![Artefacto creado en Figma](src/img/Cap3/ToneOfVoice.png)

\vspace{1em}

**Eslogan**

El eslogan de Temporaly, "Create, use and forget ;)", refleja perfectamente el enfoque de la app. En pocas palabras, se comunica la simplicidad del servicio: crear un correo temporal, utilizarlo, y olvidarse de él cuando ya no es necesario. El guiño añadido al final " ;)" le da un toque juvenil y relajado, alineado con el tono amigable y cercano que busca la marca.

![Artefacto creado en Figma](src/img/Cap3/Eslogan.png)

\vspace{1em}

### ***Information Architecture***

![Artefacto creado en Canva](src/img/Cap3/info_arch.png)

La Arquitectura de la Información (AI) organiza y estructura el contenido en sistemas digitales, permitiendo a los usuarios navegar de manera eficiente y acceder a lo que necesitan sin dificultades. Una buena AI alinea las necesidades del usuario con los objetivos del negocio, optimizando la experiencia de uso.

\begin{quote}
Como describe Rosenfeld et al. (2015), una buena arquitectura de la información no solo ayuda a los usuarios a orientarse, sino que también optimiza la experiencia general del producto, haciéndola más intuitiva y eficiente.
\end{quote}

\vspace{1em}

En esta sección, se exploran los principios y estrategias que hemos aplicado en Temporaly para organizar su contenido de manera lógica, coherente y accesible, garantizando que los usuarios puedan navegar por la aplicación sin dificultades y encontrar la información que buscan de manera rápida y sencilla.


#### ***Organization Systems***

Los usuarios pueden navegar por la interfaz de *Temporaly* de manera clara y efectiva, gracias a su estructura organizativa optimizada para la protección de datos temporales.

\begin{tabular}{|l|p{11cm}|}
\hline
\textbf{Tópico} & \textbf{Definición} \\
\hline
\textbf{Email Management} & Administración de correos temporales de manera rápida, permitiendo la creación, uso y eliminación de correos electrónicos desechables. \\
\hline
\textbf{User Authentication} & Implementación de métodos de autenticación como inicio de sesión con terceros (Google, Facebook) y autenticación biométrica (huella dactilar). \\
\hline
\textbf{Inbox Organization} & Organización de correos electrónicos en categorías como activos e inactivos para facilitar la gestión y el acceso. \\
\hline
\textbf{Security Protocols} & Uso de tecnologías avanzadas para proteger los datos temporales generados por los usuarios, garantizando la privacidad. \\
\hline
\textbf{User-Friendly Navigation} & Diseño de una interfaz sencilla con un menú lateral y navegación clara para mejorar la experiencia de usuario. \\
\hline
\textbf{Email History} & Registro completo del historial de correos electrónicos temporales generados, categorizados por estado (activo o inactivo). \\
\hline
\textbf{Data Deletion} & Proceso fácil de eliminación de cuentas y datos de usuarios, asegurando que toda la información temporal sea eliminada de manera permanente. \\
\hline
\end{tabular}

\vspace{1em}

La estructura organizativa de *Temporaly* está diseñada para ofrecer una experiencia de usuario eficiente, centrada en la seguridad y facilidad de uso. Cada sistema ha sido implementado con el objetivo de simplificar la gestión de correos temporales y garantizar que los usuarios puedan proteger su información personal de manera efectiva. Esta organización clara permite que los usuarios interactúen con la aplicación de manera intuitiva, sin complicaciones.


#### ***Labelling Systems***

Los sistemas de etiquetado en *Temporaly* se han diseñado para que los usuarios puedan navegar de manera eficiente a través de la aplicación con una terminología clara y coherente. Cada etiqueta, botón y sección ha sido nombrada para que los usuarios puedan comprender de inmediato su función o propósito.

\begin{tabular}{|l|p{13cm}|}
\hline
\textbf{Etiqueta} & \textbf{Descripción} \\
\hline
\textbf{Sign In} & Etiqueta utilizada para que los usuarios accedan a la aplicación con sus credenciales de inicio de sesión o cuentas externas como Google o Facebook. \\
\hline
\textbf{New Email} & Etiqueta para crear un nuevo correo temporal en la plataforma de manera rápida y sencilla. \\
\hline
\textbf{Delete Email} & Etiqueta que permite eliminar un correo temporal una vez que ya no se necesita. \\
\hline
\textbf{Email History} & Etiqueta que muestra el historial de correos electrónicos generados por el usuario, organizados por estado (activo o inactivo). \\
\hline
\textbf{Settings} & Etiqueta que proporciona acceso a las configuraciones de la cuenta del usuario, incluyendo la eliminación de cuentas o cambios en las notificaciones. \\
\hline
\textbf{Sign Up} & Etiqueta que guía a los usuarios para crear una cuenta nueva en la aplicación. \\
\hline
\textbf{Inbox} & Etiqueta que indica la sección principal donde los correos temporales activos e inactivos son visibles. \\
\hline
\end{tabular}

\vspace{1em}

#### ***SEO Tags and Meta Tags***

En la aplicación *Temporaly*, los SEO Tags y Meta Tags juegan un rol crucial en la optimización de la visibilidad de la aplicación en motores de búsqueda y en proporcionar información esencial para su correcto funcionamiento en entornos web. Aunque *Temporaly* es principalmente una aplicación móvil, la landing page y cualquier página relacionada con el servicio puede beneficiarse enormemente del uso correcto de estas etiquetas.

**SEO Tags**

Los SEO (Search Engine Optimization) Tags son utilizados para mejorar el posicionamiento de la landing page de Temporaly en motores de búsqueda como *Google*. Algunos ejemplos de *SEO Tags* utilizados incluyen:

- **Title Tag:** Especifica el título de la página que aparece en los resultados de búsqueda.

::: norm
```html
   <title>Temporaly - Protección Temporal de Datos para Estudiantes</title>
```
:::

- **Meta Description:** Proporciona un breve resumen del contenido de la página para los motores de búsqueda.

::: norm
```html
   <meta name="description" content="Temporaly es una aplicación que permite la creación de correos temporales para proteger tu información personal de forma rápida y segura." />
```
:::

- **Header Tags (H1, H2, H3):** Estas etiquetas son utilizadas para estructurar el contenido y mejorar la jerarquía de la información en la *landing page*.

::: norm
```html
   <h1>Protege tu Privacidad con Correos Temporales</h1>
```
:::

**Meta Tags**

Los *Meta Tags* son etiquetas que proporcionan información adicional sobre la página web al navegador y a los motores de búsqueda. Estas etiquetas no afectan directamente al contenido visible por los usuarios, pero son esenciales para mejorar la experiencia en la web y optimizar el posicionamiento SEO. Algunos ejemplos de Meta Tags utilizados en Temporaly son:

- **Charset Meta Tag:** Define el conjunto de caracteres que la página está utilizando, esencial para evitar errores de visualización.
  
::: code
```html
   <meta charset="UTF-8">
```
:::

- **Viewport Meta Tag:** Asegura que la página se vea bien en dispositivos móviles.

::: code
```html  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
```
:::

**Robots Meta Tag:** Indica a los motores de búsqueda si deben o no indexar la página.

::: code
```html  
   <meta name="robots" content="index, follow">
```
:::

**Canonical Tag:** Evita contenido duplicado al especificar la URL principal.

::: code
```html 
    <link rel="canonical" href="https://temporaly.com">
```
:::

Además de estas etiquetas clave, para la optimización específica de Temporaly como una aplicación móvil, se pueden añadir las siguientes etiquetas, especialmente en la landing page para maximizar la visibilidad y facilitar el acceso a la descarga de la app:

**Landing Page SEO Tags (para la aplicación móvil):**

- **Title:** Temporaly | Protección Temporal de Datos en tu Móvil
- **Description:** Temporaly - Crea correos temporales directamente desde tu móvil para proteger tu información personal de manera rápida y segura. Disponible para iOS y Android.
- **Keywords:** correos temporales, app móvil, protección de datos, privacidad, seguridad, estudiantes.
- **Author:** CodeMinds
- **Canonical:** https://temporaly.com/

**Meta Tags adicionales para la landing page:**

- **og(Open Graph):** Temporaly | Protección Temporal de Datos
- **og(Open Graph):** Temporaly te permite crear correos temporales directamente desde tu dispositivo móvil, disponible en las tiendas de apps.
- **og(Open Graph):** https://temporaly.com/assets/logo.png
- **og(Open Graph):** https://temporaly.com/
- **app-download-url:**
  - Android: https://play.google.com/store/apps/details?id=com.temporaly
  - iOS: https://apps.apple.com/app/temporaly/id123456789

El uso adecuado de SEO Tags y Meta Tags garantiza que la landing page de Temporaly tenga un mayor alcance y visibilidad en los motores de búsqueda, permitiendo a los usuarios encontrar rápidamente la aplicación y acceder a sus servicios. Asimismo, estas etiquetas aseguran una experiencia optimizada para los usuarios que acceden desde dispositivos móviles, facilitando la descarga y el uso de la aplicación.


#### ***Searching Systems***

El sistema de búsqueda de Temporaly está diseñado para ofrecer una experiencia de usuario eficiente y sencilla, permitiendo a los usuarios acceder rápidamente a la información que necesitan. Dado que Temporaly es una aplicación enfocada en la generación y gestión de correos electrónicos temporales, los mecanismos de búsqueda dentro de la app son clave para la organización y recuperación de la información.

\begin{tabular}{|l|p{10cm}|}
\hline
\textbf{Filtro} & \textbf{Definición} \\
\hline
\textbf{Email Address} & Filtro que permite buscar los correos electrónicos temporales generados por dirección de correo. \\
\hline
\textbf{Creation Date} & Filtro que permite buscar los correos según la fecha en que fueron generados en la plataforma. \\
\hline
\textbf{Active/Inactive Status} & Filtro que permite visualizar los correos según su estado: activos o inactivos. \\
\hline
\textbf{Duration} & Filtro que permite buscar correos según el tiempo de validez seleccionado al momento de su creación (10, 30 o 60 minutos). \\
\hline
\textbf{Advanced Search} & Opciones avanzadas de búsqueda que permiten combinar múltiples criterios como correo electrónico, estado y duración para obtener resultados más precisos. \\
\hline
\end{tabular}

\vspace{1em}

El sistema de búsqueda está optimizado para asegurar que el usuario no pierda tiempo en la gestión de sus correos temporales y pueda acceder a la información de manera inmediata.

#### ***Navigation Systems***

El sistema de navegación en Temporaly está diseñado para ser intuitivo y accesible, ofreciendo a los usuarios una experiencia de uso fluida y sin complicaciones. La estructura de navegación asegura que los usuarios puedan desplazarse fácilmente entre las diferentes funcionalidades de la aplicación, optimizando la interacción y minimizando el tiempo de aprendizaje.

\begin{tabular}{|l|p{10cm}|}
\hline
\textbf{Nombre} & \textbf{Definición} \\
\hline
\textbf{Menú Lateral} & Despliega opciones principales de navegación como Home, Contact Us, About Us, Terms and Conditions, y Settings, permitiendo una navegación rápida entre las diferentes secciones de la aplicación. \\
\hline
\textbf{Barra de Navegación Inferior} & Proporciona acceso rápido a las funciones clave como Email (bandeja de entrada) y History (historial de correos generados), mejorando la accesibilidad a las características más utilizadas. \\
\hline
\textbf{Email} & Vista principal de los correos electrónicos temporales activos y la opción de crear, actualizar o eliminar correos desde esta sección. \\
\hline
\textbf{History} & Historial de todos los correos temporales creados por el usuario, organizados según su estado (activo o inactivo). \\
\hline
\textbf{Settings} & Opciones de configuración de la cuenta del usuario, incluyendo ajustes de notificaciones, cierre de sesión y eliminación de cuenta. \\
\hline
\end{tabular}


\vspace{1em}


### ***Domain-Driven Software Architecture***

#### ***Software Architecture Context Level Diagram***

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Contexto.png)

#### ***Software Architecture Container Level Diagram***

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Contenedores.png)

#### ***Software Architecture Components Diagram***

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Componentes.png)

### ***Software Object-Oriented Design****

#### ***Class Diagrams***
Nuestro dominio se divide en 4 Bounded Contexts:

1.- **Login Bounded Context**: Centrado en los actores/usuarios que se autentican en la solución y la gestión del proceso de login y logout.

2.- **Profile Settings Bounded Context**: Centrado en los cambios de configuración del perfil de los usuarios, incluyendo preferencias, ajustes y personalización.

3.- **Privacy Policy Bounded Context**: Centrado en la gestión de las políticas de privacidad y la obtención o revocación de consentimiento por parte de los usuarios.

4.- **Email History Management Bounded Context**: Centrado en el registro y seguimiento del historial de acciones de correo electrónico realizadas por el sistema y los usuarios.

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/iam_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/email_management_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/profile_settings_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/privacy_policy_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/email_history_bc.jpeg)

#### ***Class Dictionary***

##### ***Email History Management Bounded Context***

- ***EmailHistoryManagementContext***

  - ***`retrieveEmailHistory(userId: String): List<EmailHistory>`***: Recupera el historial de correos electrónicos de un usuario específico.
    
  - ***`logEmailEvent(userId: String, email: String, action: String): void`***: Registra un evento de correo electrónico (como la creación o expiración de un correo temporal).

- ***EmailHistory***

  - ***`id: String`***: Identificador único del historial del correo electrónico.
    
  - ***`email: String`***: Dirección de correo electrónico asociada al historial.
    
  - ***`action: String`***: Acción tomada (como creación, expiración).
    
  - ***`timestamp: Date`***: Marca de tiempo del evento registrado.
    
  - ***`logEmailAction(email: String, action: String): void`***: Registra una acción específica realizada sobre el correo electrónico.
    
  - ***`getHistory(): List<EmailHistory>`***: Devuelve una lista de los eventos de correo electrónico registrados.

#####  ***Email Management Bounded Context***

- ***EmailManagementContext***

  - ***`handleTemporaryEmailCreation(): void`***: Gestiona la creación de correos electrónicos temporales.
    
  - ***`handleTemporaryEmailExpiration(): void`***: Gestiona la expiración de correos electrónicos temporales.

  **TemporaryEmail**
  - ***`tempId: String`***: Identificador único para el correo temporal.
    
  - ***`creationDate: Date`***: Fecha de creación del correo temporal.
    
  - ***`getTempId(): String`***: Obtiene el identificador del correo temporal.
    
  - ***`getCreationDate(): Date`***: Obtiene la fecha de creación del correo temporal.
    
  - ***`expireEmail(): void`***: Expira el correo temporal.

- ***Email***

  - ***`id: String`***: Identificador único del correo electrónico.
    
  - ***`email: String`***: Dirección del correo electrónico.
    
  - ***`expirationDate: Date`***: Fecha de expiración del correo electrónico.
    
  - ***`createEmail(): Email`***: Crea una nueva instancia de correo 
  electrónico.

  - ***`getId(): String`***: Obtiene el identificador del correo electrónico.
    
  - ***`getEmail(): String`***: Obtiene la dirección de correo electrónico.
    
  - ***`getExpirationDate(): Date`***: Obtiene la fecha de expiración del correo electrónico.

##### ***Login Bounded Context (Identity and Access Management)***

- ***User***

  - ***`username: String`***: Nombre de usuario.
    
  - ***`info: UserInfo`***: Información adicional del usuario.
    
  - ***`roles: Set<Role>`***: Conjunto de roles asignados al usuario.
    
  - ***`email: String`***: Dirección de correo electrónico del usuario.
    
  - ***`password: String`***: Contraseña del usuario.
    
  - ***`id: String`***: Identificador único del usuario.
    
  - ***`getId(): String`***: Devuelve el identificador del usuario.
    
  - ***`getUsername(): String`***: Devuelve el nombre de usuario.
    
  - ***`getEmail(): String`***: Devuelve la dirección de correo electrónico del usuario.
    
  - ***`getPassword(): String`***: Devuelve la contraseña del usuario.
    
  - ***`getRoles(): Set<Role>`***: Devuelve el conjunto de roles asignados.
    
  - ***`getInfo(): UserInfo`***: Devuelve la información del usuario.
    
  - ***`getFullName(): String`***: Devuelve el nombre completo del usuario.

- ***UserInfo***

  - ***`lastNames: List<String>`***: Apellidos del usuario.
    
  - ***`names: List<String>`***: Nombres del usuario.
    
  - ***`getNames(): List<String>`***: Devuelve una lista con los nombres del usuario.
    
  - ***`getLastNames(): List<String>`***: Devuelve una lista con los apellidos del usuario.
    
  - ***`setNames(List<String>): void`***: Establece los nombres del usuario.
    
  - ***`setLastNames(List<String>): void`***: Establece los apellidos del usuario.
    
  - ***`equals(Object): boolean`***: Compara dos objetos UserInfo.
    
  - ***`canEqual(Object): boolean`***: Verifica si dos objetos pueden ser iguales.
    
  - ***`hashCode(): int`***: Devuelve el código hash del objeto.

  - ***`toString(): String`***: Convierte el objeto en cadena de texto.

- ***Role***

  - ***`id: String`***: Identificador único del rol.
    
  - ***`name: Roles`***: Nombre del rol.
    
  - ***`toRoleFromName(String): Role`***: Convierte el nombre en un objeto Role.
    
  - ***`getId(): String`***: Devuelve el identificador del rol.
    
  - ***`getName(): Roles`***: Devuelve el nombre del rol.
    
  - ***`getDefaultRole(): Role`***: Devuelve el rol por defecto.

##### ***Privacy Policy Bounded Context***

- ***PrivacyPolicyBoundedContext***

  - ***`manageUserConsent(): void`***: Gestiona el consentimiento del usuario para las políticas de privacidad.
    
  - ***`updatePrivacyPolicy(): void`***: Actualiza las políticas de privacidad.

- **PrivacyPolicy**

  - ***`id: String`***: Identificador único de la política de privacidad.
    
  - ***`policyText: String`***: Texto de la política de privacidad.
    
  - ***`lastUpdated: Date`***: Fecha de la última actualización de la política.
    
  - ***`getPolicy(): String`***: Devuelve el texto de la política de privacidad.
    
  - ***`updatePolicy(String): void`***: Actualiza el texto de la política de privacidad.

- **Consent**

  - ***`userId: String`***: Identificador del usuario que ha dado o no su consentimiento.
    
  - ***`consentGiven: boolean`***: Indica si el usuario ha dado su consentimiento.
    
  - ***`giveConsent(): void`***: Otorga el consentimiento del usuario.
    
  - ***`revokeConsent(): void`***: Revoca el consentimiento del usuario.
    
  - ***`hasGivenConsent(): boolean`***: Verifica si el usuario ha dado su consentimiento.


##### ***Profile Settings Bounded Context***

- ***ProfileSettingsBoundedContext***

  - ***`handleUserSettings(): void`***: Gestiona la configuración de usuario.
    
  - ***`updateUserPreferences(): void`***: Actualiza las preferencias del usuario.

- **UserProfile**

  - ***`id: String`***: Identificador único del perfil de usuario.
    
  - ***`username: String`***: Nombre de usuario.
    
  - ***`email: String`***: Dirección de correo electrónico del usuario.
    
  - ***`preferences: Map<String, String>`***: Preferencias del usuario.
    
  - ***`updateProfile(): void`***: Actualiza el perfil del usuario.
    
  - ***`getPreferences(): Map<String, String>`***: Devuelve las preferencias del usuario.
  
  - ***`getUsername(): String`***: Devuelve el nombre de usuario.
    
  - ***`getEmail(): String`***: Devuelve la dirección de correo electrónico del usuario.

- ***UserSettings***

  - ***`theme: String`***: Tema seleccionado por el usuario.
    
  - ***`notificationsEnabled: boolean`***: Indica si las notificaciones están habilitadas.
    
  - ***`getSettings(): Map<String, String>`***: Devuelve la configuración del usuario.
    
  - ***`updateSettings(Map<String, String>): void`***: Actualiza la configuración del usuario.


#### ***Database Design***

![Class diagram Temporaly, imagen creada en Mermaid](src/img/Cap3/database_desing.png)

#### ***Database Diagram***

![Class diagram Temporaly, imagen creada en Mermaid](src/img/Cap3/database_diagram.png)