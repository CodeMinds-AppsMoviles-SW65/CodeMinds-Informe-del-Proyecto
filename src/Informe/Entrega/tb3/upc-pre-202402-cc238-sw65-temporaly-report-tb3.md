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
bibliography: src/Informe/Entrega/tb3/bibliografia.bib
csl: src/Informe/Entrega/tb3/apa.csl
book: true
classoption: oneside
code-block-font-size: \scriptsize
nocite: |
  @gothelf2021,
  @hernandez2018,
  @kasparova2022,
  @kalbach2016,
  @smith2020,
  @johnson2019,
  @brown2022,
  @igartua2019desconexion,
  @jiang2024pervasive,
  @kaspersky_privacy,
  @collave2024datos
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

**Registro de Versiones del Informe**

\begin{longtable}{|c|c|c|p{6cm}|}
  \hline
  \textbf{Versión} & \textbf{Fecha} & \textbf{Autor} & \textbf{Descripción de Modificación} \\
  \hline
  tb1 & 27/08/2024 & Ortega Huaraca, Abel & Ayudé con la estructura del informe en general. Respecto a los puntos específicos, contribuí con la elaboración del \textit{Solution Profile}, \textit{Startup Profile}, Segmentos objetivo, \textit{User Stories} y una introducción para los \textit{Requirements Specification}. \\
  \hline
  tb1 & 27/08/2024 & Ramos Rios, Belén del Rocio & Realice la descripción de competidores, análisis competitivo y las estrategias frente a competidores. También aporté en la creación de los \textit{User Journey Mapping}, \textit{To-Be Scenario Mapping} y el \textit{Product Backlog}. \\
  \hline
  tb1 & 27/08/2024 & Vilchez Rios, Mateo Alejandro & Capitulo 1: \textit{Lean UX Process} - Antecendetes y Problemática, Capitulo 2: Registro de Entrevista - \textit{Empathy Map} - \textit{As-is} - \textit{Scenario Mapping} - \textit{Impact Mapping}. \\
  \hline
  tb1 & 27/08/2024 & Avila Asto, Alex Ramon Alberto & Realicé el análisis de entrevistas, \textit{netfinding}, la creación de \textit{User Personas} y la tabla de \textit{User Task Matrix}. \\
  \hline
  tb2 & 14/09/2024 & Vilchez Rios, Mateo Alejandro & Capitulo 3: \textit{Landing Page UI Design} - \textit{Architecture Overview} - \textit{Class Dictionary}, Capitulo 4: \textit{Sofware Configuration Management} - \textit{Testing Suite Evidence for Sprint Review}\\
  \hline
  tb2 & 15/09/2024 &  Ramos Rios, Belen del Rocio & Capitulo 3: \textit{Style Guidelines} - \textit{Information Arhitecture} - \textit{Landing Page UI Design}, Capitulo 4: \textit{Sprint Backlog 1}\\
  \hline
  tb2 & 15/09/2024 & Ortega Huaraca, Abel Angel & Capitulo 4: Realicé el desarrollo del diseño de los wireframes de la aplicación y los prototipos \\
  \hline
  tb2 & 15/09/2024 & Avila Asto, Alex Ramon Alberto & Realicé la implementación del diseño y despliegue del backend \\
\hline
  tp & 28/09/2024 & Vilchez Rios, Mateo Alejandro & Capitulo 5: \textit{Landing Page UI Implementation} - \textit{Architecture Overview} - \textit{Class Dictionary}, Capitulo 5: Realicé la implementación del bounded context \textit{Privacy Policy}. \\
  \hline
  tp & 28/09/2024 &  Ramos Rios, Belen del Rocio &  Capitulo 5: \textit{Sprint Backlog 2} - \textit{Validation Interviews} - Realicé la implementación del bounded context \textit{Privacy Policy}.\\
  \hline
  tp & 28/09/2024 & Ortega Huaraca, Abel Angel & Capitulo 5: Realicé el diseño y desarrollo del bounded context \textit{Temporary Email Management}  \\
  \hline
  tp & 28/09/2024 & Avila Asto, Alex Ramon Alberto & Capitulo 5: Realicé la implementación del diseño y despliegue del backend de autenticación. Asimismo realicé la implementación del bounded context \textit{Login}. \\
  \hline
  tb3 & 25/10/2024 & Vilchez Rios, Mateo Alejandro & Capitulo 5: \textit{Landing Page UI Implementation} - \textit{Architecture Overview} - \textit{Class Dictionary}, Capitulo 5: Realicé la reimplementación del bounded context \textit{Privacy Policy} para \textit{Flutter}. \\
  \hline
  tb3 & 25/10/2024 &  Ramos Rios, Belen del Rocio &  Capitulo 5: \textit{Sprint Backlog 2} - \textit{Validation Interviews} - Realicé la reimplementación del bounded context \textit{Privacy Policy} para \textit{Flutter}.\\
  \hline
  tb3 & 25/10/2024 & Ortega Huaraca, Abel Angel & Capitulo 5: Realicé el diseño y desarrollo del bounded context \textit{Temporary Email Management} para \textit{Flutter} \\
  \hline
  tb3 & 25/10/2024 & Avila Asto, Alex Ramon Alberto & Capitulo 5: Realicé la implementación del diseño y despliegue del backend de autenticación. Asimismo realicé la reimplementación del bounded context \textit{Login} para \textit{Flutter}. \\
\bottomrule
\end{longtable}

\newpage

***Student Outcome***

El curso contribuye al cumplimiento del ***Student Outcome ABET:*** *ABET-EAC - Student Outcome 7*

* **Criterio:** *La capacidad de adquirir y aplicar nuevos conocimientos según sea necesario, utilizando estrategias de aprendizaje apropiadas*.

En el siguiente cuadro se describe las acciones realizadas y enunciadas de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro de ***ABET - EAC - Student Outcome 7.***

\begin{longtable}{|p{4cm}|p{6cm}|p{5cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{Criterio Específico}} & \multicolumn{1}{c|}{\textbf{Acciones Realizadas}} & \multicolumn{1}{c|}{\textbf{Conclusiones}} \\
\hline
\endfirsthead
\multirow{2}{*}{
\parbox[t]{4cm}{
\textit{Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.}
}
}
&  
\parbox[t]{6cm}{
\textbf{TB1:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Coordiné y realicé la reunión inicial del proyecto, explicando claramente los objetivos y el plan de trabajo. Cree diferentes reuniones para clarificar los roles de cada integrante del equipo y organicé los flujos de trabajas de un tablero Kanban (Scrum). Respecto al informe, culminé en tiempo y forma las pendientes que se me asignaron. \\
\textbf{Belen del Rocio Ramos Rios} \\
Utilicé nuevas herramientas para documentar el informe y amplié mis conocimientos en áreas clave como User Journey Mapping y análisis competitivo. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Aprendí nuevas herramientas para mejorar la documentación del informe y profundicé en la metodología Lean UX para aplicarla en nuestro proyecto. \\
\textbf{Alex Avila Asto} \\
Utilicé nuevas herramientas para la elaboración del informe y mejoré mis habilidades en el reconocimiento de puntos clave para la creación de User Personas y User Task Matrix. Estas actividades han optimizado mi comprensión del usuario y el enfoque del proyecto, fortaleciendo mi desarrollo profesional y alineando mejor las soluciones con las necesidades reales de los usuarios.
\\} 
&
\parbox[t]{5cm}{
\textbf{TB1:} \\
Como grupo, nos hemos comprometido a mantenernos en constante actualización de los conceptos y conocimientos necesarios para nuestro desarrollo profesional, especialmente en el ámbito de los proyectos de soluciones de software. A lo largo de este proceso, hemos aprendido a implementar nuevas herramientas y metodologías que no solo han fortalecido nuestras habilidades individuales, sino que también han potenciado el éxito del proyecto en su conjunto.
En conjunto, hemos demostrado que nuestro compromiso con el aprendizaje continuo y la aplicación de nuevas estrategias es fundamental para garantizar el éxito de nuestro proyecto. Este proceso nos ha permitido no solo crecer como profesionales, sino también asegurar que nuestras soluciones de software sean relevantes, eficientes y estén perfectamente alineadas con las necesidades reales de los usuarios. \\
} \\ 

\cline{2-3}

&  
\parbox[t]{6cm}{
\textbf{TB2:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Logré reforzar conocimientos clave en herramientas de prototipado y flujos de interacción, esenciales para mi desarrollo profesional en soluciones de software. \\
\textbf{Belen del Rocio Ramos Rios} \\
Implementé nuevas herramientas de documentación y desarrollé la arquitectura de información para mejorar la experiencia de usuario. También colaboré en la creación de wireframes y mockups para asegurar la coherencia visual y funcional del proyecto. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Utilicé metodologías ágiles para organizar el flujo de trabajo e implementé mejoras en la UI de la landing page mediante wireframes y mockups, siguiendo las guías de estilo. \\
\textbf{Alex Avila Asto} \\
En esta entrega, desarrollé diagramas de base de datos, clases y despliegue, aplicando conocimientos actualizados en diseño de arquitectura de software. Este proceso me permitió reforzar habilidades clave en modelado y diseño estructural, esenciales para mi desarrollo profesional en soluciones de software. \\
} 
&
\parbox[t]{5cm}{
\textbf{TB2:} \\
En esta segunda entrega, como equipo, nos enfocamos en actualizar y aplicar conceptos clave para el desarrollo de soluciones de software, consolidando nuestros conocimientos en diversas áreas fundamentales del proyecto. Cada miembro contribuyó de manera activa en el diseño y documentación de diferentes aspectos del sistema, incluyendo wireframes, mockups, prototipos, wireflows, y diagramas de base de datos, clases y despliegue. Este proceso no solo nos permitió perfeccionar habilidades técnicas específicas, sino también fortalecer nuestra capacidad para trabajar de manera colaborativa en proyectos complejos.
A través de la implementación de metodologías ágiles, la utilización de herramientas de diseño actualizadas y la estructuración eficaz de la arquitectura de software, hemos logrado un avance significativo en la creación de un producto coherente y alineado con los estándares de la industria. Este enfoque nos ha permitido actualizar los conocimientos necesarios para nuestro desarrollo profesional, aplicando las mejores prácticas en la creación de soluciones de software sólidas y bien documentadas. \\
} \\

\cline{2-3}

&  
\parbox[t]{6cm}{
\textbf{TP:} \\
\textbf{Abel Angel Ortega Huaraca} \\
En esta tercera entrega, participé activamente en el desarrollo del backend, implementando servicios RESTful y asegurando la correcta integración con la aplicación móvil. \\
\textbf{Belen del Rocio Ramos Rios} \\
Colaboré en la optimización de la experiencia del usuario en la app, asegurando una navegación intuitiva y fluida, y contribuyendo a la integración del frontend con el backend de manera efectiva. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Apliqué metodologías ágiles para gestionar las tareas relacionadas con el desarrollo del backend y la aplicación móvil. Implementé funciones clave que permitieron la interacción con los servicios de backend y me aseguré de que las API fueran correctamente consumidas por la aplicación. \\
\textbf{Alex Avila Asto} \\
Participé en la conexión y despliegue de la aplicación móvil, garantizando la integración y comunicación efectiva entre ambas partes de la solución de software. Este proceso reforzó mis habilidades en arquitectura de sistemas y desarrollo full-stack. \\
} 
&
\parbox[t]{5cm}{
\textbf{TP:} \\
En esta tercera entrega, el equipo se centró en el desarrollo del backend y la aplicación móvil, integrando funcionalidades clave que permitieron un flujo de datos eficiente y una experiencia de usuario mejorada. Cada miembro asumió roles específicos en la implementación de servicios, controladores y la integración entre las capas del sistema, aplicando los conocimientos adquiridos en tecnologías backend y desarrollo móvil. \\
Mediante el uso de metodologías ágiles y la colaboración activa, logramos una implementación exitosa que permitió la correcta comunicación entre el backend y la aplicación móvil, cumpliendo con los estándares de la industria. Este enfoque contribuyó al fortalecimiento de nuestras habilidades en desarrollo de software y la entrega de una solución sólida, escalable y bien documentada, alineada con los objetivos del proyecto. \\
} \\

\cline{2-3}

&  
\parbox[t]{6cm}{
\textbf{TB3:} \\
\textbf{Abel Angel Ortega Huaraca} \\
En esta cuarta entrega, participé activamente en el desarrollo del backend, implementando servicios RESTful y asegurando la correcta integración con la aplicación móvil. \\
\textbf{Belen del Rocio Ramos Rios} \\
Colaboré en la optimización de la experiencia del usuario en la app, asegurando una navegación intuitiva y fluida, y contribuyendo a la integración del frontend con el backend de manera efectiva. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Apliqué metodologías ágiles para gestionar las tareas relacionadas con el desarrollo del backend y la aplicación móvil. Implementé funciones clave que permitieron la interacción con los servicios de backend y me aseguré de que las API fueran correctamente consumidas por la aplicación. \\
\textbf{Alex Avila Asto} \\
Participé en la conexión y despliegue de la aplicación móvil, garantizando la integración y comunicación efectiva entre ambas partes de la solución de software. Este proceso reforzó mis habilidades en arquitectura de sistemas y desarrollo full-stack. \\
} 
&
\parbox[t]{5cm}{
\textbf{TB3:} \\
En esta cuarta entrega, el equipo se centró en el desarrollo del backend y la aplicación móvil, integrando funcionalidades clave que permitieron un flujo de datos eficiente y una experiencia de usuario mejorada. Cada miembro asumió roles específicos en la implementación de servicios, controladores y la integración entre las capas del sistema, aplicando los conocimientos adquiridos en tecnologías backend y desarrollo móvil. \\
Mediante el uso de metodologías ágiles y la colaboración activa, logramos una implementación exitosa que permitió la correcta comunicación entre el backend y la aplicación móvil, cumpliendo con los estándares de la industria. Este enfoque contribuyó al fortalecimiento de nuestras habilidades en desarrollo de software y la entrega de una solución sólida, escalable y bien documentada, alineada con los objetivos del proyecto. \\
} \\

\hline

\multirow{2}{*}{
\parbox[t]{4cm}{
\textit{Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de software.}
}
}
&  
\parbox[t]{6cm}{
\textbf{TB1:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Cree repositorios para almacenar nuestro informe con un registro de versiones constante, además de comenzar un registro de los puntos que nos falta completar.Siempre monitoreando y asesorando a mi equipo acerca de sus avances. \\
\textbf{Belen del Rocio Ramos Rios} \\
Reconocí la necesidad de seguir aprendiendo para optimizar tanto las herramientas de documentación como los procesos de Needfinding para el desarrollo de un producto que se destaque y cumpla con las expectativas de los usuarios. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Reconocí la importancia de actualizarme en herramientas de documentación y profundicé en metodologías ágiles para gestionar mejor el trabajo en equipo. \\
\textbf{Alex Avila Asto} \\
Identifiqué la necesidad de seguir aprendiendo para mejorar mis habilidades en el desarrollo de software, lo que me llevó a explorar nuevas tecnologías y metodologías ágiles. Gracias a esto, pude implementar herramientas más eficientes para la gestión de proyectos y la documentación, lo que facilitó el trabajo en equipo. \\}
&
\parbox[t]{5cm}{
\textbf{TB1:} \\
Como equipo, hemos reconocido la importancia del aprendizaje continuo para nuestro desarrollo profesional y la ejecución exitosa de proyectos en soluciones de software. A lo largo de nuestro trabajo, hemos identificado que la necesidad de actualizar y adquirir nuevos conocimientos es esencial para mejorar nuestras competencias y la calidad de nuestras entregas.
En conjunto, hemos comprendido que el aprendizaje permanente no solo es un requisito para mantenernos actualizados, sino también un pilar que nos permite enfrentar desafíos con soluciones innovadoras y eficientes, garantizando así el éxito y la relevancia de nuestros proyectos.
} \\

\cline{2-3}

&  
\parbox[t]{6cm}{
\textbf{TB2:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Este enfoque me permitió actualizar mis habilidades y adaptarme a nuevas herramientas, esenciales para el desarrollo de proyectos de software y el desempeño profesional en un entorno tecnológico en constante cambio. \\
\textbf{Belen del Rocio Ramos Rios} \\
Reconocí la importancia de seguir aprendiendo sobre herramientas de documentación y optimización, especialmente en gestión de etiquetas SEO y sistemas de búsqueda, para garantizar una landing page organizada y accesible, cumpliendo con los estándares de navegación y experiencia del usuario. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Reconocí la importancia de continuar aprendiendo sobre gestión del código y configuración del entorno de desarrollo, lo que mejoró mis contribuciones al proyecto. Implementé buenas prácticas en gestión de código y despliegue, haciendo el proceso más eficiente y colaborativo. \\
\textbf{Alex Avila Asto} \\
En esta entrega, creé diagramas de base de datos, clases y despliegue, destacando la importancia del aprendizaje continuo en arquitectura de software. Esto me permitió actualizar mis habilidades en modelado y diseño estructural, esenciales para el desarrollo de soluciones de software. \\
}
&
\parbox[t]{5cm}{
\textbf{TB2:} \\
En esta segunda entrega, nuestro equipo ha demostrado un firme compromiso con el aprendizaje permanente, fundamental para el desarrollo profesional y la creación de soluciones de software.
Abel se centró en el diseño de interfaces, adaptándose a nuevas herramientas y técnicas para mejorar el prototipado y la experiencia del usuario. Belén optimizó herramientas de documentación y gestión de etiquetas SEO, asegurando una landing page bien organizada y accesible. Mateo mejoró en la gestión del código fuente y la configuración del entorno de desarrollo, promoviendo la eficiencia y la colaboración en el proyecto. Alex se enfocó en el diseño de diagramas de base de datos y arquitectura, actualizando sus habilidades en modelado estructural.
Juntos, hemos integrado estas actualizaciones y aprendizajes en nuestras contribuciones, reflejando la importancia del aprendizaje continuo para el éxito en proyectos de software y el desarrollo profesional. \\
} \\

\cline{2-3}

&  

\parbox[t]{6cm}{
\textbf{TP:} \\
\textbf{Abel Angel Ortega Huaraca} \\
En esta tercera entrega, me enfoqué en el desarrollo del backend, aprendiendo nuevas tecnologías y herramientas para la creación de servicios RESTful y la integración con la aplicación móvil. Este proceso me permitió adquirir habilidades clave en la gestión de APIs y en el manejo de bases de datos, esenciales para mi crecimiento en el desarrollo de soluciones de software. \\
\textbf{Belen del Rocio Ramos Rios} \\
A través de este trabajo, reforcé mis conocimientos en la comunicación entre la aplicación móvil y los servicios, aplicando mejores prácticas para garantizar un flujo de datos eficiente y una interfaz atractiva y funcional. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Mi aporte en esta entrega se centró en la configuración del entorno de desarrollo para el backend y la aplicación móvil, asegurando una implementación fluida de las funciones y servicios. \\
\textbf{Alex Avila Asto} \\
En esta entrega, participé activamente en la implementación de la arquitectura de backend y la integración con la aplicación móvil, creando servicios y controladores que permitieron la correcta funcionalidad del sistema. \\
} 
&
\parbox[t]{5cm}{
\textbf{TP:} \\
En esta tercera entrega, nuestro equipo se dedicó al desarrollo del backend y la aplicación móvil, integrando conocimientos actualizados en la creación de servicios y en la implementación de una aplicación funcional y bien documentada. \\
Abel se enfocó en el desarrollo de servicios RESTful, adaptándose a nuevas herramientas y tecnologías para asegurar la correcta integración entre las capas del sistema. Belén se centró en el desarrollo y optimización de la aplicación móvil, asegurando una experiencia de usuario mejorada y una comunicación eficiente con el backend. Mateo se dedicó a la gestión y configuración del entorno de desarrollo, facilitando el despliegue y la implementación de las funciones del proyecto. Alex desarrolló la arquitectura del backend y se encargó de la integración con la aplicación móvil, aplicando buenas prácticas de desarrollo full-stack. \\
} \\

\cline{2-3}

&  

\parbox[t]{6cm}{
\textbf{TB3:} \\
\textbf{Abel Angel Ortega Huaraca} \\
En esta cuarta entrega, me enfoqué en el desarrollo del backend, aprendiendo nuevas tecnologías y herramientas para la creación de servicios RESTful y la integración con la aplicación móvil. Este proceso me permitió adquirir habilidades clave en la gestión de APIs y en el manejo de bases de datos, esenciales para mi crecimiento en el desarrollo de soluciones de software. \\
\textbf{Belen del Rocio Ramos Rios} \\
A través de este trabajo, reforcé mis conocimientos en la comunicación entre la aplicación móvil y los servicios, aplicando mejores prácticas para garantizar un flujo de datos eficiente y una interfaz atractiva y funcional. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Mi aporte en esta entrega se centró en la configuración del entorno de desarrollo para el backend y la aplicación móvil, asegurando una implementación fluida de las funciones y servicios. \\
\textbf{Alex Avila Asto} \\
En esta entrega, participé activamente en la implementación de la arquitectura de backend y la integración con la aplicación móvil, creando servicios y controladores que permitieron la correcta funcionalidad del sistema. \\
} 
&
\parbox[t]{5cm}{
\textbf{TB3:} \\
En esta cuarta entrega, nuestro equipo se dedicó al desarrollo del backend y la aplicación móvil, integrando conocimientos actualizados en la creación de servicios y en la implementación de una aplicación funcional y bien documentada. \\
Abel se enfocó en el desarrollo de servicios RESTful, adaptándose a nuevas herramientas y tecnologías para asegurar la correcta integración entre las capas del sistema. Belén se centró en el desarrollo y optimización de la aplicación móvil, asegurando una experiencia de usuario mejorada y una comunicación eficiente con el backend. Mateo se dedicó a la gestión y configuración del entorno de desarrollo, facilitando el despliegue y la implementación de las funciones del proyecto. Alex desarrolló la arquitectura del backend y se encargó de la integración con la aplicación móvil, aplicando buenas prácticas de desarrollo full-stack. \\
} \\

\bottomrule
\end{longtable}

\newpage

**Objetivos** ***SMART***

\begin{longtable}{|>{\centering\arraybackslash}m{4cm}|>{\centering\arraybackslash}m{3cm}|>{\centering\arraybackslash}m{5cm}|>{\centering\arraybackslash}m{3cm}|}
\hline
\multicolumn{4}{|c|}{\textbf{TB1}} \\
\hline
\textbf{\textit{SMART Goals}} & \textbf{Estudiante} & \textbf{Descripción del objetivo} & \textbf{Fechas de entrega} \\
\hline
\endfirsthead

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Específico:} \textit{¿Qué se va a lograr?} \\
El objetivo indica con especificidad, cuál es el proceso, servicio o producto en cuestión, para qué área es relevante, u otro detalle clave que brinde contexto. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Para esta entrega mi objetivo es realizar y dar una estructura detallada al informe con el fin de alcanzar una calidad profesional. Asimismo, entregar en tiempo y forma las puntos que se me encargaron; y coloborar en el proyecto backend a traves del uso de las herramientas designadas en grupo. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Contribuí a la mejora del informe y el proyecto mediante la implementación de herramientas de documentación avanzadas y el desarrollo de sistemas de etiquetado y organización. Esto me permitió adquirir habilidades clave en arquitectura de la información, lo cual es esencial para mi futuro profesional en desarrollo web y diseño de sistemas. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
Mi objetivo en esta entrega fue mejorar la documentación del informe y aplicar correctamente metodologías ágiles, como Lean UX, para asegurar que mi crecimiento en la creación de productos digitales se refleje en el resultado del proyecto. Este conocimiento es relevante para mi carrera, ya que me proporciona habilidades clave en diseño UX/UI y gestión de proyectos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
Para esta entrega, me he centrado en el análisis de entrevistas y la estructuración del informe, asegurando una comprensión profunda de las necesidades del proyecto. En entregas futuras, mi objetivo es contribuir al desarrollo del backend y del móvil de la aplicación, áreas en las que tengo mayor experiencia y fortalezas. Esto permitirá asegurar que ambas partes del proyecto se desarrollen de manera eficiente y estén bien integradas. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Medible:} \textit{¿Tiene KPI o métrica clara?} \\
El enunciado tiene una meta con indicador (KPI) o métrica clara, que determinará si el objetio se cumplió. Idealmente, describe el impacto (lo que vamos a lograr) más que el entregable (lo que vamos a hacer) \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Considero que para esta entrega se establecieron métricas claras. En donde, cada actividad o responsabilidad fue designado y colaborado corractamente. Asimismo, cada punto reflejo un indicador de relevancia y peso en el trabajo del proyecto. Por último, el logro de este primer entregable fue claro; realizar un informe de calidad profesional tanto en contenido como en diseño y estructura. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El éxito se midió por la calidad del informe entregado y la implementación efectiva de mejoras en la arquitectura de la landing page, un paso relevante en mi formación profesional. Esto no solo se refleja en el trabajo del curso, sino que fortalece mis competencias para el ámbito laboral. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alehandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
El éxito de esta entrega se midió por la claridad y coherencia del informe entregado y por la implementación de wireframes y mockups que cumplieron con las expectativas del equipo. Esto refuerza mi capacidad para aplicar herramientas de diseño y gestionar la documentación, habilidades necesarias para mi desarrollo profesional. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El éxito en esta entrega se medirá a través de la calidad y la profundidad del análisis de entrevistas realizado, así como la claridad y cohesión del informe estructurado. En futuras etapas, el éxito se evaluará mediante la eficiencia y calidad del código desarrollado para el backend y la aplicación móvil, utilizando métricas como la tasa de bugs, el tiempo de desarrollo, y la satisfacción del usuario final con la funcionalidad implementada. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Ambicioso:} \textit{¿Es retador y va más allá de sus funciones?} \\
El objetivo inspira y reta a pensar acciones para dar el salto que se requiere para el logro, no se lograría sin una estrategia y un foco potentes. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Considero que el motivar a mi equipo a utilizar herramientas nuevas para la realización de este trabajo, refleja el reto y compromiso con nuestro desenvolvimiento para los objetivos que queremos lograr. Siempre buscando realizar funciones ambiciosas que van mas allá de nuestros conocimientos y que nos inspiran a realizar proyectos con una alta calidad. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Este objetivo me retó a consolidar el aprendizaje de nuevas herramientas y sistemas de etiquetado SEO, habilidades que no dominaba por completo pero que son cruciales para mi crecimiento en diseño y desarrollo de productos digitales. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Este objetivo me desafió a mejorar en áreas como la planificación y organización de sistemas UX. Logré consolidar mi aprendizaje en un entorno práctico, lo que me prepara mejor para futuros proyectos en mi carrera. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
Implementar nuevas herramientas y metodologías en la organización del informe representa un reto significativo y un compromiso con la calidad y eficiencia del proyecto. Este enfoque va más allá de mis funciones actuales, impulsándome a aplicar soluciones innovadoras y a desarrollar tanto el backend como la aplicación móvil con un alto estándar de calidad, superando mis habilidades previas y contribuyendo de manera destacada al éxito del proyecto.  \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Relevante:} \textit{¿Está alineado a la estratégia?} \\
Existe una explicación clara respecto a cómo el objetivo impacta sobre los objetivos estratégicos de la institución o \textit{Laurate} Perú. Brinda una noción del alcance del objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Considero que nuestro trabajo y el resultado de este, reflejan claramente nuestra constancia por cumplir con los objetivos estratégicos establecidos por la institución \textit{Laurate} Perú. En donde, abordamos minuciosamente cada aspecto a través de una planificación del proyecto basada en los lineamientos exigidos por la universidad. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
La mejora en mi habilidad para organizar sistemas de navegación y optimizar la accesibilidad de las interfaces es directamente relevante para mi desarrollo profesional, ayudándome a prepararme mejor para los retos futuros en mi carrera.\\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Mi desarrollo profesional se beneficia de este objetivo, ya que fortalece mi capacidad para trabajar con metodologías ágiles y mejorar mi dominio en diseño de interfaces, habilidades esenciales para el crecimiento en la industria tecnológica. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El informe al que contribuí y mi participación en el proyecto reflejan no solo mi esfuerzo individual, sino también nuestra capacidad colectiva para alinear nuestras acciones con los objetivos estratégicos de \textit{Laurate} Perú. Este trabajo en equipo asegura que cada aspecto del proyecto esté en sintonía con las directrices establecidas por la institución, contribuyendo de manera efectiva al cumplimiento de sus metas estratégicas. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Tiempo Límite:} \textit{¿Cuándo se cumplirá?} \\
En caso que la expectativa de fecha de cumplimiento sea previa al cierre de año, el enunciado contiene de forma explícita la fecha límite para alcanzar el objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Para esta entrega, he cumplido satisfactoriamente con la colaboración y entrega de mis responsabilidades en conjunto con mi equipo de trabajo. Las fechas límite estuvieron establecidas claramente desde el inicio, por lo pude cumplir en tiempo y forma con mis deberes; y a su vez, colaborar con mi equipo siempre que se presentó una dificultad o tarea que involucrara a todos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Logré cumplir el objetivo a tiempo, entregando todos los avances el 28 de agosto de 2024, lo que permitió que mi equipo avanzara sin retrasos, y reforzando mis capacidades de gestión de tiempo y proyectos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Cumplí con el objetivo dentro del plazo establecido, entregando los avances el 28 de agosto de 2024, lo que me permitió integrar estos aprendizajes y asegurar un trabajo colaborativo eficaz.\\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 27-08-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
He completado todas mis responsabilidades dentro del plazo establecido, asegurando que cada tarea se finalizara según lo previsto. La claridad en las fechas límite desde el inicio facilitó la organización efectiva de mi trabajo, permitiéndome cumplir con los objetivos a tiempo. Además, esto me permitió colaborar eficientemente con el equipo y contribuir al éxito del proyecto en el plazo acordado. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\bottomrule

\end{longtable}

\newpage

\begin{longtable}{|>{\centering\arraybackslash}m{4cm}|>{\centering\arraybackslash}m{3cm}|>{\centering\arraybackslash}m{5cm}|>{\centering\arraybackslash}m{3cm}|}
\hline
\multicolumn{4}{|c|}{\textbf{TB2}} \\
\hline
\textbf{\textit{SMART Goals}} & \textbf{Estudiante} & \textbf{Descripción del objetivo} & \textbf{Fechas de entrega} \\
\hline
\endfirsthead

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Específico:} \textit{¿Qué se va a lograr?} \\
El objetivo indica con especificidad, cuál es el proceso, servicio o producto en cuestión, para qué área es relevante, u otro detalle clave que brinde contexto. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es diseñar y desarrollar wireframes, mockups, prototipos y wireflows para la aplicación, con el fin de crear una interfaz de usuario intuitiva y coherente. Este proceso es relevante para el área de diseño de experiencia de usuario (UX) y diseño de interfaces (UI), asegurando que la aplicación sea visualmente atractiva y funcional, y cumpla con los requisitos del usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Mi objetivo en esta entrega es mejorar la arquitectura de la landing page, centrándome en la optimización del etiquetado SEO y la navegabilidad del sitio. Esto no solo es importante para el proyecto, sino que también me ayudará a adquirir habilidades necesarias para destacarme en el desarrollo web y optimización de motores de búsqueda (SEO), áreas en crecimiento profesional. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
En esta entrega, continuaré perfeccionando la documentación del proyecto y mejoré mis habilidades en configuración de software y diagramado arquitectónico. Estos conocimientos son esenciales para mi desarrollo en roles técnicos como ingeniero de software, permitiéndole tener una base sólida para la gestión de proyectos a gran escala. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es crear diagramas detallados de base de datos, clases y despliegue para la aplicación, con el fin de estructurar y organizar eficientemente los datos y el entorno de desarrollo. Este proceso es relevante para el área de arquitectura de software y diseño de sistemas, garantizando que la solución sea robusta, escalable y bien documentada, facilitando su implementación y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Medible:} \textit{¿Tiene KPI o métrica clara?} \\
El enunciado tiene una meta con indicador (KPI) o métrica clara, que determinará si el objetio se cumplió. Idealmente, describe el impacto (lo que vamos a lograr) más que el entregable (lo que vamos a hacer) \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la cantidad de iteraciones de wireframes, mockups y prototipos completados y aprobados por los usuarios y partes interesadas. La métrica clave será obtener al menos un 90\% de aprobación en pruebas de usabilidad realizadas con usuarios finales, lo que indicará que la interfaz es intuitiva y cumple con los requisitos de experiencia de usuario. Además, se evaluará la reducción en el número de revisiones y cambios requeridos después de las pruebas iniciales. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El éxito se medirá por la efectividad de los sistemas de etiquetado SEO y la navegación de la página, asegurando que el trabajo esté alineado con los estándares del proyecto y con las expectativas de usuarios y clientes, reforzando mis competencias en desarrollo web. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alehandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la calidad de los diagramas arquitectónicos y la correcta configuración del software, elementos clave que no solo cumplirán con los objetivos del proyecto, sino que contribuirán a mi crecimiento como profesional en desarrollo de software. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la integridad y precisión de los diagramas de base de datos, clases y despliegue en un 100% de conformidad con los requisitos del proyecto. Las métricas clave incluirán la validación de los diagramas por parte del equipo de desarrollo y la reducción de errores en la implementación del sistema en un 80%. También se evaluará el impacto en la eficiencia del desarrollo y la facilidad de mantenimiento del sistema, con un objetivo de reducir el tiempo de resolución de problemas en un 30% tras la implementación. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Ambicioso:} \textit{¿Es retador y va más allá de sus funciones?} \\
El objetivo inspira y reta a pensar acciones para dar el salto que se requiere para el logro, no se lograría sin una estrategia y un foco potentes. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es retador porque implica no solo diseñar wireframes, mockups y prototipos efectivos, sino también liderar la implementación de una metodología de diseño centrada en el usuario que podría ser adoptada como estándar para futuros proyectos. Esto requiere ir más allá de las funciones básicas, adoptando técnicas avanzadas de prototipado y herramientas innovadoras para asegurar una experiencia de usuario excepcional. La ambición está en transformar la visión del proyecto en una solución altamente interactiva y visualmente impactante, alineada con las mejores prácticas del mercado. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Este objetivo es ambicioso ya que me reta a mejorar mis conocimientos en SEO, una herramienta clave para la creación de productos digitales competitivos, lo cual es fundamental para mi desarrollo a largo plazo. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Este objetivo es retador, ya que me exige dominar nuevas herramientas de configuración y mejorar mi comprensión de la arquitectura de software, áreas cruciales para mi avance en roles técnicos de mayor responsabilidad en mi carrera.\\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es ambicioso ya que requiere desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, y además, establecer un proceso robusto para su integración y mantenimiento. Esto va más allá de la simple creación de diagramas; implica implementar un diseño que soporte escalabilidad, optimización del rendimiento y adaptabilidad a futuros cambios. El reto es establecer un estándar de arquitectura que no solo cumpla con los requisitos actuales, sino que también prepare al sistema para enfrentar desafíos futuros, mejorando significativamente la eficiencia y reduciendo el tiempo de desarrollo y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Relevante:} \textit{¿Está alineado a la estratégia?} \\
Existe una explicación clara respecto a cómo el objetivo impacta sobre los objetivos estratégicos de la institución o \textit{Laurate} Perú. Brinda una noción del alcance del objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia de la institución al mejorar la calidad y eficacia del desarrollo de software mediante el diseño centrado en el usuario. Al crear wireframes, mockups y prototipos efectivos, contribuimos a asegurar que la aplicación cumpla con los estándares de usabilidad y accesibilidad, lo cual impacta positivamente en la satisfacción del usuario final. Esta alineación con los principios de diseño de la institución refuerza nuestra capacidad para entregar productos de alta calidad que cumplen con las expectativas del mercado y los requisitos estratégicos de Laurate Perú. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Optimizar la arquitectura de la landing page y asegurar una navegación eficiente es vital no solo para este proyecto, sino para mi carrera, ya que estas son competencias esenciales en el ámbito del desarrollo web y diseño de productos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
La correcta implementación de diagramas de arquitectura y configuraciones de software es vital para mi crecimiento en la industria de la tecnología, preparándome para enfrentar retos más grandes en el futuro. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia institucional al garantizar una arquitectura de software sólida y bien documentada, que respalde la escalabilidad y el rendimiento del sistema. Al desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, contribuimos a la creación de soluciones de software robustas que cumplen con los estándares de calidad y eficiencia esperados por Laurate Perú. Esta alineación asegura que el sistema esté preparado para soportar futuros desarrollos y cambios, optimizando el proceso de desarrollo y mantenimiento en línea con los objetivos estratégicos de la institución. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Tiempo Límite:} \textit{¿Cuándo se cumplirá?} \\
En caso que la expectativa de fecha de cumplimiento sea previa al cierre de año, el enunciado contiene de forma explícita la fecha límite para alcanzar el objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 15 de septiembre del 2024. Para esta fecha, se espera haber completado el diseño de wireframes, mockups, prototipos y wireflows, y haber obtenido retroalimentación de los usuarios para garantizar que cumplan con los estándares de experiencia de usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El objetivo será cumplido para el 15 de septiembre de 2024, asegurando que la planificación del sprint backlog también esté lista para la próxima iteración del proyecto. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 15 de septiembre de 2024, asegurando que las contribuciones estén completas a tiempo para las próximas fases del proyecto, lo que refuerza mi habilidad para trabajar bajo plazos estrictos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 15 de septiembre del 2024. Para esta fecha, se espera haber desarrollado y documentado los diagramas de base de datos, clases y despliegue, y haber implementado las mejores prácticas en el entorno de desarrollo para asegurar una integración efectiva y eficiente. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 07-09-2024 \\
\textbf{Fecha de entrega:} 15-09-2024 \\
} \\
\bottomrule

\end{longtable}

\newpage

\begin{longtable}{|>{\centering\arraybackslash}m{4cm}|>{\centering\arraybackslash}m{3cm}|>{\centering\arraybackslash}m{5cm}|>{\centering\arraybackslash}m{3cm}|}
\hline
\multicolumn{4}{|c|}{\textbf{TP}} \\
\hline
\textbf{\textit{SMART Goals}} & \textbf{Estudiante} & \textbf{Descripción del objetivo} & \textbf{Fechas de entrega} \\
\hline
\endfirsthead

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Específico:} \textit{¿Qué se va a lograr?} \\
El objetivo indica con especificidad, cuál es el proceso, servicio o producto en cuestión, para qué área es relevante, u otro detalle clave que brinde contexto. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es diseñar y desarrollar wireframes, mockups, prototipos y wireflows para la aplicación, con el fin de crear una interfaz de usuario intuitiva y coherente. Este proceso es relevante para el área de diseño de experiencia de usuario (UX) y diseño de interfaces (UI), asegurando que la aplicación sea visualmente atractiva y funcional, y cumpla con los requisitos del usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Mi objetivo en esta entrega es mejorar la arquitectura de la landing page, centrándome en la optimización del etiquetado SEO y la navegabilidad del sitio. Esto no solo es importante para el proyecto, sino que también me ayudará a adquirir habilidades necesarias para destacarme en el desarrollo web y optimización de motores de búsqueda (SEO), áreas en crecimiento profesional. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
En esta entrega, continuaré perfeccionando la documentación del proyecto y mejoré mis habilidades en configuración de software y diagramado arquitectónico. Estos conocimientos son esenciales para mi desarrollo en roles técnicos como ingeniero de software, permitiéndole tener una base sólida para la gestión de proyectos a gran escala. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es crear diagramas detallados de base de datos, clases y despliegue para la aplicación, con el fin de estructurar y organizar eficientemente los datos y el entorno de desarrollo. Este proceso es relevante para el área de arquitectura de software y diseño de sistemas, garantizando que la solución sea robusta, escalable y bien documentada, facilitando su implementación y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Medible:} \textit{¿Tiene KPI o métrica clara?} \\
El enunciado tiene una meta con indicador (KPI) o métrica clara, que determinará si el objetio se cumplió. Idealmente, describe el impacto (lo que vamos a lograr) más que el entregable (lo que vamos a hacer) \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la cantidad de iteraciones de wireframes, mockups y prototipos completados y aprobados por los usuarios y partes interesadas. La métrica clave será obtener al menos un 90\% de aprobación en pruebas de usabilidad realizadas con usuarios finales, lo que indicará que la interfaz es intuitiva y cumple con los requisitos de experiencia de usuario. Además, se evaluará la reducción en el número de revisiones y cambios requeridos después de las pruebas iniciales. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El éxito se medirá por la efectividad de los sistemas de etiquetado SEO y la navegación de la página, asegurando que el trabajo esté alineado con los estándares del proyecto y con las expectativas de usuarios y clientes, reforzando mis competencias en desarrollo web. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alehandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la calidad de los diagramas arquitectónicos y la correcta configuración del software, elementos clave que no solo cumplirán con los objetivos del proyecto, sino que contribuirán a mi crecimiento como profesional en desarrollo de software. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la integridad y precisión de los diagramas de base de datos, clases y despliegue en un 100% de conformidad con los requisitos del proyecto. Las métricas clave incluirán la validación de los diagramas por parte del equipo de desarrollo y la reducción de errores en la implementación del sistema en un 80%. También se evaluará el impacto en la eficiencia del desarrollo y la facilidad de mantenimiento del sistema, con un objetivo de reducir el tiempo de resolución de problemas en un 30% tras la implementación. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Ambicioso:} \textit{¿Es retador y va más allá de sus funciones?} \\
El objetivo inspira y reta a pensar acciones para dar el salto que se requiere para el logro, no se lograría sin una estrategia y un foco potentes. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es retador porque implica no solo diseñar wireframes, mockups y prototipos efectivos, sino también liderar la implementación de una metodología de diseño centrada en el usuario que podría ser adoptada como estándar para futuros proyectos. Esto requiere ir más allá de las funciones básicas, adoptando técnicas avanzadas de prototipado y herramientas innovadoras para asegurar una experiencia de usuario excepcional. La ambición está en transformar la visión del proyecto en una solución altamente interactiva y visualmente impactante, alineada con las mejores prácticas del mercado. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Este objetivo es ambicioso ya que me reta a mejorar mis conocimientos en SEO, una herramienta clave para la creación de productos digitales competitivos, lo cual es fundamental para mi desarrollo a largo plazo. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Este objetivo es retador, ya que me exige dominar nuevas herramientas de configuración y mejorar mi comprensión de la arquitectura de software, áreas cruciales para mi avance en roles técnicos de mayor responsabilidad en mi carrera.\\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es ambicioso ya que requiere desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, y además, establecer un proceso robusto para su integración y mantenimiento. Esto va más allá de la simple creación de diagramas; implica implementar un diseño que soporte escalabilidad, optimización del rendimiento y adaptabilidad a futuros cambios. El reto es establecer un estándar de arquitectura que no solo cumpla con los requisitos actuales, sino que también prepare al sistema para enfrentar desafíos futuros, mejorando significativamente la eficiencia y reduciendo el tiempo de desarrollo y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Relevante:} \textit{¿Está alineado a la estratégia?} \\
Existe una explicación clara respecto a cómo el objetivo impacta sobre los objetivos estratégicos de la institución o \textit{Laurate} Perú. Brinda una noción del alcance del objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia de la institución al mejorar la calidad y eficacia del desarrollo de software mediante el diseño centrado en el usuario. Al crear wireframes, mockups y prototipos efectivos, contribuimos a asegurar que la aplicación cumpla con los estándares de usabilidad y accesibilidad, lo cual impacta positivamente en la satisfacción del usuario final. Esta alineación con los principios de diseño de la institución refuerza nuestra capacidad para entregar productos de alta calidad que cumplen con las expectativas del mercado y los requisitos estratégicos de Laurate Perú. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Optimizar la arquitectura de la landing page y asegurar una navegación eficiente es vital no solo para este proyecto, sino para mi carrera, ya que estas son competencias esenciales en el ámbito del desarrollo web y diseño de productos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
La correcta implementación de diagramas de arquitectura y configuraciones de software es vital para mi crecimiento en la industria de la tecnología, preparándome para enfrentar retos más grandes en el futuro. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia institucional al garantizar una arquitectura de software sólida y bien documentada, que respalde la escalabilidad y el rendimiento del sistema. Al desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, contribuimos a la creación de soluciones de software robustas que cumplen con los estándares de calidad y eficiencia esperados por Laurate Perú. Esta alineación asegura que el sistema esté preparado para soportar futuros desarrollos y cambios, optimizando el proceso de desarrollo y mantenimiento en línea con los objetivos estratégicos de la institución. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Tiempo Límite:} \textit{¿Cuándo se cumplirá?} \\
En caso que la expectativa de fecha de cumplimiento sea previa al cierre de año, el enunciado contiene de forma explícita la fecha límite para alcanzar el objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 27 de septiembre del 2024. Para esta fecha, se espera haber completado el diseño de wireframes, mockups, prototipos y wireflows, y haber obtenido retroalimentación de los usuarios para garantizar que cumplan con los estándares de experiencia de usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El objetivo será cumplido para el 27 de septiembre de 2024, asegurando que la planificación del sprint backlog también esté lista para la próxima iteración del proyecto. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 27 de septiembre de 2024, asegurando que las contribuciones estén completas a tiempo para las próximas fases del proyecto, lo que refuerza mi habilidad para trabajar bajo plazos estrictos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 27 de septiembre del 2024. Para esta fecha, se espera haber desarrollado y documentado los diagramas de base de datos, clases y despliegue, y haber implementado las mejores prácticas en el entorno de desarrollo para asegurar una integración efectiva y eficiente. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 20-09-2024 \\
\textbf{Fecha de entrega:} 28-09-2024 \\
} \\
\bottomrule

\end{longtable}

\newpage

\begin{longtable}{|>{\centering\arraybackslash}m{4cm}|>{\centering\arraybackslash}m{3cm}|>{\centering\arraybackslash}m{5cm}|>{\centering\arraybackslash}m{3cm}|}
\hline
\multicolumn{4}{|c|}{\textbf{TB3}} \\
\hline
\textbf{\textit{SMART Goals}} & \textbf{Estudiante} & \textbf{Descripción del objetivo} & \textbf{Fechas de entrega} \\
\hline
\endfirsthead

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Específico:} \textit{¿Qué se va a lograr?} \\
El objetivo indica con especificidad, cuál es el proceso, servicio o producto en cuestión, para qué área es relevante, u otro detalle clave que brinde contexto. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es diseñar y desarrollar wireframes, mockups, prototipos y wireflows para la aplicación, con el fin de crear una interfaz de usuario intuitiva y coherente. Este proceso es relevante para el área de diseño de experiencia de usuario (UX) y diseño de interfaces (UI), asegurando que la aplicación sea visualmente atractiva y funcional, y cumpla con los requisitos del usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Mi objetivo en esta entrega es mejorar la arquitectura de la landing page, centrándome en la optimización del etiquetado SEO y la navegabilidad del sitio. Esto no solo es importante para el proyecto, sino que también me ayudará a adquirir habilidades necesarias para destacarme en el desarrollo web y optimización de motores de búsqueda (SEO), áreas en crecimiento profesional. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
En esta entrega, continuaré perfeccionando la documentación del proyecto y mejoré mis habilidades en configuración de software y diagramado arquitectónico. Estos conocimientos son esenciales para mi desarrollo en roles técnicos como ingeniero de software, permitiéndole tener una base sólida para la gestión de proyectos a gran escala. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es crear diagramas detallados de base de datos, clases y despliegue para la aplicación, con el fin de estructurar y organizar eficientemente los datos y el entorno de desarrollo. Este proceso es relevante para el área de arquitectura de software y diseño de sistemas, garantizando que la solución sea robusta, escalable y bien documentada, facilitando su implementación y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Medible:} \textit{¿Tiene KPI o métrica clara?} \\
El enunciado tiene una meta con indicador (KPI) o métrica clara, que determinará si el objetio se cumplió. Idealmente, describe el impacto (lo que vamos a lograr) más que el entregable (lo que vamos a hacer) \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la cantidad de iteraciones de wireframes, mockups y prototipos completados y aprobados por los usuarios y partes interesadas. La métrica clave será obtener al menos un 90\% de aprobación en pruebas de usabilidad realizadas con usuarios finales, lo que indicará que la interfaz es intuitiva y cumple con los requisitos de experiencia de usuario. Además, se evaluará la reducción en el número de revisiones y cambios requeridos después de las pruebas iniciales. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El éxito se medirá por la efectividad de los sistemas de etiquetado SEO y la navegación de la página, asegurando que el trabajo esté alineado con los estándares del proyecto y con las expectativas de usuarios y clientes, reforzando mis competencias en desarrollo web. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alehandro Vilchez Rios \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la calidad de los diagramas arquitectónicos y la correcta configuración del software, elementos clave que no solo cumplirán con los objetivos del proyecto, sino que contribuirán a mi crecimiento como profesional en desarrollo de software. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El éxito se medirá por la integridad y precisión de los diagramas de base de datos, clases y despliegue en un 100% de conformidad con los requisitos del proyecto. Las métricas clave incluirán la validación de los diagramas por parte del equipo de desarrollo y la reducción de errores en la implementación del sistema en un 80%. También se evaluará el impacto en la eficiencia del desarrollo y la facilidad de mantenimiento del sistema, con un objetivo de reducir el tiempo de resolución de problemas en un 30% tras la implementación. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Ambicioso:} \textit{¿Es retador y va más allá de sus funciones?} \\
El objetivo inspira y reta a pensar acciones para dar el salto que se requiere para el logro, no se lograría sin una estrategia y un foco potentes. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo es retador porque implica no solo diseñar wireframes, mockups y prototipos efectivos, sino también liderar la implementación de una metodología de diseño centrada en el usuario que podría ser adoptada como estándar para futuros proyectos. Esto requiere ir más allá de las funciones básicas, adoptando técnicas avanzadas de prototipado y herramientas innovadoras para asegurar una experiencia de usuario excepcional. La ambición está en transformar la visión del proyecto en una solución altamente interactiva y visualmente impactante, alineada con las mejores prácticas del mercado. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Este objetivo es ambicioso ya que me reta a mejorar mis conocimientos en SEO, una herramienta clave para la creación de productos digitales competitivos, lo cual es fundamental para mi desarrollo a largo plazo. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
Este objetivo es retador, ya que me exige dominar nuevas herramientas de configuración y mejorar mi comprensión de la arquitectura de software, áreas cruciales para mi avance en roles técnicos de mayor responsabilidad en mi carrera.\\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo es ambicioso ya que requiere desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, y además, establecer un proceso robusto para su integración y mantenimiento. Esto va más allá de la simple creación de diagramas; implica implementar un diseño que soporte escalabilidad, optimización del rendimiento y adaptabilidad a futuros cambios. El reto es establecer un estándar de arquitectura que no solo cumpla con los requisitos actuales, sino que también prepare al sistema para enfrentar desafíos futuros, mejorando significativamente la eficiencia y reduciendo el tiempo de desarrollo y mantenimiento. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Relevante:} \textit{¿Está alineado a la estratégia?} \\
Existe una explicación clara respecto a cómo el objetivo impacta sobre los objetivos estratégicos de la institución o \textit{Laurate} Perú. Brinda una noción del alcance del objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia de la institución al mejorar la calidad y eficacia del desarrollo de software mediante el diseño centrado en el usuario. Al crear wireframes, mockups y prototipos efectivos, contribuimos a asegurar que la aplicación cumpla con los estándares de usabilidad y accesibilidad, lo cual impacta positivamente en la satisfacción del usuario final. Esta alineación con los principios de diseño de la institución refuerza nuestra capacidad para entregar productos de alta calidad que cumplen con las expectativas del mercado y los requisitos estratégicos de Laurate Perú. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
Optimizar la arquitectura de la landing page y asegurar una navegación eficiente es vital no solo para este proyecto, sino para mi carrera, ya que estas son competencias esenciales en el ámbito del desarrollo web y diseño de productos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
La correcta implementación de diagramas de arquitectura y configuraciones de software es vital para mi crecimiento en la industria de la tecnología, preparándome para enfrentar retos más grandes en el futuro. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
Este objetivo está alineado con la estrategia institucional al garantizar una arquitectura de software sólida y bien documentada, que respalde la escalabilidad y el rendimiento del sistema. Al desarrollar diagramas detallados y efectivos para la base de datos, clases y despliegue, contribuimos a la creación de soluciones de software robustas que cumplen con los estándares de calidad y eficiencia esperados por Laurate Perú. Esta alineación asegura que el sistema esté preparado para soportar futuros desarrollos y cambios, optimizando el proceso de desarrollo y mantenimiento en línea con los objetivos estratégicos de la institución. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\hline

\multirow{4}{*}{
\parbox[t]{4cm}{
\textbf{Tiempo Límite:} \textit{¿Cuándo se cumplirá?} \\
En caso que la expectativa de fecha de cumplimiento sea previa al cierre de año, el enunciado contiene de forma explícita la fecha límite para alcanzar el objetivo. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 25 de octubre del 2024. Para esta fecha, se espera haber completado el diseño de wireframes, mockups, prototipos y wireflows, y haber obtenido retroalimentación de los usuarios para garantizar que cumplan con los estándares de experiencia de usuario. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen del Rocio Ramos Rios
}
&
\parbox[t]{5cm}{
El objetivo será cumplido para el 25 de octubre de 2024, asegurando que la planificación del sprint backlog también esté lista para la próxima iteración del proyecto. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo Alejandro Vilchez Rios\\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 25 de octubre de 2024, asegurando que las contribuciones estén completas a tiempo para las próximas fases del proyecto, lo que refuerza mi habilidad para trabajar bajo plazos estrictos. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex Avila Asto \\
}
&
\parbox[t]{5cm}{
El objetivo se cumplirá para el 25 de octubre del 2024. Para esta fecha, se espera haber desarrollado y documentado los diagramas de base de datos, clases y despliegue, y haber implementado las mejores prácticas en el entorno de desarrollo para asegurar una integración efectiva y eficiente. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 18-10-2024 \\
\textbf{Fecha de entrega:} 26-10-2024 \\
} \\
\bottomrule

\end{longtable}

\newpage

***Project Report Collaboration Insights***

::: warn
Para mayor información, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Informe-del-Proyecto/pulse) 
:::

**TB1:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-2.png)

\newpage

**TB2:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-3.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-4.png)

\newpage

**TP:**

![Imagen extraída de Github - Codeminds](src/img/Cap5/insights.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-2.png)

\newpage

**TB3:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-tb3-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/team-colaboration-tb3-2.png)

\newpage

*Actividades Colaborativas* ***(Github Kanban)***

::: warn
Para mayor información, haga click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

**TB1:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-2.png)

\newpage

**TB2:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-3.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-4.png)

\newpage

**TP:**

![Imagen extraída de Github - Codeminds](src/img/Cap5/development-evidence.png)

![Imagen extraída de Github - Codeminds](src/img/Cap5/colaboration-insights-1.png)

\newpage

**TB3:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/colaboration-insights-tb3-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/colaboration-insights-tb3-2.png)

\newpage

# Capítulo I: Presentación 

## *Startup Profile*

### Descripción de la Startup

**CodeMinds: Innovando en Seguridad y Privacidad Digital**

CodeMinds es una startup dedicada a crear soluciones innovadoras que se ajustan a los estándares y necesidades del público general. Nos especializamos en el desarrollo de tecnologías que priorizan la seguridad y la privacidad de los datos de nuestros usuarios, conscientes de que en el mundo digital actual, proteger la información personal es fundamental. 
Nuestras plataformas están diseñadas para proporcionar herramientas seguras y accesibles, que permiten a los usuarios controlar y proteger sus datos de manera efectiva. En CodeMinds, estamos comprometidos con ofrecer soluciones que no solo satisfacen las expectativas de nuestros clientes, sino que también les brindan la tranquilidad de saber que su información está protegida.
Cada solución que desarrollamos está impulsada por nuestra firme creencia en la importancia de la privacidad y la seguridad digital. En CodeMinds, estamos redefiniendo la forma en que se abordan estos aspectos cruciales, colocando la protección de datos en el centro de nuestras innovaciones.

![CodeMinds logo](src/img/Logo/CodeMinds.png)

\newpage

::: box 
**Misión**

Nuestra misión en CodeMinds es desarrollar soluciones innovadoras que prioricen la seguridad y la privacidad de los datos del usuario. Nos enfocamos en crear herramientas accesibles y eficaces que permitan a nuestros clientes proteger su información personal en un entorno digital en constante evolución. Nos comprometemos a ofrecer tecnologías que se adapten a las necesidades del público general, asegurando que la protección de los datos sea sencilla, confiable y esté al alcance de todos.
:::

::: box
**Visión**

Nuestra visión en CodeMinds es ser líderes en el desarrollo de soluciones tecnológicas que redefinan la seguridad y la privacidad en la era digital. Aspiramos a ser reconocidos como una startup que empodera a los usuarios, brindándoles control total sobre sus datos a través de plataformas intuitivas y seguras. Buscamos transformar la manera en que las personas interactúan con la tecnología, asegurando que la protección de la información personal sea una prioridad en cada solución que ofrecemos.
:::

\newpage

### Perfiles de integrantes del equipo

Nuestro equipo está conformado por individuos apasionados y comprometidos, cada uno aportando
sus habilidades únicas para lograr nuestros objetivos de manera efectiva y colaborativa. Aquí semuestra
a nuestros miembros clave:

\definecolor{mybackground}{HTML}{eed6d1}

\begin{tcolorbox}[colframe=mybackground, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
\begin{minipage}[c]{0.3\textwidth}
\includegraphics[width=\linewidth]{src/img/Integrantes/abel.jpg}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Abel Angel Ortega Huaraca} \\
\textit{Ingeniero de Software} \\
Me considero una persona responsable y comprometida en las funciones que se me designe. Conforme a mis habilidades, puedo adaptarme rápidamente al equipo y al ritmo de trabajo. Asimismo, puedo contribuir con información y soluciones a través de una exhaustiva investigación para los problemas que el proyecto presente.
\end{minipage}
}
\end{tcolorbox}

\begin{tcolorbox}[colframe=mybackground, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
\begin{minipage}[c]{0.3\textwidth}
\includegraphics[width=\linewidth]{src/img/Integrantes/alex.jpg}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Alex Avila Asto} \\
\textit{Ingeniero de Software} \\
Soy una persona con buenas habilidades y adaptabilidad para todo lo relacionado a TI. Manejo un set robusto de tecnologías como C++, SQL, Java, Kotlin, etc. Por lo que puedo aportar al equipo con mis conocimientos técnicos y brindar soporte si lo amerita. 
\end{minipage}
}
\end{tcolorbox}

\begin{tcolorbox}[colframe=mybackground, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
\begin{minipage}[c]{0.3\textwidth}
\includegraphics[width=\linewidth]{src/img/Integrantes/belen.jpg}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Belen del Rocio Ramos Rios} \\
\textit{Ingeniera de Software} \\
Soy estudiante del sexto ciclo de la carrera de Ingeniería de Software. A lo largo de mi formación, he adquirido conocimientos en diversos lenguajes de programación, como Java, C++, y SQL. Además, manejo frameworks como Spring Boot para el desarrollo backend, y tanto Vue como Angular para el desarrollo frontend.
\end{minipage}
}
\end{tcolorbox}

\begin{tcolorbox}[colframe=mybackground, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
\begin{minipage}[c]{0.3\textwidth}
\includegraphics[width=\linewidth, height=\linewidth, keepaspectratio]{src/img/Integrantes/mateo.jpg}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Mateo Alejandro Vilchez Rios} \\
\textit{Ingeniero de Software} \\
Soy estudiante de la carrera de Ingeniería de Software cursando actualmente el 6to ciclo. Me considero una persona eficiente, disciplinada y responsable. Poseo conocimientos básicos en C++, Java y JavaScript. Manejo de Base de Datos relacionales. Conocimientos en Frameworks como Angular y Spring. Me comprometo a brindar todo el apoyo necesario para cumplir con todos los requerimientos.
\end{minipage}
}
\end{tcolorbox}

\newpage

## *Solution Profile* 

En la era digital actual, la protección de datos y la privacidad se han convertido en prioridades esenciales para usuarios y empresas por igual. A medida que la tecnología avanza, surgen nuevas amenazas y desafíos relacionados con la seguridad de la información, lo que hace que las soluciones tradicionales sean insuficientes para enfrentar las necesidades actuales.

CodeMinds aborda este desafío al ofrecer soluciones innovadoras diseñadas específicamente para garantizar la seguridad y privacidad de los datos del usuario. En lugar de conformarse con las prácticas estándar, nos enfocamos en desarrollar tecnologías avanzadas que faciliten la protección de la información en todos los niveles. Nuestra misión es simplificar la forma en que los usuarios gestionan y protegen sus datos, haciendo que la seguridad sea accesible y efectiva.

A través de nuestra plataforma, buscamos transformar la manera en que los individuos y las empresas interactúan con la tecnología, brindando herramientas que aseguren que sus datos estén siempre protegidos y bajo su control. En CodeMinds, la innovación se encuentra en el núcleo de nuestras soluciones, permitiendo a nuestros clientes enfrentar los desafíos de seguridad con confianza y tranquilidad.

![Recurso extraído de Canva](src/img/Cap1/solution.png)

\newpage

### Antecedentes y problemática

::: info
***What***

- El uso del internet es omnipresente, lo que expone a riesgos significativos de ciberseguridad.

- La mayoría de las soluciones actuales no están diseñadas con la protección adecuada, exponiéndose innecesariamente a riesgos.
:::

::: info
***Why***

- Los estudiantes, debido a su alta exposición digital y a menudo escasa conciencia sobre los riesgos en línea, son particularmente vulnerables a las amenazas cibernéticas. 
  
- *“CodeMinds"* tiene como objetivo garantizar que la interacción de los jóvenes con la tecnología sea segura, proporcionando una protección alineada con sus comportamientos y necesidades digitales.
:::

::: info
***Who***

- Jóvenes de secundaria, estudiantes de pregrado y postgrado, quienes son usuarios frecuentes de plataformas digitales, enfrentan elevados riesgos de ciberseguridad. 

- Además, los padres son actores clave, preocupados por la seguridad digital de sus hijos.
:::

::: info
***When***

- La necesidad de proteger los datos y la privacidad de los jóvenes es constante, especialmente cada vez que acceden a internet, utilizan aplicaciones móviles o interactúan en plataformas educativas y sociales.
:::

::: info
***Where***

- Esta problemática es particularmente prevalente en entornos educativos y sociales digitales, donde los jóvenes pasan la mayor parte de su tiempo interactuando con la tecnología y compartiendo información personal.
:::

::: attn
***How***

- En el contexto actual, muchos jóvenes pueden estar expuestos a amenazas en línea sin siquiera saberlo. *"CodeMinds"* ofrece una solución que se integra de manera sencilla en sus rutinas digitales, utilizando herramientas intuitivas para proteger sus datos personales y académicos en tiempo real. 
  
- El enfoque de *“CodeMinds”* se basa en la simplicidad y efectividad, permitiendo que los estudiantes se concentren en sus estudios y vida social sin preocuparse por la seguridad de su información.
:::

::: attn
***How Much***

- El costo de no proteger adecuadamente la información de los jóvenes puede ser significativo, tanto en términos de pérdida de datos como de exposición a ciberataques. *“CodeMinds”* ofrece una solución asequible y escalable que reduce estos riesgos considerablemente, asegurando la privacidad y seguridad de sus usuarios.
:::

### *Lean UX Process*

![Recurso extraído de Google](src/img/Cap1/LeanUXProcess.png)

#### *Lean UX Problem Statements*

::: note
***Problem Statement***

- Los estudiantes de secundaria, pregrado y postgrado enfrentan riesgos de privacidad y seguridad al utilizar su correo electrónico principal para registrarse en plataformas en línea, lo que también afecta su productividad debido a la saturación de correos irrelevantes.\newline

- Las soluciones existentes no ofrecen una protección integral que combine seguridad, privacidad, y una gestión eficiente de la bandeja de entrada.\newline

- ¿Cómo podemos mejorar la experiencia de los estudiantes en la gestión de su información personal que garanticen su privacidad y optimicen su productividad?
:::

#### *Lean UX Assumptions*

***Business Assumptions***

**1. El cliente necesita** proteger su información personal y privacidad al registrarse en diversas plataformas en línea.

**2. Las necesidades del cliente se resolverán mediante** el uso de un servicio de correos temporales que les permita registrarse en sitios web sin exponer su dirección de correo principal.

**3. Los clientes son (o serán)** estudiantes de secundaria, pregrado y postgrado que son activos en línea y están preocupados por su privacidad digital.

**4. El cliente quiere** seguridad y simplicidad **de nuestro servicio**, asegurando que sus datos permanezcan privados y que sea fácil de usar.

**5. El cliente también puede obtener** una experiencia de bandeja de entrada organizada y libre de spam e mails irrelevantes mediante el uso de correos temporales.

**6. Obtendré mi base de clientes mediante** la promoción del servicio a través de instituciones educativas, comunidades en línea y plataformas de redes sociales donde los estudiantes están activos.

**7. Ganaré dinero mediante** la oferta de planes de suscripción premium con características extendidas, como tiempos de expiración más largos para los correos electrónicos y opciones de seguridad mejoradas.

**8. Mi principal competencia son** otros servicios de correos temporales y proveedores de correo enfocados en la privacidad que ofrecen funcionalidades similares.

**9. Superaremos a la competencia mediante** la oferta de una aplicación móvil fácil de usar, específicamente diseñada para estudiantes, con integraciones que satisfacen sus necesidades educativas y de privacidad.

**10. Mi mayor riesgo es** la posibilidad de que los estudiantes no vean suficiente valor en el uso de correos temporales o consideren que las soluciones existentes son suficientes.

**11. Solucionaremos el riesgo mediante** la iteración continua de nuestro producto basada en la retroalimentación de los usuarios, asegurando que nuestro servicio esté optimizado para las necesidades específicas de nuestro público objetivo.

**12. ¿Cuáles son las suposiciones que, si se demuestran falsas, harán que el proyecto fracase?**

- Los estudiantes están lo suficientemente preocupados por su privacidad como para buscar y utilizar un servicio de correos temporales.

- La facilidad de uso y las características de seguridad serán suficientes para incentivar el uso continuo del servicio.\newline

***Business Outcomes***

- El 30% de los usuarios generan al menos un correo temporal cada semana.
 
- Un aumento del 20% en la retención de usuarios a los 3 meses.

- Un 15% de usuarios gratuitos se convierten a planes premium dentro de los primeros 2 meses.

- Un 15% de nuevos usuarios provienen de referencias de usuarios existentes.\newline

***User Assumptions***

**1. ¿Quién es el usuario?**
   
- Estudiantes de secundaria, pregrado y postgrado que son activos en línea y están preocupados por su privacidad digital.\newline

**2. ¿Dónde encajaría nuestro producto en la vida (o trabajo, según el contexto del producto) del usuario?**
   
- Durante el registro en plataformas en línea, foros, o sitios de recursos académicos.

- Al acceder a recursos educativos o inscribirse en plataformas de aprendizaje.
  
- Cuando necesitan proteger su información personal en contextos donde no confían completamente en la seguridad del sitio web.\newline

**3. ¿Qué problemas resuelve el producto para el usuario?**
   
- Protección de la información personal durante registros en línea.
  
- Prevención de la saturación de la bandeja de entrada con correos no deseados.
  
- Provisión de una solución segura y temporal para registros en múltiples plataformas.\newline

**4. ¿En qué contexto utiliza el usuario el producto?**
   
- Contextos académicos, como inscripciones en plataformas educativas o acceso a recursos online.
  
- Participación en comunidades y foros en línea.
  
- Registros en sitios de entretenimiento o servicios en línea donde se requiere un correo electrónico.\newline

**5. ¿Qué características son esenciales para el usuario? ¿Y por qué?**

- Generación rápida de correos temporales: Para una experiencia ágil y sin complicaciones.
  
- Facilidad de uso: Para que cualquier estudiante, independientemente de su nivel de habilidades tecnológicas, pueda utilizar el servicio.
  
- Personalización de la duración de los correos: Para adaptarse a las necesidades específicas de cada registro o situación.
  
- Integración con plataformas educativas: Para facilitar el acceso a recursos académicos con mayor seguridad.\newline

**6. ¿Cómo debería verse y comportarse el producto?**
   
- Interfaz simple, intuitiva y minimalista.

- Diseño moderno y atractivo que apele a los estudiantes.

- Comportamiento rápido y confiable, con procesos fáciles de entender y ejecutar.

- Generación y gestión de correos temporales en pocos clics, con navegación fluida.\newline

***User Outcomes***

- Los estudiantes quieren proteger su privacidad sin complicaciones al registrarse en sitios web.
  
- Los estudiantes quieren sentirse seguros y tranquilos sabiendo que su información personal no será comprometida.
  
- Utilizar una herramienta que garantice la protección de la información personal en cada uso.\newline

***Features Assumptions***

**1. Seguridad de la Información:**

- **Suposición:** La implementación de cifrado de extremo a extremo para los correos temporales asegurará que los usuarios confíen en la seguridad de la aplicación.
  
- **Riesgo:** Si el cifrado no es lo suficientemente robusto o si los usuarios no perciben el valor de esta medida, la confianza en la seguridad podría no mejorar.\newline

**2. Facilidad de Uso:**
   
- **Suposición:** Un proceso de generación de correos temporales con un solo clic hará que la aplicación sea fácil de usar y aumentará la adopción entre los usuarios.
  
- **Riesgo:** Si el proceso no es tan intuitivo como se espera, los usuarios podrían encontrar la aplicación difícil de usar y abandonar su uso.\newline

**3. Protección de Privacidad:**

- **Suposición:** La implementación de una función que automáticamente borre los correos temporales después de un período predeterminado mejorará la percepción de privacidad entre los usuarios.

- **Riesgo:** Si los usuarios desean más control sobre cuándo se eliminan sus correos, esta función podría generar frustración en lugar de confianza.\newline

**4. Notificaciones y Recordatorios:**
  
- **Suposición:** Proveer notificaciones y recordatorios cuando un correo temporal esté a punto de expirar ayudará a los usuarios a gestionar mejor sus registros y evitar perder información importante.

- **Riesgo:** Si las notificaciones son percibidas como intrusivas o innecesarias, podrían causar descontento y disminuir la satisfacción del usuario.\newline

**5. Proceso de Registro Simplificado:**

- **Suposición:** Ofrecer un registro simplificado que no requiera información personal adicional aumentará la tasa de adopción de la aplicación, ya que los usuarios valorarán la simplicidad y la privacidad desde el primer contacto.
  
- **Riesgo:** Si el proceso de registro es demasiado simple, los usuarios podrían dudar de la legitimidad o seguridad de la aplicación, lo que podría afectar negativamente su confianza en el producto.\newline


#### *Lean UX Hypothesis Statements*

::: tip

**1. Creemos que lograremos** aumentar la retención de usuarios en un 20%. **Si** estudiantes preocupados por su privacidad digital **obtienen** una experiencia de registro en línea más segura y sin spam **con** la implementación de correos temporales rápidos y fáciles de generar.\newline

**2. Creemos que lograremos** incrementar la tasa de conversión a suscripciones premium en un 15%. **Si** los estudiantes que utilizan correos temporales regularmente **obtienen** acceso a características avanzadas como mayor tiempo de expiración para sus correos **con** la oferta de un plan premium accesible y fácil de entender.\newline

**3. Creemos que lograremos** aumentar la cantidad de referencias a la aplicación en un 10%. **Si** los usuarios satisfechos con la seguridad y privacidad de la aplicación **obtienen** incentivos para compartir la aplicación **con** sus amigos y compañeros con un programa de referidos que ofrezca beneficios exclusivos.\newline

**4. Creemos que lograremos** mejorar la percepción de seguridad entre los usuarios en un 25%. **Si** los estudiantes que se preocupan por la privacidad **obtienen** tranquilidad sobre la protección de sus datos personales **con** la implementación de notificaciones que confirmen la eliminación segura de sus correos temporales.\newline

**5. Creemos que lograremos** incrementar la adopción de la aplicación en un 30%. **Si** los estudiantes que buscan proteger su privacidad en línea **obtienen** una manera rápida y eficiente de generar correos temporales **con** una función de generación con un solo clic.
:::

#### *Lean UX Canvas*

![Artefacto creado en Figma [URL](https://www.figma.com/design/K3gw63Gdzr8KOgE32BgreJ/Lean-UX-Canvas-Template-by-Jeff-Gothelf-(Community)?node-id=0-1&t=q5cZNvpSyA30WQQd-1)](src/img/Cap1/LeanUXCanvas.png) 

\newpage

## Segmentos Objetivo

En CodeMinds, nuestro enfoque está en atender a un público clave: estudiantes de todos los niveles educativos. Desde estudiantes escolares que están dando sus primeros pasos en el mundo digital, hasta aquellos en niveles superiores como pregrado y postgrado que buscan herramientas avanzadas para proteger su información. Nuestro objetivo es ofrecer soluciones de seguridad que se adapten a las necesidades específicas de cada grupo, garantizando que todos puedan proteger sus datos con confianza y facilidad.

![Tabla del segmento objetivo 1 - Elaboración propia](src/img/Cap1/segmento-objetivo-1.png)

![Tabla del segmento objetivo 2 - Elaboración propia](src/img/Cap1/segmento-objetivo-2.png)

\newpage

# Capítulo II: *Needfinding*

## Competidores

![Recurso extraído de Canva](src/img/cap2/competidores-introduccion.png)

En un mercado donde la privacidad y la seguridad de los datos personales se han convertido en pilares fundamentales. Un análisis detallado de las soluciones existentes es esencial para identificar oportunidades de diferenciación e innovación, garantizando así que la propuesta de CodeMinds no solo cumpla con las expectativas de los usuarios, sino que también sobresalga en un entorno competitivo y exigente.

\newpage

**Competidores:**

- ***Abine Blur:*** Es una herramienta eficaz para generar correos electrónicos temporales de forma gratuita. Su enfoque en la simplicidad y el anonimato facilita a los usuarios la creación de direcciones temporales sin necesidad de registro, convirtiéndolo en una opción popular para quienes desean evitar el spam en su correo principal. Es ideal para usuarios que buscan una solución rápida, accesible y segura en sus dispositivos móviles.

![Imagen extraída de Abine [(URL)](https://abine.com/)](src/img/cap2/abine-landing.png)

- ***AnonAddy:*** Este servicio ofrece la creación de alias de correo electrónico que redirigen los correos recibidos al correo personal del usuario, permitiendo la privacidad y protección contra el spam. La aplicación móvil permite gestionar fácilmente estos alias y ofrece opciones avanzadas para usuarios más técnicos, bajo un modelo freemium.

![Imagen extraída de Addy [(URL)](https://addy.io/)](src/img/cap2/anonAddy-landing.png)

- ***TempMail:*** Es una herramienta eficaz para generar correos electrónicos temporales de forma gratuita. Su enfoque en la simplicidad y el anonimato facilita a los usuarios la creación de direcciones temporales sin necesidad de registro, convirtiéndolo en una opción popular para quienes desean evitar el spam en su correo principal. Es ideal para usuarios que buscan una solución rápida, accesible y segura en sus dispositivos móviles.

![Imagen extraída de TempMail [(URL)](https://tempmail.email/)](src/img/cap2/tempMail-landing.png)

- ***Burner Mail:*** Es un servicio especializado en la generación de direcciones de correo electrónico desechables, diseñadas para proteger la privacidad del usuario al interactuar con servicios en línea. Estas direcciones permiten registrarse en diversas plataformas sin necesidad de revelar la dirección de correo principal del usuario, lo que minimiza el riesgo de exposición a correos no deseados y posibles violaciones de seguridad.

![Imagen extraída de Burner Mail [(URL)](https://burnermail.io/)](src/img/cap2/burnerMail-landing.png)

### Análisis competitivo

![](src/img/cap2/analisisCompetitivo_1.png)

![](src/img/cap2/analisisCompetitivo_2.png)

![](src/img/cap2/analisisCompetitivo_3.png)

\newpage

### Estrategias y tácticas frente a Competidores

\vspace{1em}

\begin{quote}
Según Kašparová (2022), en el contexto de la gestión estratégica moderna, la inteligencia empresarial se ha convertido en un componente clave para desarrollar y mantener una ventaja competitiva sostenible.
\end{quote}

\vspace{1em}

La autora argumenta que la capacidad de una empresa para analizar grandes volúmenes de datos y convertirlos en información accionable es crucial para tomar decisiones estratégicas efectivas. Este enfoque permite a las empresas anticipar movimientos de la competencia, adaptar sus estrategias en tiempo real y responder de manera proactiva a las oportunidades y amenazas del mercado, lo que es esencial para asegurar el éxito a largo plazo en un entorno empresarial altamente dinámico.

Teniendo en cuenta el análisis *SWOT* previamente presentado para *CodeMinds*, proponemos las siguientes estrategias competitivas:

**Estrategias competitivas para** ***CodeMinds***

::: box
**Diferenciación a través de la Innovación:**
:::

**Estrategia:** *CodeMinds* debe destacarse en el mercado por ofrecer soluciones de privacidad y seguridad digital que no solo cumplan con las expectativas actuales, sino que también anticipen las necesidades futuras. La innovación continua en la protección de datos es crucial para mantener una ventaja competitiva. 

**Tácticas:**

   - Identificar tendencias emergentes y nuevas amenazas en el ámbito de la seguridad digital, asegurando que CodeMinds siempre esté un paso adelante.
  
   - Invertir en I+D para crear herramientas de protección de datos y correos temporales que ofrezcan funcionalidades únicas y altamente efectivas.

   - Implementar un ciclo regular de lanzamientos de nuevas funcionalidades, promoviendo activamente estas innovaciones a través de campañas de marketing dirigidas.

::: box
**Enfoque en Segmentos Específicos del Mercado:**
:::
   
**Estrategia:** *CodeMinds* debe personalizar sus soluciones para segmentos específicos, como estudiantes de todos los niveles educativos que requieren herramientas confiables y fáciles de usar para proteger su información. 

\newpage

**Tácticas:**

   - Desarrollar características específicas para estudiantes y académicos, como bandejas de entrada seguras y correos temporales con mayor control.
  
   - Establecer asociaciones con instituciones educativas para integrar CodeMinds en sus plataformas tecnológicas y ofrecer servicios exclusivos.
  
   - Dirigir campañas publicitarias específicamente a estudiantes, resaltando la relevancia y el valor de CodeMinds en sus actividades académicas diarias.

::: box
**Alianzas Estratégicas:**
:::
   
**Estrategia:** Formar alianzas con empresas y organizaciones clave en el sector de la tecnología y la ciberseguridad para mejorar la oferta de CodeMinds y expandir su presencia en el mercado.  

**Tácticas:**

   - Integrar soluciones de seguridad avanzadas de socios estratégicos, fortaleciendo así la propuesta de valor de CodeMinds.
  
   - Trabajar con plataformas de e-learning y universidades para ofrecer paquetes combinados de servicios educativos y protección de datos.

::: box
**Expansión Internacional:**
:::
   
**Estrategia:** *CodeMinds* debe considerar la expansión hacia mercados internacionales, adaptando sus productos y servicios a las necesidades de usuarios en diferentes regiones y culturas. 

**Tácticas:**

   - Adaptar la interfaz, el contenido y las funcionalidades de CodeMinds a diferentes idiomas y normas culturales para facilitar su adopción en mercados extranjeros.
  
   - Identificar y evaluar oportunidades en mercados emergentes donde la demanda de soluciones de privacidad digital está en crecimiento, y adaptar la estrategia de entrada según las condiciones locales.
  
   - Establecer alianzas con empresas locales en mercados objetivo para facilitar la entrada y acelerar la adopción de CodeMinds.

\newpage

**Tácticas Específicas para CodeMinds**

::: box
**Inversión en Marketing Diferenciado:**
:::

**Táctica:** Desarrollar una identidad de marca que subraye la superioridad técnica y la confiabilidad de CodeMinds en el ámbito de la privacidad y la seguridad digital. 

**Acciones:**

   - Crear y distribuir contenido que no solo promueva CodeMinds, sino que también eduque a los usuarios sobre la importancia de la seguridad digital.
  
   - Aprovechar testimonios de usuarios clave y casos de éxito para generar confianza y credibilidad en la marca.

::: box
**Monitoreo Competitivo Continuo:**
:::

**Táctica:** Mantener un análisis constante de las acciones de los competidores para anticipar movimientos en el mercado y ajustar las estrategias de CodeMinds en consecuencia.  

**Acciones:**

   - Monitorizar continuamente los nuevos productos, precios y promociones de los competidores para ajustar las ofertas de CodeMinds en tiempo real.

   - Utilizar herramientas avanzadas de inteligencia de mercado para identificar oportunidades y amenazas emergentes.

::: box
**Optimización de la Experiencia del Usuario (UX):**
:::

**Táctica:** Mejorar continuamente la experiencia del usuario en la aplicación de CodeMinds para aumentar la retención y satisfacción de los clientes.  

**Acciones:**

   - Implementar sistemas para recopilar y analizar feedback de los usuarios, utilizando esta información para realizar mejoras iterativas en la interfaz y funcionalidades.

   - Realizar pruebas A/B para experimentar con diferentes diseños y flujos de usuario, identificando las configuraciones que maximicen la satisfacción y el uso efectivo de la aplicación.

\newpage

::: box
**Fomento de la Fidelización del Cliente:**
:::

**Táctica:** Implementar programas y estrategias para aumentar la fidelidad del cliente y promover la retención a largo plazo.  

**Acciones:**

   - Desarrollar programas de fidelización que ofrezcan recompensas a los usuarios por su lealtad, como descuentos, acceso a funciones premium o beneficios exclusivos.

   - Enviar comunicaciones personalizadas a los clientes basadas en su comportamiento y uso de la aplicación, ofreciendo sugerencias de uso, actualizaciones de productos y promociones adaptadas a sus necesidades.

::: box
**Estrategias de Precios y Paquetes Competitivos:**
:::

**Táctica:** Ajustar estratégicamente los precios y paquetes de servicios para competir de manera efectiva en el mercado.  

**Acciones:**

   - Realizar análisis de precios comparativos y ajustar los precios de acuerdo con el valor percibido por los clientes.

   - Ofrecer paquetes personalizados que se ajusten a las necesidades específicas de diferentes tipos de clientes, como estudiantes y profesionales.

\newpage

## Entrevistas

![Recurso extraído de Canva](src/img/Cap2/entrevistas-introduccion.png)

::: note
Para acceder al video de las entrevistas, haga click en la [URL](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221a322_upc_edu_pe/ETJe4kTakANPuvEWBeV6fsoBgYJa7YDI8yt0Mp90Wf_fNg?e=rEvT4q&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
:::

\newpage

### Diseño de entrevistas

Entrevista a personas referentes a nuestro segmentos objetivo, las preguntas varían dependiendo del segmento debido a las diferentes situaciones:

::: box
**Segmento Objetivo 1:** Estudiantes de nivel escolar
:::

**Preguntas sobre Dispositivos**

1) ¿Qué dispositivos usas con más frecuencia para acceder a Internet?

2) ¿Qué marca y modelo es tu dispositivo principal?

3) ¿Tu dispositivo tiene alguna medida de seguridad activada?

4) ¿Con qué frecuencia actualizas el sistema operativo de tus dispositivos?

5) ¿Cuántas aplicaciones tienes instaladas en tu dispositivo principal? (¿Cuántas de ellas usas regularmente?)

6) ¿Alguna vez has perdido tu dispositivo? ¿Qué hiciste para proteger tu información?

7) ¿Compartes tus dispositivos con otras personas? Si es así, ¿cómo te aseguras de que tu información esté protegida?

**Preguntas sobre Navegación en Internet**

1) ¿Qué navegador utilizas más a menudo cuando navegas por Internet?

2) ¿Sabes si tu navegador tiene algún tipo de protección o bloqueo para sitios web peligrosos?

3) ¿Alguna vez has sentido que tu información personal estaba en riesgo al navegar en algún sitio web?

4) ¿Sueles aceptar las cookies cuando un sitio web te lo pide? ¿Por qué?

5) ¿Tienes algún sitio web favorito o que visites frecuentemente? ¿Por qué?

6) ¿Alguna vez has usado el modo de navegación privada o incógnito? ¿En qué situaciones?

7) ¿Has experimentado alguna vez con bloqueadores de anuncios o extensiones para mejorar tu privacidad en línea?

8) ¿Qué haces cuando encuentras un sitio web que no parece seguro?

**Preguntas sobre Seguridad y Privacidad**

1) ¿Cómo te aseguras de que un sitio web es seguro antes de ingresar tus datos personales?

2) ¿Has recibido alguna educación o formación sobre cómo proteger tu privacidad en Internet?

3) ¿Alguna vez te has encontrado con un sitio web que te pide mucha información personal? ¿Qué haces en esos casos?

4) ¿Confías en las aplicaciones que descargas para mantener tu información segura? ¿Por qué?

5) ¿Qué harías si descubrieras que tu información personal fue robada o usada sin tu permiso?

6) ¿Alguna vez has usado una VPN (Red Privada Virtual)? ¿Por qué o por qué no?

7) ¿Tienes alguna preocupación particular sobre tu seguridad o privacidad en línea?

8) ¿Sabes qué hacer si alguien intenta acceder a tus cuentas o información personal sin tu permiso?

**Preguntas sobre Preferencias de Uso**

1) ¿Qué sistema operativo prefieres en tus dispositivos móviles?

2) ¿Qué te hace sentir más seguro al usar un dispositivo móvil o una computadora?

3) ¿Prefieres usar aplicaciones o sitios web para hacer tus tareas escolares? ¿Por qué?

4) ¿Conoces o usas aplicaciones específicas para proteger tu privacidad en línea?

5) ¿Cómo te enteras de nuevas aplicaciones o sitios web que pueden ser útiles para ti?

6) ¿Qué funciones o características buscas en una aplicación antes de instalarla?

7) ¿Alguna vez has dejado de usar una aplicación porque no te sentías seguro al usarla? ¿Cuál fue la razón principal?

\newpage

::: box
**Segmento Objetivo 2:** Estudiantes de nivel universitario y superior (pregrado - postgrado)
:::

**Preguntas sobre Dispositivos**

1) ¿Qué dispositivos utilizas con mayor frecuencia para tus estudios y actividades en línea?

2) ¿Cuál es la marca y modelo de tu dispositivo principal?

3) ¿Qué sistema operativo prefieres usar en tus dispositivos principales?

4) ¿Con qué frecuencia actualizas el sistema operativo y las aplicaciones en tus dispositivos?

5) ¿Utilizas algún software de seguridad, como antivirus o firewall, en tus dispositivos?

6) ¿Qué tan cómodo te sientes manejando configuraciones de seguridad en tus dispositivos?

7) ¿Has sufrido alguna vez la pérdida o robo de un dispositivo? ¿Cómo gestionaste la seguridad de tus datos?

8) ¿Compartes tus dispositivos con otras personas? Si es así, ¿qué medidas tomas para proteger tu información personal?

**Preguntas sobre Navegación en Internet**

1) ¿Qué navegadores usas más frecuentemente para tus actividades en línea?

2) ¿Qué tan consciente eres de las medidas de seguridad integradas en los navegadores que utilizas?

3) ¿Has experimentado alguna vez problemas de seguridad mientras navegabas por Internet, como alertas de sitios inseguros?

4) ¿Usas el modo de navegación privada o incógnito? ¿Con qué frecuencia y en qué situaciones?

5) ¿Has experimentado con el uso de bloqueadores de anuncios, extensiones de seguridad, o configuraciones de privacidad en tu navegador?

6) ¿Qué medidas tomas para asegurarte de que un sitio web es seguro antes de ingresar información personal o realizar transacciones?

7) ¿Tienes configuraciones específicas en tu navegador para mejorar tu privacidad en línea?

8) ¿Qué haces si te encuentras con un sitio web que parece no ser seguro o que pide demasiada información personal?

**Preguntas sobre Seguridad y Privacidad**

1) ¿Cuánto te preocupa la seguridad y privacidad de tus datos al utilizar aplicaciones y servicios en línea?

2) ¿Qué estrategias utilizas para proteger tu información personal en línea, como contraseñas, datos bancarios o información académica?

3) ¿Has recibido alguna formación específica sobre ciberseguridad o privacidad de datos en tus estudios?

4) ¿Qué tan importante es para ti que las aplicaciones que usas tengan políticas claras de privacidad y protección de datos?

5) ¿Alguna vez has revisado las políticas de privacidad o términos de uso de las aplicaciones o servicios que utilizas?

6) ¿Has utilizado herramientas como gestores de contraseñas o autenticación de dos factores para proteger tus cuentas?

7) ¿Qué tan seguro te sientes usando servicios en la nube para almacenar o compartir archivos?

8) ¿Alguna vez has considerado usar una VPN (Red Privada Virtual) para proteger tu conexión a Internet? Si es así, ¿por qué?

9) ¿Te preocupa el seguimiento en línea o la recopilación de datos por parte de aplicaciones y sitios web? ¿Qué medidas tomas al respecto?

10) ¿Qué harías si descubrieras que tu información personal ha sido comprometida en un ciberataque?

11) ¿Alguna vez has dejado de usar un servicio o aplicación porque te preocupaba la seguridad de tus datos? ¿Cuál fue la razón?

**Preguntas sobre Preferencias de Uso**

1) ¿Qué dispositivos y sistemas operativos prefieres usar para tus estudios y trabajo?

2) ¿Qué aplicaciones consideras esenciales para tus estudios y por qué?

3) ¿Prefieres utilizar aplicaciones o sitios web específicos para realizar tus tareas académicas?

4) ¿Qué características buscas en una aplicación antes de decidir instalarla y usarla regularmente?

5) ¿Cómo descubres nuevas aplicaciones o servicios que pueden ayudarte en tus estudios?

6) ¿Qué tan importante es para ti que las aplicaciones o servicios que usas sean seguros y respeten tu privacidad?

7) ¿Has dejado de utilizar alguna aplicación porque no cumplía con tus expectativas de seguridad o privacidad?

8) ¿Qué expectativas tienes sobre la protección de tus datos personales al usar aplicaciones educativas?

\newpage

**Preguntas sobre Conductas en Línea**

1) ¿Con qué frecuencia revisas y ajustas las configuraciones de privacidad en tus cuentas en línea?

2) ¿Qué tan consciente eres de las amenazas cibernéticas como phishing, malware, o robo de identidad?

3) ¿Cómo gestionas la información que compartes en redes sociales y plataformas públicas?

4) ¿Qué tan cómodo te sientes utilizando autenticación de dos factores (2FA) para proteger tus cuentas?

5) ¿Alguna vez has experimentado un intento de phishing o estafa en línea? ¿Cómo reaccionaste?

6) ¿Qué tan probable es que uses herramientas o aplicaciones diseñadas específicamente para mejorar tu seguridad en línea?

7) ¿Qué tan dispuesto estás a pagar por aplicaciones o servicios que garanticen una mayor seguridad y privacidad?

\newpage

### Registro de entrevistas

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
\textbf{Tiempo de entrevista} & 00:00 - 09:34           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**
Pol Adriano Ramos Ríos, un joven de 14 años, utiliza principalmente su laptop HP para realizar tareas escolares y, ocasionalmente, su celular. Aunque no ha activado medidas de seguridad adicionales en su dispositivo, confía en las configuraciones predeterminadas de Windows y actualiza su sistema operativo con poca frecuencia. Pol tiene entre 12 y 15 aplicaciones instaladas en su dispositivo y guarda su información en la nube, específicamente en OneDrive, como medida de respaldo.
En cuanto a la navegación por internet, Pol utiliza el navegador Brave, que prefiere por su VPN integrada y su capacidad para bloquear anuncios y cookies, lo que le brinda una sensación de mayor seguridad. No ha sentido que su información personal esté en riesgo, excepto en ocasiones al utilizar Chrome u Opera, y evita aceptar cookies por preocupaciones de rastreo. Sus sitios web favoritos son Twitch y YouTube, donde sigue transmisiones de videojuegos y busca contenido educativo. Pol ha utilizado el modo incógnito para explorar herramientas como Tor y valora las extensiones de privacidad que le ofrece Brave.
Pol se asegura de que un sitio web sea seguro antes de ingresar información personal utilizando un correo secundario o falso. No ha recibido formación específica sobre privacidad en internet, pero es cauteloso al interactuar con sitios que solicitan demasiada información personal. En cuanto a las aplicaciones, Pol prefiere no descargar muchas, pero cuando lo hace, las prueba exhaustivamente antes de confiar en ellas, llegando incluso a resetear su computadora como medida de precaución.
Pol considera que iOS es más seguro que Android, pero cuando se trata de usar dispositivos, prefiere su computadora porque siente que le ofrece un mayor control sobre sus actividades y datos. Para sus tareas escolares, prefiere utilizar sitios web como YouTube y ChatGPT, que le brindan explicaciones directas y fáciles de entender.
Finalmente, Pol confía en su capacidad para evaluar nuevas aplicaciones y sitios web a través de reseñas y calificaciones antes de instalarlas. Aunque no ha dejado de usar ninguna aplicación por motivos de seguridad, siempre verifica su confiabilidad antes de continuar usándolas.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_AdrianoRamos.png)

\newpage

**Entrevista #2**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Grecia Jazmín Capristán Yepes \\ \hline
\textbf{Edad}                 & 14 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & 09:35 - 19:02           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**
Grecia Jazmín Capristán Yepes, una joven de 14 años, utiliza principalmente su iPhone para acceder a internet. Aunque su dispositivo cuenta con medidas de seguridad activadas, Grecia no está completamente segura de cuáles son. Sin embargo, se asegura de mantener su sistema operativo actualizado, siguiendo las indicaciones de su teléfono cada vez que se le solicita. En su dispositivo, solo tiene instaladas cinco aplicaciones, entre las cuales usa regularmente TikTok, Instagram y WhatsApp. Para navegar por internet, prefiere utilizar Google Chrome, confiando en las herramientas de seguridad del navegador para bloquear sitios peligrosos, lo que le proporciona una sensación de tranquilidad al sentir que su información no está en riesgo.
Grecia es selectiva al aceptar cookies: solo las permite en sitios web en los que confía y las rechaza en aquellos que le generan desconfianza. Aunque no suele usar el modo de navegación incógnito, ha experimentado con bloqueadores de anuncios. A pesar de no haber recibido formación específica sobre protección de la privacidad en internet, Grecia evita proporcionar información personal en sitios que le generan sospechas. En cuanto a las aplicaciones, confía únicamente en algunas para mantener su información segura, y prefiere utilizar un correo electrónico secundario al registrarse en aquellas que no le inspiran total confianza.
Grecia reconoce que, si su información personal llegara a ser comprometida, no estaría segura de cómo manejar la situación, ya que nunca ha enfrentado un problema de este tipo. No ha utilizado VPNs y, por el momento, no tiene preocupaciones particulares sobre su seguridad en línea. Tampoco sabría qué hacer si alguien intentara acceder a su información sin su permiso.
Grecia prefiere iOS como sistema operativo y considera que su dispositivo móvil es más seguro que una computadora. Para sus tareas escolares, opta por utilizar sitios web en lugar de aplicaciones, ya que considera que estos le ofrecen mayor información. Aunque no utiliza aplicaciones específicas para proteger su privacidad, se mantiene informada sobre nuevas herramientas a través de recomendaciones de sus compañeros o anuncios. Antes de instalar una nueva aplicación, Grecia se asegura de que esta solicite únicamente los permisos adecuados. En el pasado, ha dejado de usar aplicaciones cuando no se sentía segura, como en una ocasión en la que se filtraron sus contactos, lo que la llevó a cambiar su número de teléfono.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_GreciaCapristan.png)

\newpage

**Entrevista #3**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Carlet Gil Olivera \\ \hline
\textbf{Edad}                 & 17 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & 19:03 - 27:32           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**
Carlet, de 17 años, utiliza su celular para acceder a internet y confía en las medidas de seguridad que vienen preinstaladas en su dispositivo Apple. Debido a que no comparte su celular con otras personas, siente que su información personal está más protegida. Para navegar por internet, utiliza el navegador Safari, aunque no está muy informada sobre sus características de seguridad. En ocasiones, ha sentido que su información podría estar en riesgo al visitar sitios con numerosos anuncios emergentes, y admite que suele aceptar cookies sin leer los términos y condiciones.
Carlet utiliza el modo de navegación privada de manera ocasional, sobre todo cuando accede a páginas que podrían contener virus o para ver películas. Sin embargo, nunca ha utilizado bloqueadores de anuncios ni extensiones de privacidad, optando en su lugar por salir de los sitios que considera inseguros. Aunque reconoce el ícono del candado en la barra de direcciones como un indicador de seguridad en sitios web, no ha recibido ninguna educación formal sobre cómo proteger su privacidad en línea.
Tiende a desconfiar de los sitios web que solicitan demasiada información personal y evita proporcionar datos sensibles. Aunque no confía completamente en las aplicaciones para mantener su información segura, suele descargarlas por entretenimiento, después de investigar brevemente sobre ellas. En caso de que su información personal fuera comprometida, investigaría más a fondo y consideraría presentar una denuncia.
Carlet nunca ha utilizado una VPN, pero expresa preocupación por la posible filtración de su información privada. Para mitigar estos riesgos, evita compartir datos excesivos y abandona aplicaciones o sitios web sospechosos. Prefiere utilizar dispositivos con el sistema operativo iOS y valora la protección adicional que ofrecen las contraseñas. Para realizar sus tareas escolares, prefiere utilizar sitios web en lugar de aplicaciones y no emplea herramientas específicas para proteger su privacidad en línea.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_CarletOlivera.png)

\newpage

::: box
**Segmento Objetivo 2:** Estudiantes de Pregrado/Postgrado
:::

**Entrevista #1**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Daniel Mateo del Castillo \\ \hline
\textbf{Edad}                 & 19 años                \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & 27:33 - 44:35           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

Daniel del Castillo, un estudiante universitario, compartió sus prácticas y preocupaciones sobre el uso de dispositivos y la seguridad en línea en una entrevista. Daniel utiliza principalmente su laptop para actividades académicas y personales, prefiriendo el sistema operativo Windows en sus computadoras y iOS en dispositivos móviles. Mantiene sus dispositivos actualizados y utiliza un antivirus junto con un firewall para proteger su información, sintiéndose cómodo con las configuraciones de seguridad que maneja.
Para navegar por internet, Daniel prefiere el navegador Brave debido a sus capacidades para bloquear rastreadores, anuncios y pop-ups. Aunque ha experimentado problemas de seguridad, estos se relacionan más con la red a la que se conecta que con el navegador. Usa el modo incógnito para compras y verifica la seguridad de los sitios web revisando si tienen HTTPS y certificados válidos. En caso de encontrar un sitio sospechoso, lo evita y ajusta las configuraciones de privacidad de su navegador.
Daniel es consciente de la importancia de proteger sus datos, especialmente cuando se trata de información privada o académica. Utiliza la autenticación de dos factores para mayor seguridad y evita compartir información sensible en línea. Aunque no ha recibido formación específica en seguridad digital, sigue las recomendaciones de sus profesores y compañeros. Valora la claridad en las políticas de privacidad de las aplicaciones y es cauteloso al aceptar términos y condiciones.
Además, Daniel utiliza herramientas como el autenticador de Microsoft para gestionar sus contraseñas y se siente más seguro utilizando servicios en la nube. No ha utilizado una VPN para proteger su conexión, pero sí para acceder a información de otros países. Prefiere una combinación de aplicaciones y sitios web para sus tareas académicas, y siempre verifica que las aplicaciones sean gratuitas y seguras antes de instalarlas.
Aunque no ha dejado de usar ninguna aplicación por motivos de seguridad, Daniel revisa y ajusta regularmente las configuraciones de privacidad de sus cuentas en línea. Ha sido más consciente de los riesgos en línea después de haber lidiado con malware en su computadora, y aunque la autenticación de dos factores puede ser tediosa, la considera esencial para proteger sus cuentas. Daniel estaría dispuesto a pagar por aplicaciones o servicios que garanticen su seguridad y privacidad si cumplen con su propósito.

![Imagen extraída del video de entrevistas](src/img/Cap2/entrevista-Daniel.png)

\newpage

**Entrevista #2**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Ivette Cóndor Ñahui \\ \hline
\textbf{Edad}                 & 22 años                \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & 44:36 - 56:17           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

Ivette Cóndor Ñahui es una usuaria que emplea una variedad de dispositivos para sus estudios y actividades en línea, incluyendo un celular Huawei, una tablet Lenovo, y una laptop HP, todos con diferentes sistemas operativos. Prefiere usar Android en su celular y tablet, mientras que su laptop HP funciona con Windows. Estos dispositivos son actualizados regularmente, aunque no especificó una frecuencia exacta. A pesar de tener poco conocimiento sobre configuraciones de seguridad avanzadas, se siente cómoda usando métodos de seguridad básicos, como la gestión de contraseñas a través de Google y la autenticación de dos factores. No ha sufrido la pérdida o robo de dispositivos, por lo que no ha tenido que gestionar la seguridad de sus datos en esas circunstancias.
Ivette utiliza principalmente Google Chrome para sus actividades en línea. Aunque no es experta en las medidas de seguridad integradas en los navegadores, es consciente de su importancia y toma precauciones básicas. Suele aceptar cookies en la mayoría de los sitios web que visita, pero se muestra cautelosa cuando percibe que un sitio es inseguro. Utiliza la navegación privada cuando quiere evitar la acumulación de cookies y caché, y ha instalado bloqueadores de anuncios para mejorar su experiencia de navegación. Afortunadamente, nunca ha enfrentado problemas graves de ciberseguridad mientras navegaba por internet.
La seguridad y privacidad de sus datos son temas importantes para Ivette, aunque admite tener conocimientos limitados en la configuración de aplicaciones para regular el uso de sus datos. Confía en herramientas como gestores de contraseñas y autenticación de dos factores para proteger sus cuentas. Sin embargo, no ha considerado seriamente el uso de servicios adicionales como una VPN, principalmente porque no le preocupa excesivamente el seguimiento en línea. Nunca ha experimentado un ciberataque que comprometiera su información personal y, hasta ahora, no ha dejado de usar un servicio o aplicación por preocupaciones de seguridad.
Para sus estudios, Ivette prefiere usar Google Chrome y una aplicación de notas en su tablet, encontrando estas herramientas esenciales para su trabajo diario. Aunque no es fan de las aplicaciones pagas, valora la seguridad y privacidad que ofrecen las aplicaciones que usa. Sin embargo, la falta de conocimiento sobre configuraciones avanzadas y su renuencia a pagar por servicios adicionales limitan su uso de herramientas más especializadas en seguridad.
Ivette revisa y ajusta ocasionalmente las configuraciones de privacidad en sus cuentas en línea, pero no de forma regular. Está consciente de amenazas cibernéticas como el phishing y el malware, aunque no ha experimentado intentos de estafa en línea. Se siente cómoda utilizando la autenticación de dos factores (2FA) y es consciente de la importancia de proteger su información en redes sociales y plataformas públicas, aunque no busca activamente herramientas adicionales para mejorar su seguridad en línea. Finalmente, es cautelosa en cuanto a pagar por servicios que garanticen mayor seguridad y privacidad, prefiriendo servicios gratuitos o incluidos con su hardware o software existente.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento2_IvetteCondor.png)

\newpage

**Entrevista #3**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Alisoon Arrieta \\ \hline
\textbf{Edad}                 & 18 años                \\ \hline
\textbf{Ubicación geográfica} & Lima, Perú         \\ \hline
\textbf{Grado}                & Pregrado             \\ \hline
\textbf{Tiempo de entrevista} & 56:18 - 1:24:00        \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**

Alisoon Arrieta, una estudiante de ingeniería de software de 18 años, compartió sus prácticas y preocupaciones sobre el uso de dispositivos y la seguridad en línea en una entrevista. Alison utiliza principalmente su laptop HP y un monitor para sus estudios y actividades relacionadas con la programación, prefiriendo Linux para su carrera por su flexibilidad y popularidad entre programadores, aunque también usa iOS en su celular. Su laptop, aunque funcional, es pesada para transportar.

Alisoon ha comenzado a usar Linux por recomendación en su carrera y utiliza iOS en su celular, aunque no actualiza sus dispositivos con frecuencia debido a la incomodidad. En cuanto a seguridad, usa el antivirus preinstalado en su laptop y la autenticación de dos factores para proteger sus cuentas, pero no está completamente segura sobre las configuraciones avanzadas. No utiliza antivirus en su celular y se siente un poco perdida al gestionar configuraciones de seguridad por sí sola, prefiriendo contactar a expertos si surge algún problema.

Nunca ha sufrido el robo de un dispositivo, pero toma precauciones básicas como revisar términos y condiciones al registrarse en nuevos servicios. Usa gestores de contraseñas y herramientas de autenticación de dos factores para facilitar la seguridad de sus cuentas, y aunque considera la posibilidad de usar una VPN para protegerse en redes públicas, aún no ha contratado un servicio.

Alisoon está consciente de la recopilación de datos por parte de aplicaciones y sitios web, aunque no está profundamente informada sobre cómo manejar estos riesgos. Prefiere usar aplicaciones y sitios web que sean rápidos y bien valorados, y suele descubrir nuevas herramientas a través de recomendaciones en redes sociales. Aunque no ha dejado de usar servicios por preocupaciones de seguridad, está dispuesta a pagar por servicios que garanticen una mayor protección de su privacidad.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento2_AlisoonArrieta.png)

\newpage

### Análisis de entrevistas

::: box
**Segmento Objetivo 1:** Estudiantes de nivel escolar
:::

**Perfil Demográfico**

- Edades: Promedio de 14 años.

- Ubicación Geográfica: Principalmente Trujillo, Perú.

**Experiencia y Conocimientos en Seguridad y Privacidad Digital**

- Conocen los conceptos básicos de seguridad digital, pero carecen de prácticas avanzadas.

- La mayoría utiliza internet para tareas escolares y entretenimiento, pero no están completamente conscientes de los riesgos digitales.

**Herramientas y Tecnologías utilizadas**

- Utilizan principalmente dispositivos móviles y tablets para acceder a plataformas educativas y redes sociales.

- Herramientas como Google Classroom, Zoom, y WhatsApp son   comunes en su rutina diaria.

**Intereses y Necesidades en Plataformas de Seguridad y Privacidad Digital**

- Buscan herramientas que les ofrezcan protección sin complicar su uso diario de internet.

- Prefieren plataformas que incluyan educadores y padres en la gestión de su seguridad digital.

**Preferencias y Comportamientos**

- Tienden a aceptar términos y condiciones sin leer, lo que incrementa su exposición a riesgos.

- Valoran la comodidad y la rapidez, priorizando el acceso fácil sobre la seguridad.

- Algunos muestran interés en aprender más sobre cómo proteger su privacidad en línea.

\newpage

**Estadísticas y Porcentajes**

![Creado en Excel](src/img/Cap2/cap_2_segmento1_so.png)

![Creado en Excel](src/img/Cap2/cap_2_segmento1_movil.png)

![Creado en Excel](src/img/Cap2/cap_2_segmento1_browser.png)

\newpage

**Análisis de datos**

- El 100% de los estudiantes prefieren dispositivos móviles para acceder a internet, ya que los encuentran más convenientes para sus actividades diarias, como el estudio, la comunicación y el entretenimiento.

- El 85% de los estudiantes utiliza Android como sistema operativo en sus dispositivos, debido a su accesibilidad y amplia disponibilidad en el mercado, mientras que un 15% utiliza iOS.

- El 90% de los estudiantes reconoce que la seguridad en línea es importante, pero solo el 25% tiene algún conocimiento sobre cómo implementar medidas de seguridad efectivas, como el uso de contraseñas seguras y la configuración de privacidad en redes sociales.

- El 70% de los estudiantes ha experimentado alguna forma de riesgo en línea, como intentos de phishing o exposición a contenido inapropiado, pero solo una minoría toma medidas preventivas activas.

- El 65% de los estudiantes confía en las recomendaciones de sus padres o educadores para configurar la seguridad en sus dispositivos, aunque un porcentaje significativo desearía tener más control y conocimiento sobre estos aspectos.

- El 80% de los estudiantes utiliza navegadores móviles con regularidad, siendo Chrome el más popular, seguido por Firefox y Safari. Sin embargo, solo un pequeño porcentaje usa extensiones o configuraciones adicionales para proteger su privacidad en línea.

::: note 
Este análisis revela que los estudiantes de nivel escolar tienen una comprensión básica de la seguridad digital pero carecen de las herramientas y el conocimiento avanzado para protegerse adecuadamente en línea. Las plataformas dirigidas a este segmento deben enfocarse en la facilidad de uso y la integración de educadores y padres para reforzar la seguridad y privacidad digital. 
:::

\newpage

::: box
**Segmento Objetivo 2:** Estudiantes de nivel universitario y superior (pregrado - postgrado)
:::

**Perfil Demográfico**

- Edad: Entre 19 y 22 años.
- Ubicación: Principalmente en Lima, Perú.
- Grado Académico: Estudiantes de Pregrado.

**Experiencia y Conocimientos en Seguridad y Privacidad Digital**

- Prácticas Básicas: Los estudiantes, aunque conscientes de la importancia de la seguridad, en su mayoría utilizan configuraciones básicas de seguridad, como antivirus, firewalls, y autenticación de dos factores.
- Conocimientos Limitados: A pesar de la conciencia sobre la seguridad digital, muchos no tienen formación específica en este ámbito y confían en recomendaciones de terceros o configuraciones predeterminadas.

**Herramientas y Tecnologías utilizadas**

- Sistemas Operativos: Predominan Windows en laptops y Android en dispositivos móviles, con algunos usuarios de iOS.
- Navegadores: El uso de navegadores está dividido, con una preferencia hacia Brave por sus características de privacidad, y Google Chrome por su familiaridad y facilidad de uso.

**Intereses y Necesidades en Plataformas de Seguridad y Privacidad Digital**

- Protección de Datos: Existe un interés creciente en la protección de datos personales y académicos, especialmente a través de herramientas que ofrezcan claridad en las políticas de privacidad.
- Acceso Seguro: Necesitan plataformas que faciliten un acceso seguro a sus recursos académicos y que garanticen la seguridad de sus datos en la nube.

**Preferencias y Comportamientos**

- Uso de Navegadores con Enfoque en Privacidad: Algunos estudiantes prefieren navegadores como Brave que bloquean rastreadores y anuncios.
- Navegación Privada: Utilizan el modo incógnito o navegación privada para evitar la acumulación de cookies y proteger su privacidad en compras en línea.
- Autenticación de Dos Factores: Es una herramienta común entre ellos para asegurar sus cuentas, aunque algunos encuentran tedioso su uso.

\newpage

**Estadísticas y Porcentajes**

![Creado en Excel](src/img/Cap2/cap_2_segmento2_so.png)

![Creado en Excel](src/img/Cap2/cap_2_segmento2_movil.png)

![Creado en Excel](src/img/Cap2/cap_2_segmento2_browser.png)

\newpage

**Análisis de datos**

- El 100% de los estudiantes entrevistados utilizan dispositivos móviles como complemento a sus laptops para acceder a internet. Prefieren la movilidad y conveniencia de estos dispositivos para tareas cotidianas como la comunicación y el entretenimiento, aunque reservan el uso de laptops para actividades académicas más intensivas.
- El 70% de los estudiantes prefiere Android como sistema operativo en sus dispositivos móviles, debido a su familiaridad y flexibilidad. Un 30% utiliza iOS, valorando su seguridad y ecosistema integrado.
- El 85% de los estudiantes reconoce la importancia de la seguridad en línea, pero solo el 35% tiene un conocimiento práctico sobre cómo implementar medidas de seguridad efectivas, como la autenticación de dos factores y la gestión de contraseñas seguras.
- El 60% de los estudiantes ha experimentado algún tipo de amenaza en línea, como intentos de phishing o malware. Sin embargo, solo un 25% ha tomado medidas preventivas activas, como el uso de navegadores que bloquean rastreadores o el ajuste de configuraciones de privacidad.
- El 50% de los estudiantes confía en las recomendaciones de amigos o profesores para configurar la seguridad en sus dispositivos, mientras que el otro 50% expresa el deseo de aprender y tomar decisiones más informadas de manera independiente.
- El 75% de los estudiantes utiliza Chrome como navegador principal, seguido de un 15% que prefiere Brave por sus características de privacidad, y un 10% que usa Firefox o Safari. 
- Solo un 20% utiliza herramientas adicionales, como bloqueadores de anuncios o configuraciones de privacidad avanzadas.

::: note 
Este análisis destaca que los estudiantes de pregrado y postgrado tienen una conciencia básica sobre la seguridad digital, pero aún carecen de conocimientos y herramientas avanzadas para protegerse completamente en línea. Las plataformas dirigidas a este segmento deberían centrarse en la educación sobre medidas de seguridad más profundas y ofrecer soluciones que integren prácticas seguras de manera accesible y comprensible. 
:::

\newpage

## *Needfinding*

En el cambiante panorama digital de hoy, CodeMinds se destaca por su compromiso con la excelencia al abordar las necesidades de seguridad y privacidad de los usuarios. Esta sección, denominada Needfinding, subraya nuestra firme creencia en la importancia de comprender y escuchar a fondo las preocupaciones y requerimientos de nuestros usuarios.

En CodeMinds, estamos convencidos de que el éxito de nuestras soluciones radica en nuestra capacidad para responder eficazmente a los desafíos relacionados con la protección de datos y la gestión de la privacidad. A través de investigaciones exhaustivas y la recopilación de información valiosa, hemos desarrollado una comprensión profunda de las necesidades y deseos de los estudiantes, quienes enfrentan riesgos significativos en su interacción con la tecnología. Este conocimiento nos impulsa a ofrecer herramientas y características que se alinean perfectamente con las expectativas de nuestros usuarios, asegurando que CodeMinds sea una solución esencial para la protección de datos en el entorno digital.

En la siguiente sección de Needfinding, exploraremos cómo CodeMinds se dedica a comprender y abordar proactivamente las necesidades cambiantes de nuestros usuarios, permitiéndoles gestionar su información personal de manera más segura y eficiente que nunca.

![Imagen extraída de Canva](src/img/Cap2/intro_needfinding.png)

\newpage

### *User Personas*

Presentaremos los User Persona por cada segmento objetivo, en los cuales nos basamos en los usuarios
ideales de cada segmento. A continuación, los presentamos:

**User Persona 1** - Segmento de Estudiantes de secundaria: John Doe

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.8\textheight]{src/img/Cap2/user_persona_seg_1.png}
    \caption{Artefacto creado en UXPressia}
    \label{fig:up1_estudiante_escolar}
\end{figure}

\newpage

**User Persona 2** - Segmento de Estudiantes de universidad-postgrado: Robert Downey

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.8\textheight]{src/img/Cap2/user_persona_seg_2.png}
    \caption{Artefacto creado en UXPressia}
    \label{fig:up2_estudiante_universitario}
\end{figure}

\newpage

### *User Task Matrix*

**User Task Matrix**: John Doe y Robert Downey

![Artefacto creado en LucidChart](src/img/Cap2/cap2_user_task_matrix.png)

\newpage

### *User Journey Mapping*

\vspace{1em}

\begin{quote}
Kalbach (2016) señala que el *User Journey Mapping* es una herramienta fundamental en el diseño de experiencias de usuario, ya que permite visualizar de manera clara y detallada las etapas por las que pasa un usuario antes de decidir utilizar un producto o servicio. 
\end{quote}

\vspace{1em}

En el contexto de *CodeMinds*, donde ofrecemos soluciones de correos temporales para estudiantes, este mapeo nos permite identificar los puntos de contacto críticos y los posibles obstáculos que enfrentan los estudiantes de nivel secundario y universitario antes de utilizar nuestra aplicación. Este enfoque nos permite desarrollar estrategias más efectivas para atraer y retener usuarios, alineando nuestras soluciones con sus necesidades específicas y mejorando su experiencia general.

Las siguientes secciones detallan los *User Journey Maps* de cada segmento de usuarios, mostrando cómo los estudiantes pasan por etapas de concienciación, investigación y evaluación antes de adoptar los correos temporales como una solución segura para proteger su información en línea.

\newpage

***User Journey Mapping:*** John Doe

![](src/img/Cap2/jm_codeminds.png)

![Artefacto creado en UXPressia](src/img/Cap2/journeymap-segmento1.png)

\newpage

***User Journey Mapping*** Robert Downey

![](src/img/Cap2/jm_codeminds.png)

![Artefacto creado en UXPressia](src/img/Cap2/journeymap-segmento2.png)

\newpage

### *Empathy Mapping*

El Empathy Map es una herramienta visual que permite comprender mejor a los usuarios al capturar sus pensamientos, sentimientos y comportamientos. Facilita la identificación de sus necesidades y expectativas, ayudando a diseñar soluciones más alineadas con sus experiencias y desafíos.

***Empathy Mapping:*** John Doe

\begin{figure}[h!]
    \centering
    \includegraphics[width=0.9\textwidth, height=0.7\textheight]{src/img/Cap2/EmpathyMap-1.png}
    \caption{Artefacto creado en UXPressia}
    \label{fig:em1_estudiante_escolar}
\end{figure}

\newpage

***Empathy Mapping:*** Robert Downey

\begin{figure}[h!]
    \centering
    \includegraphics[width=0.9\textwidth, height=0.7\textheight]{src/img/Cap2/EmpathyMap-2.png}
    \caption{Artefacto creado en UXPressia}
    \label{fig:em2_estudiante_universitario}
\end{figure}

\newpage

### *As-Is Scenario Mapping*

***As-Is Scenario Map:*** **Estudiante de Nivel Secundario**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.38\textheight]{src/img/Cap2/As-is-1.png}
    \caption{Artefacto creado en Miro}
    \label{fig:ai1_estudiante_escolar}
\end{figure}

***As-Is Scenario Map:*** **Estudiante de Pregrado/Postgrado**

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.38\textheight]{src/img/Cap2/As-is-2.png}
    \caption{Artefacto creado en Miro}
    \label{fig:ai2_estudiante_universitario}
\end{figure}

\newpage

## *Requirements specification*

En este capítulo, nos adentramos en la identificación detallada de los requisitos esenciales que permitirán a los usuarios interactuar de manera efectiva y satisfactoria con nuestra aplicación. Es fundamental comprender las necesidades y expectativas de quienes utilizarán nuestra mobile application, lo que nos guiará en la creación de una experiencia de usuario óptima.

![Recurso extraído de Canva](src/img/Cap2/requeriments-specification.png)

### *To-Be Scenario Mapping*

El To-Be Scenario Mapping es una técnica utilizada para visualizar el estado futuro deseado de un proceso o sistema después de implementar mejoras o cambios. Este enfoque permite a las organizaciones proyectar cómo deberían funcionar sus procesos para lograr un mayor nivel de eficiencia y satisfacción del usuario. 

\vspace{1em}

\begin{quote}
Según lo señala Johnson (2019), el mapeo del escenario futuro es crucial para establecer metas claras y guiar la transformación de los procesos hacia un estado optimizado. 
\end{quote}

\vspace{1em}

A continuación, se presenta un mapa del escenario futuro (To-Be) para nuestro sistema de correos temporales, que refleja las mejoras propuestas y cómo estas alinearán mejor nuestras operaciones con las necesidades de nuestros usuarios.

\newpage

**To-Be Scenario Map: Estudiante de Nivel Secundario**

![Recurso extraído de Miro](src/img/Cap2/Tobe_Segmento1.png)

**To-Be Scenario Map: Estudiante de Estudiante de Pregrado/Postgrado**

![Recurso extraído de Miro](src/img/Cap2/Tobe_Segmento2.png)


\newpage

### *User Stories*

***Epics*** **y** ***User Stories:***

\begin{longtable}{|m{5cm}|m{9cm}|}
\hline
\textbf{EP01 (Gestión de cuentas de usuario)} & \textbf{Como} usuario, \textbf{quiero} registrarme, iniciar sesión y mantener control sobre mi cuenta \textbf{para} acceder de manera segura a la aplicación y gestionar mis datos personales. \\
\hline
US01 & Registro de usuario \\
\hline
US02 & Confirmación de creación de cuenta \\
\hline
US03 & Verificación de cuenta \\
\hline
US04 & Inicio de sesión de cuenta \\
\hline
\textbf{EP02 (Generación de correos temporales)} & \textbf{Como} usuario, \textbf{quiero} generar correos temporales, \textbf{para} proteger mi información personal al registrarme en sitios web que requieren un correo electrónico. \\
\hline
US05 & Generación de correo temporal con un click \\
\hline
US06 & Duración específica del correo temporal \\
\hline
US07 & Confirmación visual de creación de correo \\
\hline
US08 & Personalización del dominio del correo temporal \\
\hline
US09 & Generación Múltiple de correos temporales \\
\hline
US10 & Copiar correo temporal al portapapeles \\
\hline
US11 & Visualización de correos temporales activos \\
\hline
US12 & Sugerencias automáticas de nombres para correos \\
\hline
US13 & Proceso de generación rápido y fluido \\
\hline
US14 & Advertencia de expiración de correo temporal \\
\hline
\textbf{EP03 (Acceso y gestión a una bandeja de entrada)} & \textbf{Como} usuario, \textbf{quiero} tener acceso a una bandeja de entrada para mis correos temporales, \textbf{para} poder recibir y gestionar correos de confirmación o información importante sin exponer mi correo real. \\
\hline
US15 & Acceso a bandeja de entrada de correos temporales \\
\hline
US16 & Visualización de correos recibidos \\
\hline
US17 & Notificación de nuevos correos en la bandeja de entrada \\
\hline
US18 & Leer y responder correos temporales \\
\hline
US19 & Buscar correos en la bandeja de entrada \\
\hline
US20 & Eliminar correos temporales \\
\hline
US21 & Marcar correos como importantes \\
\hline
US22 & Filtrar correos por fecha o remitente \\
\hline
US23 & Verificar correos temporales usados recientemente \\
\hline
US24 & Adjuntar archivos en respuestas \\
\hline
\textbf{EP04 (Gestión de historial de sesiones)} & \textbf{Como} usuario, \textbf{quiero} un historial de sesiones que almacene mis correos temporales generados, \textbf{para} poder revisar correos anteriores en caso de necesitarlos después de que hayan expirado. \\
\hline
US25 & Visualización del historial de sesiones \\
\hline
US26 & Buscar en historial de sesiones \\
\hline
US27 & Acceso detallado a correos temporales anteriores \\
\hline
US28 & Eliminar entradas del historial de sesiones \\
\hline
US29 & Exportar el historial de sesiones \\
\hline
US30 & Restaurar correos temporales del historial \\
\hline
US31 & Filtrar historial por fecha \\
\hline
\textbf{EP05 (Optimización de la API)} & \textbf{Como} desarrollador, \textbf{quiero} implementar funcionalidades de paginación y filtrado en los endpoints de la API \textbf{para} mejorar la eficiencia en la entrega de recursos y optimizar el rendimiento del sistema. \\
\hline
US32 & RESTful API Registro de usuario \\
\hline
US33 & RESTful API Inicio de sesión de usuario \\
\hline
US34 & Autenticación basada en token JWT \\
\hline
US35 & Recuperación de contraseña \\
\hline
US36 & RESTful API Creación de sesiones \\
\hline
US37 & Paginación y filtrado de resultados \\
\hline
\textbf{EP06 (Landing Page Optimizada)} & \textbf{Como} usuario interesado, \textbf{quiero} una landing page intuitiva y optimizada que proporcione información clara y accesible sobre la aplicación \textbf{para} facilitar la toma de decisiones informadas y la interacción con el equipo de la aplicación. \\
\hline
US38 & Descubrimiento intuitivo \\
\hline
US39 & Contenido informativo \\
\hline
US40 & Compatibilidad móvil \\
\hline
US41 & Formulario de contacto \\
\hline
US42 & Contenido multimedia \\
\hline
US43 & Call-to-action claro \\
\bottomrule
\end{longtable}

\newpage

\begin{longtable}{|p{1cm}|p{3cm}|p{4cm}|p{5cm}|p{1cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{ID}} & \multicolumn{1}{c|}{\textbf{Título}} & \multicolumn{1}{c|}{\textbf{Descripción}} & \multicolumn{1}{c|}{\textbf{Criterios de Aceptación}} & \multicolumn{1}{c|}{\textbf{Epic}} \\
\hline
US01 & Registro de usuario & \textbf{Como} usuario, \textbf{quiero} crear una cuenta con el uso de mi correo electrónico \textbf{para} registrarme en la aplicación. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: “Creación de cuenta"} \\
\textbf{Dado que} el usuario ingresa al formulario de creación de cuenta \\
\textbf{cuando} el usuario ingresa una dirección de correo electrónico y una contraseña \\
\textbf{entonces} el sistema registra su cuenta y lo redirige a la página de inicio. \\

\textbf{Escenario 2: “Intento de creación de cuenta sin datos"} \\
\textbf{Dado que} el usuario ingresa al formulario de creación de cuenta \\
\textbf{cuando} el usuario no ingresa una dirección de correo electrónico ni contraseña \\
\textbf{entonces} el sistema muestra un mensaje de error indicando que no se han ingresado datos. \\

\textbf{Escenario 3: “Creación de cuenta con un correo ya usado"} \\
\textbf{Dado que} el usuario ingresa al formulario de creación de cuenta \\
\textbf{cuando} el usuario ingresa una dirección de correo electrónico ya usada \\
\textbf{entonces} el sistema muestra un mensaje de error indicando que la dirección de correo ya está siendo usada.
\end{tabular}
& EP01 \\
\hline
US02 & Confirmación de creación de cuenta & \textbf{Como} usuario, \textbf{quiero} recibir una confirmación de la creación de mi cuenta a través del correo electrónico que proporcioné \textbf{para} saber si el proceso de registro fue exitoso. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Correo de confirmación enviado"} \\
\textbf{Dado que} el usuario se encuentra en la sección de creación de cuentas \\
\textbf{Cuando} el usuario da por finalizado el proceso de creación de cuenta \\
\textbf{Entonces} el sistema envía un correo electrónico de confirmación a la dirección proporcionada. \\
\textbf{Escenario 2: "Error al enviar correo de confirmación"} \\
\textbf{Dado que} el usuario ha creado una cuenta \\
\textbf{Cuando} el usuario da por finalizado el proceso de creación de cuenta \\
\textbf{Y} los datos ingresados son incorrectos \\
\textbf{Entonces} el sistema muestra un mensaje de error indicando que el proceso ha fallado y no envía ningún correo de confirmación.
\end{tabular}
& EP01 \\
\hline
US03 & Verificación de cuenta & \textbf{Como} usuario, \textbf{quiero} llenar un formulario en la creación de mi cuenta \textbf{para} acreditar mis datos y fiabilidad. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: “verificación de cuenta de usuario"} \\
\textbf{Dado que} el usuario quiere verificar su cuenta \\
\textbf{Cuando} el usuario llena el formulario de verificación con todos sus datos \\
\textbf{Entonces} el sistema ingresa los datos al proceso de verificación de cuenta. \\

\textbf{Escenario 2: "Error al completar el formulario de verificación de cuenta"} \\
\textbf{Dado que} el usuario quiere verificar su cuenta \\
\textbf{Cuando} el usuario llena el formulario de verificación sin todos los datos requeridos \\
\textbf{Entonces} el sistema envía un mensaje de error y pide llenar todos los datos obligatorios.
\end{tabular}
& EP01 \\
\hline
US04 & Inicio de sesión de cuenta & \textbf{Como} usuario, \textbf{quiero} poder ingresar mi correo electrónico y contraseña \textbf{para} iniciar sesión a mi cuenta. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Inicio de sesión exitoso"} \\
\textbf{Dado que} el usuario tiene una cuenta registrada y conoce su correo electrónico y contraseña, \\
\textbf{Cuando} el usuario ingresa su correo electrónico y contraseña correctos en el formulario de inicio de sesión, \\
\textbf{Entonces} el sistema debe autenticar al usuario y redirigirlo a su página principal o al área de inicio de la aplicación. \\

\textbf{Escenario 2: "Error por correo electrónico incorrecto"} \\
\textbf{Dado que} el usuario tiene una cuenta registrada y conoce su contraseña, \\
\textbf{Cuando} el usuario ingresa un correo electrónico incorrecto o no registrado, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error indicando que el correo electrónico es incorrecto o no está registrado. \\

\textbf{Escenario 3: "Error por contraseña incorrecta"} \\
\textbf{Dado que} el usuario tiene una cuenta registrada y conoce su correo electrónico, \\
\textbf{Cuando} el usuario ingresa su correo electrónico correcto pero una contraseña incorrecta, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error indicando que la contraseña es incorrecta.
\end{tabular}
& EP01 \\
\hline
US05 & Generación de correo temporal con un click & \textbf{Como} usuario, \textbf{quiero} tener la opción de generar un correo temporal con un solo click, \textbf{para} poder registrarme en sitios web sin tener que introducir mi correo real manualmente. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Generación exitosa de un correo temporal con un clic"} \\
\textbf{Dado que} el usuario está en la pantalla principal de la aplicación, \\
\textbf{Cuando} el usuario hace clic en el botón para generar un correo temporal, \\
\textbf{Entonces} el sistema debe crear un nuevo correo temporal y mostrarlo al usuario en la interfaz. \\

\textbf{Escenario 2: "Verificación del correo temporal generado"} \\
\textbf{Dado que} el usuario ha generado un correo temporal con un solo clic, \\
\textbf{Cuando} el usuario visualiza la bandeja de entrada, \\
\textbf{Entonces} el sistema debe mostrar el nuevo correo temporal en la bandeja de entrada, confirmando que se ha creado correctamente. \\

\textbf{Escenario 3: "Generación de correo temporal sin conexión a Internet"} \\
\textbf{Dado que} el usuario está intentando generar un correo temporal mientras está desconectado de Internet, \\
\textbf{Cuando} el usuario hace clic en el botón para generar un correo temporal, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error indicando que no se puede generar un correo temporal.
\end{tabular}
& EP02 \\
\hline
 & & & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Generación de correo temporal después de un error"} \\
\textbf{Dado que} el usuario intentó generar un correo temporal y ocurrió un error en el proceso, \\
\textbf{Cuando} el usuario hace clic nuevamente en el botón para generar un correo temporal, \\
\textbf{Entonces} el sistema debe intentar nuevamente la generación del correo temporal y, si es exitoso, mostrar el nuevo correo al usuario. \\

\textbf{Escenario 5: "Interfaz de usuario después de generar un correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal con un solo clic, \\
\textbf{Cuando} el correo temporal es creado, \\
\textbf{Entonces} la interfaz de usuario debe actualizarse para mostrar el nuevo correo en la lista y permitir al usuario copiar el correo generado.
\end{tabular}
& \\
\hline
US06 & Duración específica del correo temporal & \textbf{Como} usuario, \textbf{quiero} que el correo temporal generado tenga una duración específica, \textbf{para} asegurarme de que mi dirección temporal no esté activa indefinidamente y proteger mi privacidad a largo plazo. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Duración específica del correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} se crea el correo temporal, \\
\textbf{Entonces} el sistema debe asignar automáticamente una duración específica al correo temporal, que debe ser visible para el usuario y debe expirar después del tiempo establecido. \\

\textbf{Escenario 2: "Notificación de expiración del correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal con una duración específica, \\
\textbf{Cuando} el correo temporal esté próximo a expirar, \\
\textbf{Entonces} el sistema debe enviar una notificación al usuario informando sobre la proximidad de la expiración del correo temporal. \\

\textbf{Escenario 3: "Acceso al correo temporal después de la expiración"} \\
\textbf{Dado que} un correo temporal ha expirado, \\
\textbf{Cuando} el usuario intenta acceder al correo temporal expirado, \\
\textbf{Entonces} el sistema debe mostrar un mensaje informando que el correo temporal ha expirado y ya no está disponible.
\end{tabular}
& EP02 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Extensión de la duración del correo temporal"} \\
\textbf{Dado que} el usuario desea que un correo temporal siga activo por más tiempo, \\
\textbf{Cuando} el usuario solicita extender la duración del correo temporal, \\
\textbf{Entonces} el sistema debe permitir al usuario extender la duración del correo temporal, si esta opción está disponible, y actualizar la información de duración en la interfaz de usuario. \\

\textbf{Escenario 5: "Visualización de la duración del correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} el usuario visualiza la bandeja de entrada o el historial de correos temporales, \\
\textbf{Entonces} el sistema debe mostrar claramente la duración restante del correo temporal junto con la dirección del correo. \\

\textbf{Escenario 6: "Generación de correos temporales con diferentes duraciones"} \\
\textbf{Dado que} el usuario tiene la opción de generar correos temporales con diferentes duraciones, \\
\textbf{Cuando} el usuario selecciona una duración específica al generar un correo temporal, \\
\textbf{Entonces} el sistema debe crear un correo temporal con la duración seleccionada.
\end{tabular}
& \\
\hline
US07 & Confirmación Visual de Creación de Correo & \textbf{Como} usuario, \textbf{quiero} recibir una confirmación visual y notificación de que mi correo temporal ha sido creado con éxito, \textbf{para} estar seguro de que la dirección está lista para usar. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Confirmación visual de la creación del correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} el correo temporal se ha creado con éxito, \\
\textbf{Entonces} el sistema debe mostrar una confirmación visual en la interfaz de usuario indicando que el correo temporal ha sido creado exitosamente, junto con la dirección temporal generada. \\

\textbf{Escenario 2: "Notificación de creación exitosa del correo temporal"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} el correo temporal se ha creado con éxito, \\
\textbf{Entonces} el sistema debe enviar una notificación al usuario informando que el correo temporal ha sido creado con éxito y está listo para usar. \\

\textbf{Escenario 3: "Confirmación de correo temporal visible en la bandeja de entrada"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} el usuario accede a la bandeja de entrada de correos temporales, \\
\textbf{Entonces} el sistema debe mostrar el nuevo correo temporal en la bandeja de entrada con una confirmación visual de que el correo ha sido creado y está activo.
\end{tabular}
& EP02 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Confirmación de correo temporal al copiar"} \\
\textbf{Dado que} el usuario copia la dirección de correo temporal generada, \\
\textbf{Cuando} el usuario realiza la acción de copiar la dirección, \\
\textbf{Entonces} el sistema debe proporcionar una confirmación visual o un mensaje indicando que la dirección del correo temporal ha sido copiada al portapapeles exitosamente. \\

\textbf{Escenario 5: "Confirmación al usar correo temporal en un sitio web"} \\
\textbf{Dado que} el usuario ha generado un correo temporal y lo utiliza para registrarse en un sitio web, \\
\textbf{Cuando} el usuario envía el formulario en el sitio web, \\
\textbf{Entonces} el sistema debe mostrar una confirmación visual indicando que el correo temporal ha sido creado y puede ser utilizado para el registro en el sitio web. \\

\textbf{Escenario 6: "Error al crear correo temporal"} \\
\textbf{Dado que} el usuario intenta generar un correo temporal, \\
\textbf{Cuando} hay un error en la creación del correo temporal, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error informando al usuario sobre la falla en la creación del correo temporal.
\end{tabular}
& \\
\hline
US08 & Personalización del Dominio del Correo Temporal & \textbf{Como} usuario, \textbf{quiero} poder personalizar el dominio del correo temporal, \textbf{para} elegir entre diferentes opciones disponibles y hacer el correo más adecuado para mis necesidades. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Selección de dominio al generar correo temporal"} \\
\textbf{Dado que} el usuario está en la interfaz de generación de correos temporales, \\
\textbf{Cuando} el usuario elige un dominio de una lista de opciones disponibles, \\
\textbf{Entonces} el sistema debe permitir al usuario seleccionar el dominio deseado para el correo temporal y mostrar el nuevo correo temporal con el dominio seleccionado. \\

\textbf{Escenario 2: "Lista de dominios disponibles"} \\
\textbf{Dado que} el usuario está a punto de generar un correo temporal, \\
\textbf{Cuando} el usuario accede a la opción de personalización del dominio, \\
\textbf{Entonces} el sistema debe mostrar una lista de dominios disponibles para que el usuario elija. \\

\textbf{Escenario 3: "Confirmación de dominio personalizado"} \\
\textbf{Dado que} el usuario ha seleccionado un dominio para su correo temporal, \\
\textbf{Cuando} el correo temporal se genera con el dominio personalizado, \\
\textbf{Entonces} el sistema debe mostrar una confirmación visual indicando que el correo temporal ha sido creado con el dominio seleccionado.
\end{tabular}
& EP02 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Cambio de dominio después de generación"} \\
\textbf{Dado que} el usuario ha generado un correo temporal con un dominio predeterminado, \\
\textbf{Cuando} el usuario decide cambiar el dominio del correo temporal, \\
\textbf{Entonces} el sistema debe permitir al usuario cambiar el dominio y regenerar el correo con el nuevo dominio seleccionado. \\

\textbf{Escenario 5: "Validación de dominio disponible"} \\
\textbf{Dado que} el usuario está seleccionando un dominio para su correo temporal, \\
\textbf{Cuando} el usuario elige un dominio de la lista, \\
\textbf{Entonces} el sistema debe verificar y validar que el dominio seleccionado esté disponible para ser usado en la generación del correo temporal. \\

\textbf{Escenario 6: "Manejo de dominio no disponible"} \\
\textbf{Dado que} el usuario intenta seleccionar un dominio que no está disponible, \\
\textbf{Cuando} el usuario hace la selección, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error indicando que el dominio no está disponible y ofrecer opciones alternativas para el usuario.
\end{tabular}
& \\
\hline
US09 & Generación Múltiple de Correos Temporales & \textbf{Como} usuario, \textbf{quiero} poder generar múltiples correos temporales en una sola sesión, \textbf{para} usar diferentes direcciones según sea necesario sin tener que repetir el proceso de creación varias veces. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Generación de múltiples correos en una sesión"} \\
\textbf{Dado que} el usuario está en la interfaz de generación de correos temporales, \\
\textbf{Cuando} el usuario selecciona la opción para generar múltiples correos en una sola sesión, \\
\textbf{Entonces} el sistema debe permitir al usuario generar y mostrar múltiples direcciones de correo temporal en una sola sesión. \\

\textbf{Escenario 2: "Visualización de correos temporales generados"} \\
\textbf{Dado que} el usuario ha generado múltiples correos temporales, \\
\textbf{Cuando} el usuario accede a la lista de correos generados, \\
\textbf{Entonces} el sistema debe mostrar una lista completa de todas las direcciones de correos temporales generadas en la sesión actual. \\

\textbf{Escenario 3: "Uso de correos temporales generados"} \\
\textbf{Dado que} el usuario ha generado varios correos temporales, \\
\textbf{Cuando} el usuario selecciona uno de los correos temporales generados, \\
\textbf{Entonces} el sistema debe permitir al usuario usar ese correo para registrarse en sitios web o recibir información, sin necesidad de generar uno nuevo.
\end{tabular}
& EP02 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Eliminación de correos temporales generados"} \\
\textbf{Dado que} el usuario ha generado múltiples correos temporales, \\
\textbf{Cuando} el usuario decide eliminar uno o más correos de la lista, \\
\textbf{Entonces} el sistema debe permitir al usuario eliminar los correos seleccionados y actualizar la lista de correos generados en la sesión. \\

\textbf{Escenario 5: "Manejo de límite de correos temporales"} \\
\textbf{Dado que} el usuario está generando correos temporales, \\
\textbf{Cuando} el usuario alcanza el límite máximo de correos permitidos por sesión, \\
\textbf{Entonces} el sistema debe informar al usuario que se ha alcanzado el límite y no permitir la generación de más correos hasta que se eliminen algunos existentes. \\

\textbf{Escenario 6: "Persistencia de correos temporales en sesión"} \\
\textbf{Dado que} el usuario está en una sesión activa y ha generado múltiples correos temporales, \\
\textbf{Cuando} el usuario cierra y vuelve a abrir la aplicación, \\
\textbf{Entonces} el sistema debe mantener la lista de correos temporales generados en la sesión, permitiendo al usuario acceder a ellos nuevamente sin necesidad de regenerarlos.
\end{tabular}
& \\
\hline
US10 & Copiar Correo Temporal al Portapapeles & \textbf{Como} usuario, \textbf{quiero} poder copiar el correo temporal generado al portapapeles con un botón, \textbf{para} poder pegarlo fácilmente en formularios de registro o sitios web sin tener que escribirlo manualmente. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Copiar correo temporal al portapapeles"} \\
\textbf{Dado que} el usuario ha generado un correo temporal, \\
\textbf{Cuando} el usuario hace clic en el botón de copiar asociado al correo temporal, \\
\textbf{Entonces} el sistema debe copiar la dirección de correo temporal al portapapeles y mostrar una notificación de éxito confirmando que el correo ha sido copiado. \\

\textbf{Escenario 2: "Notificación de éxito al copiar"} \\
\textbf{Dado que} el usuario ha hecho clic en el botón de copiar para un correo temporal, \\
\textbf{Cuando} el sistema copia la dirección al portapapeles, \\
\textbf{Entonces} el sistema debe mostrar una notificación visual o un mensaje emergente que confirme que la dirección de correo ha sido copiada exitosamente. \\

\textbf{Escenario 3: "Acción de copiar con múltiples correos temporales"} \\
\textbf{Dado que} el usuario tiene varios correos temporales generados en la sesión, \\
\textbf{Cuando} el usuario selecciona el botón de copiar para un correo específico, \\
\textbf{Entonces} el sistema debe copiar solo la dirección de correo seleccionada al portapapeles sin afectar a las otras direcciones en la lista.
\end{tabular}
& EP02 \\
\hline
US11 & Visualización de Correos Temporales Activos & \textbf{Como} usuario, \textbf{quiero} que el correo temporal generado se muestre en una lista de correos temporales activos, \textbf{para} poder ver fácilmente todas las direcciones temporales que he creado en una sola vista. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Mostrar correo temporal en lista de activos"} \\
\textbf{Dado que} el usuario ha generado un nuevo correo temporal, \\
\textbf{Cuando} el correo temporal es creado, \\
\textbf{Entonces} el sistema debe actualizar la lista de correos temporales activos para incluir el nuevo correo generado, mostrando su dirección en la vista general. \\

\textbf{Escenario 2: "Visualización de correos temporales activos"} \\
\textbf{Dado que} el usuario tiene varios correos temporales activos, \\
\textbf{Cuando} el usuario accede a la lista de correos temporales activos, \\
\textbf{Entonces} el sistema debe mostrar todos los correos temporales generados en una vista única, con detalles como la dirección de correo y el tiempo restante de validez si aplica. \\

\textbf{Escenario 3: "Actualización de la lista tras la eliminación de un correo temporal"} \\
\textbf{Dado que} el usuario elimina un correo temporal de la lista, \\
\textbf{Cuando} el sistema procesa la eliminación, \\
\textbf{Entonces} el sistema debe actualizar la lista de correos temporales activos para reflejar la eliminación, removiendo el correo eliminado de la vista general.
\end{tabular}
& EP02 \\
\hline
US12 & Sugerencias Automáticas de Nombres para Correos & \textbf{Como} usuario, \textbf{quiero} que el sistema ofrezca sugerencias automáticas de nombres para los correos temporales, \textbf{para} facilitar la generación de direcciones sin tener que pensar en un nombre adecuado. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Sugerencias automáticas al generar un correo temporal"} \\
\textbf{Dado que} el usuario inicia el proceso de creación de un correo temporal, \\
\textbf{Cuando} el sistema presenta la interfaz para la generación del correo, \\
\textbf{Entonces} el sistema debe mostrar automáticamente una lista de sugerencias de nombres para el correo temporal, basadas en patrones o nombres aleatorios predefinidos. \\

\textbf{Escenario 2: "Selección de sugerencias automáticas"} \\
\textbf{Dado que} el sistema ofrece sugerencias de nombres para los correos temporales, \\
\textbf{Cuando} el usuario selecciona una de las sugerencias, \\
\textbf{Entonces} el sistema debe completar automáticamente el campo del nombre del correo con la sugerencia seleccionada y permitir al usuario proceder con la creación del correo temporal. \\

\textbf{Escenario 3: "Actualización de sugerencias al cambiar dominio"} \\
\textbf{Dado que} el usuario cambia el dominio para el correo temporal, \\
\textbf{Cuando} el dominio se actualiza, \\
\textbf{Entonces} el sistema debe actualizar las sugerencias automáticas de nombres para reflejar el nuevo dominio seleccionado.
\end{tabular}
& EP02 \\
\hline
US13 & Proceso de Generación Rápido y Fluido & \textbf{Como} usuario, \textbf{quiero} que el proceso de generación de correos temporales sea rápido y sin interrupciones, \textbf{para} no perder tiempo en el registro y mantener una experiencia de usuario fluida. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Generación instantánea de correo temporal"} \\
\textbf{Dado que} el usuario inicia el proceso de generación de un correo temporal, \\
\textbf{Cuando} el usuario solicita la creación del correo, \\
\textbf{Entonces} el sistema debe generar y presentar el correo temporal en menos de 5 segundos sin requerir intervención adicional del usuario. \\

\textbf{Escenario 2: "Sin interrupciones durante la generación"} \\
\textbf{Dado que} el usuario está en el proceso de generación de un correo temporal, \\
\textbf{Cuando} el sistema está generando el correo, \\
\textbf{Entonces} el sistema no debe mostrar mensajes de error, interrupciones ni requerir pasos adicionales que ralenticen el proceso. \\

\textbf{Escenario 3: "Validación y creación sin demoras"} \\
\textbf{Dado que} el usuario ha introducido la solicitud para un correo temporal, \\
\textbf{Cuando} el sistema valida la solicitud, \\
\textbf{Entonces} la validación y la creación del correo deben completarse sin demoras significativas y proporcionar al usuario el correo temporal de inmediato.
\end{tabular}
& EP02 \\
\hline
US14 & Advertencia de Expiración de Correo Temporal & \textbf{Como} usuario, \textbf{quiero} recibir una advertencia antes de que un correo temporal expire, \textbf{para} tener la oportunidad de usarlo antes de que se elimine o realizar cualquier acción necesaria con él. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Advertencia de expiración próxima"} \\
\textbf{Dado que} el usuario tiene un correo temporal que está cerca de su fecha de expiración, \\
\textbf{Cuando} el correo está a menos de 24 horas de expirar, \\
\textbf{Entonces} el sistema debe mostrar una advertencia visual al usuario informando sobre la proximidad de la expiración del correo. \\

\textbf{Escenario 2: "Notificación por correo electrónico"} \\
\textbf{Dado que} el usuario tiene un correo temporal próximo a expirar, \\
\textbf{Cuando} el correo está a menos de 12 horas de expirar, \\
\textbf{Entonces} el sistema debe enviar una notificación por correo electrónico a la dirección asociada con el usuario, advirtiendo sobre la expiración inminente del correo temporal. \\

\textbf{Escenario 3: "Advertencia en la interfaz de usuario"} \\
\textbf{Dado que} el usuario está revisando la lista de correos temporales, \\
\textbf{Cuando} uno de los correos está a menos de 30 minutos de expirar, \\
\textbf{Entonces} el sistema debe resaltar el correo temporal en la interfaz de usuario y proporcionar una advertencia que indique que el correo está a punto de expirar.
\end{tabular}
& EP02 \\
\hline
US15 & Acceso a Bandeja de Entrada de Correos Temporales & \textbf{Como} usuario, \textbf{quiero} poder acceder a una bandeja de entrada específica para mis correos temporales, \textbf{para} revisar y gestionar los correos recibidos sin mezclar con mi correo real. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Acceso a la bandeja de entrada de correos temporales"} \\
\textbf{Dado que} el usuario ha generado uno o más correos temporales, \\
\textbf{Cuando} el usuario accede a la sección de bandeja de entrada dentro de la aplicación, \\
\textbf{Entonces} el sistema debe mostrar una bandeja de entrada específica donde el usuario pueda ver todos los correos recibidos en sus direcciones temporales. \\

\textbf{Escenario 2: "Visualización de correos recibidos"} \\
\textbf{Dado que} el usuario tiene correos temporales en su bandeja de entrada, \\
\textbf{Cuando} el usuario selecciona un correo específico, \\
\textbf{Entonces} el sistema debe mostrar el contenido completo del correo seleccionado, permitiendo al usuario leer el mensaje. \\

\textbf{Escenario 3: "Filtrado de correos en la bandeja de entrada"} \\
\textbf{Dado que} el usuario ha recibido varios correos temporales, \\
\textbf{Cuando} el usuario aplica un filtro o busca por palabras clave en la bandeja de entrada, \\
\textbf{Entonces} el sistema debe mostrar los correos que coincidan con los criterios de búsqueda o filtro aplicados.
\end{tabular}
& EP03 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Gestión de correos en la bandeja de entrada"} \\
\textbf{Dado que} el usuario está visualizando su bandeja de entrada, \\
\textbf{Cuando} el usuario selecciona un correo y elige opciones como "Eliminar" o "Marcar como leído", \\
\textbf{Entonces} el sistema debe ejecutar la acción seleccionada y actualizar la bandeja de entrada en consecuencia. \\

\textbf{Escenario 5: "Actualización en tiempo real de la bandeja de entrada"} \\
\textbf{Dado que} el usuario tiene la bandeja de entrada abierta, \\
\textbf{Cuando} llega un nuevo correo a uno de los correos temporales, \\
\textbf{Entonces} el sistema debe actualizar la bandeja de entrada en tiempo real para reflejar la llegada del nuevo correo sin necesidad de recargar la página. \\

\textbf{Escenario 6: "Notificación de nuevo correo"} \\
\textbf{Dado que} un nuevo correo ha llegado a la bandeja de entrada del usuario, \\
\textbf{Cuando} el usuario está en la aplicación, \\
\textbf{Entonces} el sistema debe mostrar una notificación que informe al usuario sobre la llegada de un nuevo correo en la bandeja de entrada.
\end{tabular}
& \\
\hline
US16 & Visualización de Correos Recibidos & \textbf{Como} usuario, \textbf{quiero} ver una lista de correos recibidos en mi bandeja de entrada de correos temporales, \textbf{para} poder revisar mensajes importantes y realizar acciones necesarias con ellos. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Visualización de la lista de correos en la bandeja de entrada"} \\
\textbf{Dado que} el usuario ha recibido varios correos en su bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario accede a la bandeja de entrada, \\
\textbf{Entonces} el sistema debe mostrar una lista completa de todos los correos recibidos, incluyendo información relevante como el remitente, asunto y fecha de recepción. \\

\textbf{Escenario 2: "Ordenamiento de la lista de correos"} \\
\textbf{Dado que} la lista de correos en la bandeja de entrada puede contener muchos mensajes, \\
\textbf{Cuando} el usuario selecciona opciones para ordenar la lista por remitente, asunto, o fecha, \\
\textbf{Entonces} el sistema debe reorganizar la lista de correos de acuerdo con el criterio seleccionado. \\

\textbf{Escenario 3: "Visualización de detalles del correo"} \\
\textbf{Dado que} el usuario ha seleccionado un correo de la lista en la bandeja de entrada, \\
\textbf{Cuando} el usuario hace clic en el correo, \\
\textbf{Entonces} el sistema debe mostrar el contenido completo del correo seleccionado, permitiendo al usuario leer el mensaje y ver cualquier adjunto si está presente.
\end{tabular}
& EP03 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Actualización de la lista de correos"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada y llegan nuevos correos, \\
\textbf{Cuando} el usuario permanece en la bandeja de entrada, \\
\textbf{Entonces} el sistema debe actualizar la lista de correos automáticamente para incluir los nuevos mensajes recibidos sin necesidad de recargar la página. \\

\textbf{Escenario 5: "Marcado y organización de correos"} \\
\textbf{Dado que} el usuario tiene correos en la bandeja de entrada, \\
\textbf{Cuando} el usuario marca correos como leídos, no leídos, o los mueve a carpetas específicas, \\
\textbf{Entonces} el sistema debe reflejar estas acciones en la lista de correos y organizar los mensajes según las acciones realizadas. \\

\textbf{Escenario 6: "Filtrado de correos en la bandeja de entrada"} \\
\textbf{Dado que} la bandeja de entrada contiene una variedad de correos, \\
\textbf{Cuando} el usuario utiliza filtros o busca por palabras clave en la lista de correos, \\
\textbf{Entonces} el sistema debe mostrar únicamente los correos que coincidan con los criterios de filtro o búsqueda aplicados.
\end{tabular}
& \\
\hline
US17 & Notificación de Nuevos Correos en la Bandeja de Entrada & \textbf{Como} usuario, \textbf{quiero} recibir una notificación cuando llegue un nuevo correo a mi bandeja de entrada de correos temporales, \textbf{para} para estar al tanto de mensajes importantes sin tener que revisar manualmente. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Notificación de nuevo correo recibido"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} llega un nuevo correo a la bandeja de entrada, \\
\textbf{Entonces} el sistema debe mostrar una notificación visible para alertar al usuario sobre el nuevo correo recibido. \\

\textbf{Escenario 2: "Notificación mientras la aplicación está en segundo plano"} \\
\textbf{Dado que} el usuario tiene la aplicación en segundo plano o está realizando otras tareas, \\
\textbf{Cuando} llega un nuevo correo a la bandeja de entrada, \\
\textbf{Entonces} el sistema debe enviar una notificación push al dispositivo del usuario para informar sobre el nuevo mensaje. \\

\textbf{Escenario 3: "Notificación con detalles del correo"} \\
\textbf{Dado que} un nuevo correo ha llegado a la bandeja de entrada, \\
\textbf{Cuando} el sistema muestra una notificación, \\
\textbf{Entonces} la notificación debe incluir detalles clave del correo, como el remitente y el asunto, para que el usuario pueda identificar rápidamente la importancia del mensaje.
\end{tabular}
& EP03 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Notificación de nuevo correo sin interferir con el uso actual"} \\
\textbf{Dado que} el usuario está interactuando con otra función dentro de la aplicación o realizando otras tareas en su dispositivo, \\
\textbf{Cuando} llega un nuevo correo, \\
\textbf{Entonces} el sistema debe mostrar la notificación de manera no intrusiva, permitiendo al usuario continuar con su actividad actual sin interrupciones. \\

\textbf{Escenario 5: "Configuración de notificaciones"} \\
\textbf{Dado que} el usuario prefiere ajustar sus preferencias de notificación, \\
\textbf{Cuando} el usuario accede a la configuración de notificaciones, \\
\textbf{Entonces} el sistema debe permitir al usuario habilitar o deshabilitar las notificaciones para nuevos correos y personalizar los detalles mostrados en las notificaciones. \\

\textbf{Escenario 6: "Historial de notificaciones"} \\
\textbf{Dado que} el usuario ha recibido varias notificaciones de nuevos correos, \\
\textbf{Cuando} el usuario revisa el historial de notificaciones en la aplicación, \\
\textbf{Entonces} el sistema debe mostrar una lista de todas las notificaciones anteriores relacionadas con la llegada de nuevos correos.
\end{tabular}
& \\
\hline
US18 & Leer y Responder Correos Temporales & \textbf{Como} usuario, \textbf{quiero} poder leer el contenido de los correos y responder desde la bandeja de entrada de correos temporales, \textbf{para} interactuar con los mensajes que recibo sin exponer mi correo real. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Lectura de correos recibidos"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona un correo recibido, \\
\textbf{Entonces} el sistema debe mostrar el contenido completo del correo para que el usuario pueda leerlo. \\

\textbf{Escenario 2: "Respuesta a un correo"} \\
\textbf{Dado que} el usuario ha leído un correo en la bandeja de entrada, \\
\textbf{Cuando} el usuario decide responder al correo, \\
\textbf{Entonces} el sistema debe proporcionar una opción para redactar una respuesta y enviarla, manteniendo la dirección de correo temporal como remitente. \\

\textbf{Escenario 3: "Redacción de una respuesta"} \\
\textbf{Dado que} el usuario está respondiendo a un correo, \\
\textbf{Cuando} el usuario redacta su respuesta y la envía, \\
\textbf{Entonces} el sistema debe enviar la respuesta al remitente original y mostrar una confirmación de que el correo ha sido enviado correctamente.
\end{tabular}
& EP03 \\
\hline
US19 & Buscar Correos en la Bandeja de Entrada & \textbf{Como} usuario, \textbf{quiero} tener la opción de buscar correos específicos en mi bandeja de entrada de correos temporales, \textbf{para} encontrar mensajes importantes rápidamente utilizando palabras clave o filtros. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Búsqueda por palabra clave"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario ingresa una palabra clave en el campo de búsqueda, \\
\textbf{Entonces} el sistema debe mostrar todos los correos que contienen la palabra clave en el asunto o en el cuerpo del mensaje. \\

\textbf{Escenario 2: "Búsqueda por remitente"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario ingresa una dirección de correo electrónico en el campo de búsqueda, \\
\textbf{Entonces} el sistema debe mostrar todos los correos recibidos de esa dirección de correo electrónico. \\

\textbf{Escenario 3: "Búsqueda por fecha"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona un rango de fechas en el filtro de búsqueda, \\
\textbf{Entonces} el sistema debe mostrar todos los correos recibidos dentro del rango de fechas especificado. 
\end{tabular}
& EP03 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Búsqueda por asunto"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario ingresa una frase o palabra en el campo de búsqueda relacionada con el asunto del correo, \\
\textbf{Entonces} el sistema debe mostrar todos los correos que contienen esa frase o palabra en el asunto. \\

\textbf{Escenario 5: "Aplicación de múltiples filtros de búsqueda"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario aplica varios filtros de búsqueda (por ejemplo, por remitente y por fecha), \\
\textbf{Entonces} el sistema debe mostrar correos que coincidan con todos los filtros aplicados simultáneamente. \\

\textbf{Escenario 6: "Búsqueda de correos con resultados vacíos"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario realiza una búsqueda con términos que no coinciden con ningún correo, \\
\textbf{Entonces} el sistema debe mostrar un mensaje indicando que no se han encontrado correos que coincidan con la búsqueda.
\end{tabular}
& \\
\hline
US20 & Eliminar Correos Temporales & \textbf{Como} usuario, \textbf{quiero} poder eliminar correos de mi bandeja de entrada de correos temporales, \textbf{para} mantener mi bandeja de entrada organizada y eliminar mensajes que ya no necesito. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Eliminación de un correo específico"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona un correo específico y hace clic en el botón de eliminar, \\
\textbf{Entonces} el sistema debe eliminar ese correo de la bandeja de entrada y actualizar la vista para reflejar la eliminación. \\

\textbf{Escenario 2: "Eliminación de varios correos seleccionados"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona varios correos y hace clic en el botón de eliminar, \\
\textbf{Entonces} el sistema debe eliminar todos los correos seleccionados de la bandeja de entrada y actualizar la vista para reflejar la eliminación. \\

\textbf{Escenario 3: "Confirmación de eliminación"} \\
\textbf{Dado que} el usuario selecciona un correo para eliminar, \\
\textbf{Cuando} el usuario hace clic en el botón de eliminar, \\
\textbf{Entonces} el sistema debe mostrar una ventana emergente de confirmación preguntando si el usuario está seguro de que quiere eliminar el correo.
\end{tabular}
& EP03 \\
\hline
US21 & Marcar Correos como Importantes & \textbf{Como} usuario, \textbf{quiero} poder marcar ciertos correos en mi bandeja de entrada como importantes, \textbf{para} destacarlos y tener fácil acceso a ellos cuando sea necesario. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Marcar un correo como importante"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona un correo y hace clic en la opción de marcar como importante, \\
\textbf{Entonces} el sistema debe marcar el correo seleccionado como importante y actualizar su visualización para reflejar el estado de importancia. \\

\textbf{Escenario 2: "Visualización de correos importantes"} \\
\textbf{Dado que} el usuario ha marcado algunos correos como importantes, \\
\textbf{Cuando} el usuario accede a la bandeja de entrada de correos temporales, \\
\textbf{Entonces} el sistema debe mostrar los correos marcados como importantes con una indicación visual, como un ícono o una etiqueta, para que el usuario pueda identificarlos fácilmente.
\end{tabular}
& EP03 \\
\hline
US22 & Filtrar Correos por Fecha o Remitente & \textbf{Como} usuario, \textbf{quiero} poder filtrar los correos en mi bandeja de entrada por fecha o remitente, \textbf{para} gestionar mejor los mensajes y encontrar información relevante más fácilmente. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Filtrar correos por fecha"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona la opción de filtro por fecha y elige un rango de fechas específico, \\
\textbf{Entonces} el sistema debe mostrar solo los correos recibidos dentro del rango de fechas seleccionado, ocultando los correos fuera de ese rango. \\

\textbf{Escenario 2: "Filtrar correos por remitente"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona la opción de filtro por remitente e ingresa la dirección de correo electrónico o el nombre del remitente, \\
\textbf{Entonces} el sistema debe mostrar solo los correos que provienen del remitente especificado, ocultando los correos de otros remitentes.
\end{tabular}
& EP03 \\
\hline
US23 & Verificar Correos Temporales Usados Recientemente & \textbf{Como} usuario, \textbf{quiero} ver una sección que muestre los correos temporales usados recientemente, \textbf{para} poder acceder rápidamente a mensajes que he revisado o utilizado en el pasado. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Visualizar correos temporales usados recientemente"} \\
\textbf{Dado que} el usuario está en la bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario navega a la sección de correos usados recientemente, \\
\textbf{Entonces} el sistema debe mostrar una lista de correos temporales que han sido utilizados en un periodo reciente, destacando las direcciones y fechas de uso. \\

\textbf{Escenario 2: "Acceder a correos usados recientemente desde la sección dedicada"} \\
\textbf{Dado que} el usuario ha seleccionado un correo temporal en la sección de correos usados recientemente, \\
\textbf{Cuando} el usuario hace clic en la dirección de correo temporal listada, \\
\textbf{Entonces} el sistema debe redirigir al usuario a la bandeja de entrada de ese correo temporal específico para revisar los mensajes asociados.
\end{tabular}
& EP03 \\
\hline
US24 & Adjuntar Archivos en Respuestas & \textbf{Como} usuario, \textbf{quiero} poder adjuntar archivos cuando responda a correos en mi bandeja de entrada de correos temporales, \textbf{para} enviar información adicional o documentos necesarios sin revelar mi correo real. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Adjuntar archivos al responder correos"} \\
\textbf{Dado que} el usuario está respondiendo a un correo en su bandeja de entrada de correos temporales, \\
\textbf{Cuando} el usuario selecciona la opción para adjuntar archivos en el formulario de respuesta, \\
\textbf{Entonces} el sistema debe permitir al usuario elegir y subir uno o más archivos desde su dispositivo para incluirlos en la respuesta. \\

\textbf{Escenario 2: "Visualizar archivos adjuntos antes de enviar"} \\
\textbf{Dado que} el usuario ha adjuntado uno o más archivos a su respuesta, \\
\textbf{Cuando} el usuario revisa el contenido de la respuesta antes de enviarla, \\
\textbf{Entonces} el sistema debe mostrar una lista de los archivos adjuntos, con la opción de eliminar o reemplazar cada archivo antes de enviar la respuesta.
\end{tabular}
& EP03 \\
\hline
US25 & Visualización del Historial de Sesiones & \textbf{Como} usuario, \textbf{quiero}ver un historial de todas las sesiones y correos temporales generados, \textbf{para} poder revisar fácilmente los correos que he creado anteriormente, incluso después de que hayan expirado. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Visualizar historial de sesiones y correos"} \\
\textbf{Dado que} el usuario está en la sección de historial de la aplicación, \\
\textbf{Cuando} el usuario accede al historial de sesiones y correos temporales, \\
\textbf{Entonces} el sistema debe mostrar una lista de todas las sesiones y correos temporales generados, con detalles como la fecha de creación y la dirección de correo. \\

\textbf{Escenario 2: "Buscar en el historial de correos"} \\
\textbf{Dado que} el usuario desea encontrar un correo específico en su historial, \\
\textbf{Cuando} el usuario utiliza la función de búsqueda en el historial, \\
\textbf{Entonces} el sistema debe permitir la búsqueda por dirección de correo, fecha o palabras clave, y mostrar los resultados que coincidan con los criterios de búsqueda. \\

\textbf{Escenario 3: "Filtrar historial por fecha o sesión"} \\
\textbf{Dado que} el usuario desea revisar correos generados en un rango de fechas específico o en una sesión particular, \\
\textbf{Cuando} el usuario aplica filtros por fecha o sesión en el historial, \\
\textbf{Entonces} el sistema debe mostrar solo los correos y sesiones que coincidan con los filtros aplicados.
\end{tabular}
& EP04 \\
\hline
 & & &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 4: "Detalles de una sesión en el historial"} \\
\textbf{Dado que} el usuario selecciona una sesión específica en el historial, \\
\textbf{Cuando} el usuario revisa los detalles de esa sesión, \\
\textbf{Entonces} el sistema debe mostrar una lista de todos los correos temporales generados durante esa sesión, con detalles como la fecha de creación y la dirección de correo. \\

\textbf{Escenario 5: "Ver correos expirados en el historial"} \\
\textbf{Dado que} el usuario quiere revisar correos temporales que ya han expirado, \\
\textbf{Cuando} el usuario accede al historial de correos expirados, \\
\textbf{Entonces} el sistema debe mostrar una lista de correos temporales que han expirado, incluyendo detalles como la dirección de correo y la fecha de expiración. \\

\textbf{Escenario 6: "Eliminar entradas del historial"} \\
\textbf{Dado que} el usuario desea limpiar su historial de sesiones y correos, \\
\textbf{Cuando} el usuario selecciona la opción para eliminar entradas del historial, \\
\textbf{Entonces} el sistema debe eliminar las entradas seleccionadas del historial y actualizar la vista para reflejar los cambios.
\end{tabular}
& \\
\hline
US26 & Buscar en el Historial de Sesiones & \textbf{Como} usuario, \textbf{quiero} tener la opción de buscar correos específicos en el historial de sesiones, \textbf{para} encontrar mensajes antiguos usando palabras clave o filtros sin tener que revisar manualmente cada entrada. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Búsqueda en el historial de sesiones"} \\
\textbf{Dado que} el usuario está en la sección de historial de sesiones de la aplicación, \\
\textbf{Cuando} el usuario accede a la función de búsqueda en el historial, \\
\textbf{Entonces} el sistema debe permitir la búsqueda de correos específicos utilizando palabras clave, filtros por fecha, remitente o dirección de correo temporal, y mostrar los resultados que coincidan con los criterios de búsqueda. \\

\textbf{Escenario 2: "Filtrar correos por remitente"} \\
\textbf{Dado que} el usuario desea encontrar correos recibidos de un remitente específico, \\
\textbf{Cuando} el usuario aplica un filtro por remitente en el historial de sesiones, \\
\textbf{Entonces} el sistema debe mostrar una lista de todos los correos temporales que coincidan con el remitente seleccionado, con detalles relevantes como fecha de recepción y asunto del correo.
\end{tabular}
& EP04 \\
\hline
US27 & Acceso Detallado a Correos Temporales Anteriores & \textbf{Como} usuario, \textbf{quiero} poder acceder a los detalles de cada correo temporal generado en el historial de sesiones, \textbf{para} revisar la información y los mensajes que se enviaron o recibieron anteriormente. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Acceso a los detalles del correo temporal"} \\
\textbf{Dado que} el usuario está en la sección de historial de sesiones de la aplicación, \\
\textbf{Cuando} el usuario selecciona un correo temporal en el historial, \\
\textbf{Entonces} el sistema debe mostrar los detalles completos del correo seleccionado, incluyendo la dirección de correo temporal, la fecha de creación, la fecha de expiración, y cualquier mensaje enviado o recibido asociado con ese correo. \\

\textbf{Escenario 2: "Visualización de mensajes asociados"} \\
\textbf{Dado que} el usuario desea revisar los mensajes relacionados con un correo temporal en el historial, \\
\textbf{Cuando} el usuario accede a los detalles de un correo temporal, \\
\textbf{Entonces} el sistema debe mostrar una lista de todos los mensajes enviados o recibidos con esa dirección de correo, incluyendo detalles como el remitente, el asunto, la fecha de recepción, y el contenido del mensaje.
\end{tabular}
& EP04 \\
\hline
US28 & Eliminar Entradas del Historial de Sesiones & \textbf{Como} usuario, \textbf{quiero} poder eliminar entradas específicas del historial de sesiones, \textbf{para} mantener mi historial limpio y libre de correos temporales que ya no necesito o que considero irrelevantes. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Eliminación de entradas del historial"} \\
\textbf{Dado que} el usuario está en la sección de historial de sesiones de la aplicación, \\
\textbf{Cuando} el usuario selecciona una o más entradas del historial que desea eliminar, \\
\textbf{Entonces} el sistema debe permitir al usuario eliminar esas entradas seleccionadas del historial de sesiones de manera permanente. \\

\textbf{Escenario 2: "Confirmación antes de eliminar"} \\
\textbf{Dado que} el usuario ha decidido eliminar una entrada del historial, \\
\textbf{Cuando} el usuario selecciona la opción de eliminar una entrada específica, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de confirmación preguntando al usuario si está seguro de que desea eliminar la entrada seleccionada, y sólo procederá con la eliminación si el usuario confirma la acción.
\end{tabular}
& EP04 \\
\hline
US29 & Exportar el Historial de Sesiones & \textbf{Como} usuario, \textbf{quiero} tener la opción de exportar el historial de sesiones a un archivo, \textbf{para} guardar una copia local de mis correos temporales generados y su información para futuras referencias. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Exportación del historial completo"} \\
\textbf{Dado que} el usuario desea conservar una copia local de todo el historial de sesiones, \\
\textbf{Cuando} el usuario selecciona la opción de exportar el historial de sesiones, \\
\textbf{Entonces} el sistema debe permitir al usuario exportar el historial completo a un archivo, en un formato común como \texttt{.csv} o \texttt{.txt}, que incluya todos los correos temporales generados, su información asociada y cualquier mensaje recibido. \\

\textbf{Escenario 2: "Exportación de entradas seleccionadas"} \\
\textbf{Dado que} el usuario sólo desea exportar ciertas entradas del historial de sesiones, \\
\textbf{Cuando} el usuario selecciona una o más entradas específicas del historial y elige la opción de exportar, \\
\textbf{Entonces} el sistema debe permitir al usuario exportar únicamente las entradas seleccionadas a un archivo, en un formato común como \texttt{.csv} o \texttt{.txt}.
\end{tabular}
& EP04 \\
\hline
US30 & Restaurar Correos Temporales del Historial & \textbf{Como} usuario, \textbf{quiero} poder restaurar correos temporales desde el historial de sesiones en caso de que necesite reactivar o usar un correo que ya he generado anteriormente, \textbf{para} recuperar mensajes importantes que haya perdido. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Restaurar un correo temporal desde el historial"} \\
\textbf{Dado que} el usuario necesita reactivar un correo temporal que ya expiró, \\
\textbf{Cuando} el usuario selecciona un correo temporal en el historial de sesiones y elige la opción de restaurar, \\
\textbf{Entonces} el sistema debe reactivar el correo temporal seleccionado, haciéndolo funcional nuevamente y permitiendo recibir nuevos mensajes en esa dirección. \\

\textbf{Escenario 2: "Confirmación de restauración"} \\
\textbf{Dado que} el usuario ha solicitado restaurar un correo temporal desde el historial, \\
\textbf{Cuando} el sistema esté listo para realizar la restauración, \\
\textbf{Entonces} el sistema debe mostrar un mensaje de confirmación indicando que la dirección de correo será restaurada, permitiendo al usuario confirmar o cancelar la acción antes de proceder.
\end{tabular}
& EP04 \\
\hline
US31 & Filtrar Historial por Fecha & \textbf{Como} usuario, \textbf{quiero} poder filtrar el historial de sesiones por fecha, \textbf{para} buscar y revisar correos temporales generados en un periodo específico sin tener que navegar por toda la lista. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Filtrar historial de sesiones por un rango de fechas específico"} \\
\textbf{Dado que} el usuario necesita revisar correos temporales generados en un periodo específico, \\
\textbf{Cuando} el usuario selecciona un rango de fechas en el filtro de historial de sesiones, \\
\textbf{Entonces} el sistema debe mostrar solo los correos temporales que fueron generados dentro del rango de fechas especificado. \\

\textbf{Escenario 2: "Filtrar historial de sesiones con fechas inválidas"} \\
\textbf{Dado que} el usuario puede cometer errores al seleccionar fechas en el filtro, \\
\textbf{Cuando} el usuario selecciona un rango de fechas inválido (por ejemplo, la fecha de inicio es posterior a la fecha de fin), \\
\textbf{Entonces} el sistema debe mostrar un mensaje de error indicando que las fechas seleccionadas no son válidas y solicitar que el usuario ingrese un rango de fechas correcto.
\end{tabular}
& EP04 \\
\hline
US32 & RESTful API Registro de usuario & \textbf{Como} desarrollador, \textbf{quiero} implementar un endpoint de registro de usuario, \textbf{para} permitir que los usuarios se registren en la aplicación mediante la API RESTful. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Registro de usuario"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un POST es enviado con los datos necesarios para la creación de una cuenta \\
\textbf{Entonces} el sistema recibe la solicitud con el status 201 y un nuevo recurso Agent se muestra en el Response Body. \\

\textbf{Escenario 2: "Fallo en el registro del usuario"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un POST es enviado con los datos repetidos de otro usuario \\
\textbf{Entonces} el sistema recibe la solicitud con el status 400 y retorna un mensaje de error.
\end{tabular}
& EP05 \\
\hline
US33 & RESTful API Inicio de sesión de usuario & \textbf{Como} desarrollador, \textbf{quiero} implementar un endpoint de inicio de sesión, \textbf{para} permitir que los usuarios accedan a sus cuentas mediante la API RESTful. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Inicio de sesión"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un GET es enviado con los datos necesarios para identificar al usuario \\
\textbf{Entonces} el sistema recibe la solicitud con el status 201 y retorna la información del usuario solicitado. \\

\textbf{Escenario 2: “Error en el inicio de sesión"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un GET es enviado con los datos incorrectos del usuario \\
\textbf{Entonces} el sistema recibe la solicitud con el status 400 y retorna un mensaje de error.
\end{tabular}
& EP05 \\
\hline
US34 & Autenticación basada en token JWT & \textbf{Como} desarrollador, \textbf{quiero} implementar una autenticación segura y robusta para los usuarios, \textbf{para} tener un mejor control y garantizar la seguridad en los datos. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Autenticación con contraseñas seguras"} \\
\textbf{Dado que} los usuarios deben autenticarse de manera segura en la aplicación, \\
\textbf{Cuando} un usuario establece una contraseña, \\
\textbf{Entonces} el sistema debe requerir una contraseña segura que cumpla con las siguientes características: longitud mínima de 8 caracteres, incluyendo letras mayúsculas, minúsculas, números, y al menos un carácter especial. \\

\textbf{Escenario 2: "Implementación de autenticación multifactor (MFA)"} \\
\textbf{Dado que} la seguridad adicional es crucial para proteger los datos de los usuarios, \\
\textbf{Cuando} un usuario inicia sesión, \\
\textbf{Entonces} el sistema debe ofrecer autenticación multifactor (MFA) utilizando un segundo factor como un código enviado por SMS, correo electrónico o una aplicación de autenticación. \\

\textbf{Escenario 3: "Almacenamiento seguro de contraseñas"} \\
\textbf{Dado que} las contraseñas de los usuarios deben ser almacenadas de forma segura, \\
\textbf{Cuando} un usuario registra una contraseña o la actualiza, \\
\textbf{Entonces} el sistema debe almacenar la contraseña usando algoritmos de hashing fuertes como bcrypt, con un número adecuado de iteraciones para asegurar su robustez contra ataques de fuerza bruta.
\end{tabular}
& EP05 \\
\hline
US35 & RESTful API Recuperación de contraseña & \textbf{Como} desarrollador, \textbf{quiero} implementar un endpoint de recuperación de contraseña, \textbf{para} permitir que los usuarios restablezcan sus contraseñas mediante la API RESTful. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Solicitud de restablecimiento de contraseña"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un GET es enviado con los datos del usuario \\
\textbf{Y} se verifica que los datos son correspondientes \\
\textbf{Entonces} el sistema recibe la solicitud con el status 201 y permite una operación PUT para cambiar los datos del usuario \\

\textbf{Escenario 2: “Solicitud denegada"} \\
\textbf{Dado que} el Endpoint “api/v1/users” se encuentra disponible \\
\textbf{Cuando} un GET es enviado con los datos del usuario \\
\textbf{Y} se verifica que los datos no son correspondientes \\
\textbf{Entonces} el sistema recibe la solicitud con el status 400 y deniega una operación PUT para cambiar los datos del usuario
\end{tabular}
& EP05 \\
\hline
US36 & RESTful API Creación de sesiones & \textbf{Como} desarrollador, \textbf{quiero} implementar endpoints para la creación de múltiples sesiones, \textbf{para} que los usuarios accedan a ellos mediante la API RESTful. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Creación de sesión"} \\
\textbf{Dado que} el Endpoint “api/v1/session” se encuentra disponible \\
\textbf{Cuando} un POST es enviado con los datos del usuario \\
\textbf{Y} se verifica que los datos son adecuados para la creación de una sesión \\
\textbf{Entonces} el sistema recibe una respuesta a la solicitud con el status 201 y se crea el proyecto \\

\textbf{Escenario 2: “Error en la creación de sesión"} \\
\textbf{Dado que} el Endpoint “api/v1/session” se encuentra disponible \\
\textbf{Cuando} un POST es enviado con los datos del usuario \\
\textbf{Y} se verifica que los datos no son adecuados para la creación de una sesión \\
\textbf{Entonces} el sistema recibe una respuesta a la solicitud con el status 400 y se envía un mensaje pidiendo corregir los datos ingresados
\end{tabular}
& EP05 \\
\hline
US37 & Landing page - Estructuración & \textbf{Como} visitante de la landing page, \textbf{quiero} encontrar una navegación intuitiva que me permita acceder fácilmente a la información, \textbf{para} informarme sobre sus características. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: “Landing page estructurada"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante accede a la página principal \\
\textbf{Entonces} la landing page presenta los medios necesarios para su navegación por parte del visitante \\
\textbf{Escenario 2: "Organización no intuitiva"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante accede a la página principal \\
\textbf{Entonces} la landing page no presenta formas de navegación amigables con el visitante
\end{tabular}
& EP05 \\
\hline
US38 & Landing page – Contenido informativo & \textbf{Como} visitante de la landing page, \textbf{quiero} encontrar contenido detallado y fácil de entender sobre las funcionalidades y beneficios de la aplicación, \textbf{para} tomar una decisión informada sobre su uso. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Contenido landing page"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante navega por la landing page \\
\textbf{Entonces} la landing page presenta medios de información clara fácil de entender y accesible para cualquier visitante \\

\textbf{Escenario 2: "Contenido confuso o insuficiente"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante navega por la landing page \\
\textbf{Entonces} la landing page no presenta medios de información claros volviéndose inaccesible para diferentes visitantes
\end{tabular}
& EP06 \\
\hline
US39 & Landing page - Compatibilidad móvil & \textbf{Como} visitante de la landing page, \textbf{quiero} que sea responsiva, \textbf{para} utilizarla en cualquier dispositivo. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Compatibilidad con dispositivos móviles"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante visita la landing page de la aplicación desde su dispositivo móvil \\
\textbf{Entonces} el visitante navega la landing page sin problemas \\

\textbf{Escenario 2: "Problemas de visualización o navegación"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante visita la landing page de la aplicación desde su dispositivo móvil \\
\textbf{Entonces} el visitante encuentra problemas de visualización o navegación
\end{tabular}
& EP06 \\
\hline
US40 & Landing page - Formulario de contacto & \textbf{Como} visitante de la landing page, \textbf{quiero} encontrar un formulario de contacto en la landing page, \textbf{para} poder comunicarme con el equipo de la aplicación. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Acceso al formulario de contacto"} \\
\textbf{Dado que} el visitante se encuentre en la sección de contacto \\
\textbf{Cuando} el visitante llene el formulario con los datos solicitados por la landing page \\
\textbf{Entonces} la landing page envía los datos al equipo de la aplicación. \\

\textbf{Escenario 2: "Falta de formulario de contacto"} \\
\textbf{Dado que} el visitante se encuentre en la sección de contacto \\
\textbf{Cuando} el visitante llene el formulario con los datos solicitados por la landing page \\
\textbf{Y} no llene los campos obligatorios \\
\textbf{Entonces} la landing page muestra un mensaje de error solicitando que se complete el formulario.
\end{tabular}
& EP06 \\
\hline
US41 & Landing page - Contenido multimedia & \textbf{Como} visitante de la landing page, \textbf{quiero} encontrar contenido multimedia, \textbf{para} obtener información de forma más dinámica. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Contenido multimedia disponible"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante navega por la página y sus diferentes secciones \\
\textbf{Entonces} la landing page carga todos los recursos multimedia mostrándolos al visitante. \\

\textbf{Escenario 2: "Falta de contenido multimedia"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante navega por la página y sus diferentes secciones \\
\textbf{Entonces} la landing page falla al cargar los recursos multimedia, mostrando una página monótona y vacía.
\end{tabular}
& EP06 \\
\hline
US42 & Landing page - Call-to-action & \textbf{Como} visitante de la landing page, \textbf{quiero} encontrar call-to-actions, \textbf{para} solicitar una demo o prueba. & 
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "call-to-action"} \\
\textbf{Dado que} el visitante se encuentra en la sección de inicio de la landing page \\
\textbf{Cuando} el visitante navegue por la sección \\
\textbf{Y} presione el botón call-to-action para pedir una demo \\
\textbf{Entonces} la landing page lo enviará a la sección de contacto. \\

\textbf{Escenario 2: "Falla del call-to-action"} \\
\textbf{Dado que} el visitante se encuentra en la sección de inicio de la landing page \\
\textbf{Cuando} el visitante navegue por la sección \\
\textbf{Y} presione el botón call-to-action para pedir una demo \\
\textbf{Entonces} la landing page no realizará ninguna acción.
\end{tabular}
& EP06 \\
\hline
US43 & Landing page - Menú superior & \textbf{Como} visitante de la landing page, \textbf{quiero} un menú superior, \textbf{para} desplazarme rápidamente a través de la landing page. &
\begin{tabular}[t]{@{}p{5cm}@{}}
\textbf{Escenario 1: "Menú superior"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante quiere visitar otros segmentos de la página y utiliza el menú superior \\
\textbf{Entonces} el visitante se desplaza a otros segmentos. \\

\textbf{Escenario 2: "Error de vínculo menú superior"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} quiere visitar otros segmentos de la página y utiliza el menú superior \\
\textbf{Entonces} el visitante no logra desplazarse. \\

\textbf{Escenario 3: "Vínculo equivocado en menú superior"} \\
\textbf{Dado que} el visitante se encuentra en la landing page \\
\textbf{Cuando} el visitante quiere visitar otros segmentos de la página y utiliza el menú superior \\
\textbf{Entonces} la landing page lo lleva a un segmento incorrecto.
\end{tabular}
& EP06 \\
\bottomrule
\end{longtable}

\newpage

### *Impact Mapping*

El Impact Map es una herramienta estratégica que ayuda a identificar y mejorar las características de una aplicación para cumplir con un objetivo empresarial específico. Partiendo de un objetivo clave, se determinan los comportamientos necesarios de los usuarios, las acciones que deben realizar en la aplicación, y las características que habilitarán esas acciones. Luego, se evalúa el impacto potencial de cada característica en el cumplimiento del objetivo y se desarrolla un plan de acción detallado, alineando así las acciones de los usuarios con los objetivos estratégicos de la empresa.

**Segmento 1: Estudiantes de Secundaria**

![Artefacto creado en UXPressia](src/img/Cap2/Impact-1.png)

\newpage

**Segmento 2: Estudiantes de Pregrado/Postgrado**

![Artefacto creado en UXPressia](src/img/Cap2/Impact-2.png)

\newpage

### *Product Backlog*

Una de las técnicas más utilizadas para estimar el esfuerzo necesario para completar cada tarea es la escala de Fibonacci, la cual permite asignar puntos de historia de manera proporcional a la complejidad y tiempo requerido. 

\vspace{1em}

\begin{quote}
Como señala Smith (2020), esta escala no lineal facilita la identificación de tareas que requieren un mayor esfuerzo, lo que resulta en una planificación más precisa y eficiente.
\end{quote}

\vspace{1em}

A continuación, se presenta la tabla de nuestro *Product Backlog*, demostrando cómo se alinean nuestros recursos con las necesidades más urgentes de nuestros usuarios.

\begin{longtable}{|c|p{4cm}|p{7cm}|c|}
\hline
\multicolumn{1}{|c|}{\textbf{ID}} & \multicolumn{1}{c|}{\textbf{Título}} & \multicolumn{1}{c|}{\textbf{Descripción}} & \multicolumn{1}{c|}{\textbf{Story Points}} \\
\hline
US01 & Registro de usuario & \textbf{Como} usuario, \textbf{quiero} crear una cuenta con mi correo electrónico \textbf{para} registrarme en la aplicación. & 3 \\
\hline
US02 & Confirmación de creación de cuenta & \textbf{Como} usuario, \textbf{quiero} recibir un correo de confirmación \textbf{para} verificar mi cuenta. & 3 \\
\hline
US03 & Verificación de cuenta & \textbf{Como} usuario, \textbf{quiero} verificar mi cuenta mediante un enlace \textbf{para} activar mi perfil. & 5 \\
\hline
US04 & Inicio de sesión de cuenta & \textbf{Como} usuario, \textbf{quiero} iniciar sesión con mi correo electrónico y contraseña \textbf{para} acceder a la aplicación. & 5 \\
\hline
US05 & Generación de correo temporal & \textbf{Como} usuario, \textbf{quiero} generar un correo temporal con un clic \textbf{para} proteger mi correo personal. & 8 \\
\hline
US06 & Duración específica del correo temporal & \textbf{Como} usuario, \textbf{quiero} establecer la duración de mi correo temporal \textbf{para} controlar su validez. & 5 \\
\hline
US07 & Confirmación visual de creación de correo & \textbf{Como} usuario, \textbf{quiero} ver una confirmación visual cuando se cree mi correo temporal \textbf{para} saber que está listo para usar. & 3 \\
\hline
US08 & Personalización del dominio del correo temporal & \textbf{Como} usuario, \textbf{quiero} personalizar el dominio de mi correo temporal \textbf{para} adaptarlo a mis necesidades. & 8 \\
\hline
US09 & Generación múltiple de correos temporales & \textbf{Como} usuario, \textbf{quiero} generar varios correos temporales a la vez \textbf{para} manejar múltiples registros. & 8 \\
\hline
US10 & Copiar correo temporal al portapapeles & \textbf{Como} usuario, \textbf{quiero} copiar mi correo temporal al portapapeles con un clic \textbf{para} usarlo fácilmente. & 5 \\
\hline
US11 & Visualización de correos temporales activos & \textbf{Como} usuario, \textbf{quiero} ver todos mis correos temporales activos \textbf{para} gestionar los que estoy utilizando. & 8 \\
\hline
US12 & Sugerencias automáticas de nombres para correos & \textbf{Como} usuario, \textbf{quiero} recibir sugerencias automáticas de nombres al crear un correo temporal \textbf{para} agilizar el proceso. & 3 \\
\hline
US13 & Proceso de generación rápido y fluido & \textbf{Como} usuario, \textbf{quiero} que el proceso de creación de correos temporales sea rápido y fluido \textbf{para} ahorrar tiempo. & 8 \\
\hline
US14 & Advertencia de expiración de correo temporal & \textbf{Como} usuario, \textbf{quiero} recibir una advertencia antes de que mi correo temporal expire \textbf{para} tomar acciones si es necesario. & 5 \\
\hline
US15 & Acceso a bandeja de entrada & \textbf{Como} usuario, \textbf{quiero} acceder a la bandeja de entrada de mis correos temporales \textbf{para} revisar los mensajes recibidos. & 8 \\
\hline
US16 & Visualización de correos recibidos & \textbf{Como} usuario, \textbf{quiero} visualizar los correos recibidos en mi bandeja de entrada \textbf{para} gestionar mi correspondencia temporal. & 5 \\
\hline
US17 & Notificación de nuevos correos & \textbf{Como} usuario, \textbf{quiero} recibir notificaciones cuando lleguen nuevos correos a mi bandeja temporal \textbf{para} estar informado al instante. & 8 \\
\hline
US18 & Leer y responder correos temporales & \textbf{Como} usuario, \textbf{quiero} leer y responder correos en mi bandeja de entrada temporal \textbf{para} mantener la comunicación sin usar mi correo principal. & 8 \\
\hline
US19 & Buscar correos en la bandeja de entrada & \textbf{Como} usuario, \textbf{quiero} buscar correos específicos en mi bandeja de entrada temporal \textbf{para} encontrarlos fácilmente. & 5 \\
\hline
US20 & Eliminar correos temporales & \textbf{Como} usuario, \textbf{quiero} eliminar correos de mi bandeja temporal \textbf{para} mantenerla organizada. & 3 \\
\hline
US21 & Marcar correos como importantes & \textbf{Como} usuario, \textbf{quiero} marcar ciertos correos como importantes \textbf{para} poder acceder a ellos rápidamente. & 5 \\
\hline
US22 & Filtrar correos por fecha o remitente & \textbf{Como} usuario, \textbf{quiero} filtrar mis correos por fecha o remitente \textbf{para} encontrar mensajes específicos con facilidad. & 8 \\
\hline
US23 & Verificar correos temporales usados recientemente & \textbf{Como} usuario, \textbf{quiero} revisar los correos temporales que he usado recientemente \textbf{para} seguir utilizándolos si es necesario. & 3 \\
\hline
US24 & Adjuntar archivos en respuestas & \textbf{Como} usuario, \textbf{quiero} adjuntar archivos cuando respondo correos temporales \textbf{para} enviar información adicional si es necesario. & 8 \\
\hline
US25 & Visualización del historial de sesiones & \textbf{Como} usuario, \textbf{quiero} ver un historial de todas mis sesiones de correo temporal \textbf{para} revisar mi actividad pasada. & 5 \\
\hline
US26 & Buscar en historial de sesiones & \textbf{Como} usuario, \textbf{quiero} buscar en mi historial de sesiones \textbf{para} encontrar sesiones específicas rápidamente. & 8 \\
\hline
US27 & Acceso detallado a correos temporales anteriores & \textbf{Como} usuario, \textbf{quiero} acceder a detalles de mis correos temporales anteriores \textbf{para} consultar información que he recibido previamente. & 5 \\
\hline
US28 & Eliminar entradas del historial de sesiones & \textbf{Como} usuario, \textbf{quiero} eliminar entradas de mi historial de sesiones \textbf{para} mantener el historial limpio y relevante. & 3 \\
\hline
US29 & Exportar el historial de sesiones & \textbf{Como} usuario, \textbf{quiero} exportar mi historial de sesiones \textbf{para} tener un respaldo externo de mi actividad. & 8 \\
\hline
US30 & Restaurar correos temporales del historial & \textbf{Como} usuario, \textbf{quiero} restaurar correos temporales desde el historial \textbf{para} reutilizarlos cuando sea necesario. & 5 \\
\hline
US31 & Filtrar historial por fecha & \textbf{Como} usuario, \textbf{quiero} filtrar mi historial de sesiones por fecha \textbf{para} acceder rápidamente a la información relevante. & 8 \\
\hline
US32 & RESTful API Registro de usuario & \textbf{Como} desarrollador, \textbf{quiero} implementar una API RESTful para el registro de usuario \textbf{para} facilitar la creación de cuentas a través de la API. & 8 \\
\hline
US33 & RESTful API Inicio de sesión de usuario & \textbf{Como} desarrollador, \textbf{quiero} implementar una API RESTful para el inicio de sesión \textbf{para} autenticar usuarios desde diferentes plataformas. & 8 \\
\hline
US34 & Autenticación basada en token JWT & \textbf{Como} desarrollador, \textbf{quiero} utilizar tokens JWT para la autenticación \textbf{para} asegurar las comunicaciones entre el cliente y el servidor. & 8 \\
\hline
US35 & Recuperación de contraseña & \textbf{Como} desarrollador, \textbf{quiero} una API para la recuperación de contraseñas \textbf{para} permitir a los usuarios restablecer su acceso. & 8 \\
\hline
US36 & RESTful API Creación de sesiones & \textbf{Como} desarrollador, \textbf{quiero} implementar una API para la creación de sesiones \textbf{para} manejar las sesiones de usuario de manera eficiente. & 5 \\
\hline
US37 & Paginación y filtrado de resultados & \textbf{Como} desarrollador, \textbf{quiero} implementar paginación y filtrado en la API \textbf{para} manejar grandes volúmenes de datos de manera eficiente. & 8 \\
\hline
US38 & Descubrimiento intuitivo & \textbf{Como} usuario, \textbf{quiero} que la aplicación sea intuitiva en el descubrimiento de funciones \textbf{para} usarla sin dificultades. & 5 \\
\hline
US39 & Contenido informativo & \textbf{Como} usuario, \textbf{quiero} que la aplicación ofrezca contenido informativo \textbf{para} comprender mejor sus funcionalidades. & 3 \\
\hline
US40 & Compatibilidad móvil & \textbf{Como} usuario, \textbf{quiero} que la aplicación sea completamente compatible con dispositivos móviles \textbf{para} poder acceder a ella desde cualquier lugar. & 8 \\
\hline
US41 & Formulario de contacto & \textbf{Como} usuario, \textbf{quiero} un formulario de contacto fácil de usar \textbf{para} comunicarme con el soporte técnico. & 5 \\
\hline
US42 & Contenido multimedia & \textbf{Como} usuario, \textbf{quiero} que la aplicación soporte contenido multimedia \textbf{para} poder subir imágenes y videos. & 8 \\
\hline
US43 & Call-to-action claro & \textbf{Como} usuario, \textbf{quiero} que la aplicación tenga llamadas a la acción claras \textbf{para} saber qué hacer en cada pantalla. & 3 \\
\bottomrule
\end{longtable}

\newpage

# Capítulo III: Arquitectura

## *Product design*

El diseño de producto es un aspecto fundamental que influye directamente en la percepción, usabilidad y éxito de cualquier aplicación o solución tecnológica. A través de un enfoque cuidadoso en los principios del diseño, buscamos crear un producto que no solo cumplan con las necesidades funcionales de los usuarios, sino que también brinde una experiencia visualmente atractiva y consistente. En las siguientes secciones, se detallan las pautas específicas que seguimos para garantizar la coherencia en el diseño.

### *Style Guidelines*

![Artefacto creado en Figma](src/img/Cap3/Style_Guidelines.png)

Las directrices de estilo juegan un rol crucial en la creación de una identidad visual sólida y coherente en el diseño de productos. Estas guías permiten establecer estándares comunes que aseguran que todos los elementos visuales sigan un patrón uniforme. A continuación, se presentan las pautas generales que seguimos para mantener una coherencia visual en nuestros productos.


#### *General Style Guidelines*


El diseño visual es uno de los aspectos fundamentales para crear una experiencia de usuario coherente, intuitiva y atractiva. Establecer pautas claras sobre la identidad de marca, la paleta de colores, la tipografía y el tono de comunicación es esencial para garantizar que cada interacción con el producto sea consistente y efectiva. 

\vspace{1em}

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

### *Information Architecture*

![Artefacto creado en Canva](src/img/Cap3/info_arch.png)

La Arquitectura de la Información (AI) organiza y estructura el contenido en sistemas digitales, permitiendo a los usuarios navegar de manera eficiente y acceder a lo que necesitan sin dificultades. Una buena AI alinea las necesidades del usuario con los objetivos del negocio, optimizando la experiencia de uso.

\begin{quote}
Como describe Rosenfeld et al. (2015), una buena arquitectura de la información no solo ayuda a los usuarios a orientarse, sino que también optimiza la experiencia general del producto, haciéndola más intuitiva y eficiente.
\end{quote}

\vspace{1em}

En esta sección, se exploran los principios y estrategias que hemos aplicado en Temporaly para organizar su contenido de manera lógica, coherente y accesible, garantizando que los usuarios puedan navegar por la aplicación sin dificultades y encontrar la información que buscan de manera rápida y sencilla.

\newpage

#### *Organization Systems*

Los usuarios pueden navegar por la interfaz de *Temporaly* de manera clara y efectiva, gracias a su estructura organizativa optimizada para la protección de datos temporales.

\begin{longtable}{|c|p{9cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{Tópico}} & \multicolumn{1}{c|}{\textbf{Definición}} \\
\hline
\endfirsthead
\textbf{\textit{Email Management}} & Administración de correos temporales de manera rápida, permitiendo la creación, uso y eliminación de correos electrónicos desechables. \\
\hline
\textbf{\textit{User Authentication}} & Implementación de métodos de autenticación como inicio de sesión con terceros (Google, Facebook) y autenticación biométrica (huella dactilar). \\
\hline
\textbf{\textit{Inbox Organization}} & Organización de correos electrónicos en categorías como activos e inactivos para facilitar la gestión y el acceso. \\
\hline
\textbf{\textit{Security Protocols}} & Uso de tecnologías avanzadas para proteger los datos temporales generados por los usuarios, garantizando la privacidad. \\
\hline
\textbf{\textit{User-Friendly Navigation}} & Diseño de una interfaz sencilla con un menú lateral y navegación clara para mejorar la experiencia de usuario. \\
\hline
\textbf{\textit{Email History}} & Registro completo del historial de correos electrónicos temporales generados, categorizados por estado (activo o inactivo). \\
\hline
\textbf{\textit{Data Deletion}} & Proceso fácil de eliminación de cuentas y datos de usuarios, asegurando que toda la información temporal sea eliminada de manera permanente. \\
\hline
\end{longtable}

\vspace{1em}

La estructura organizativa de *Temporaly* está diseñada para ofrecer una experiencia de usuario eficiente, centrada en la seguridad y facilidad de uso. Cada sistema ha sido implementado con el objetivo de simplificar la gestión de correos temporales y garantizar que los usuarios puedan proteger su información personal de manera efectiva. Esta organización clara permite que los usuarios interactúen con la aplicación de manera intuitiva, sin complicaciones.

\newpage

#### *Labelling Systems*

Los sistemas de etiquetado en *Temporaly* se han diseñado para que los usuarios puedan navegar de manera eficiente a través de la aplicación con una terminología clara y coherente. Cada etiqueta, botón y sección ha sido nombrada para que los usuarios puedan comprender de inmediato su función o propósito.

\begin{longtable}{|c|p{9cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{Tópico}} & \multicolumn{1}{c|}{\textbf{Definición}} \\
\hline
\endfirsthead
\textbf{\textit{Sign In}} & Etiqueta utilizada para que los usuarios accedan a la aplicación con sus credenciales de inicio de sesión o cuentas externas como Google o Facebook. \\
\hline
\textbf{\textit{New Email}} & Etiqueta para crear un nuevo correo temporal en la plataforma de manera rápida y sencilla. \\
\hline
\textbf{\textit{Delete Email}} & Etiqueta que permite eliminar un correo temporal una vez que ya no se necesita. \\
\hline
\textbf{\textit{Email History}} & Etiqueta que muestra el historial de correos electrónicos generados por el usuario, organizados por estado (activo o inactivo). \\
\hline
\textbf{\textit{Settings}} & Etiqueta que proporciona acceso a las configuraciones de la cuenta del usuario, incluyendo la eliminación de cuentas o cambios en las notificaciones. \\
\hline
\textbf{\textit{Sign Up}} & Etiqueta que guía a los usuarios para crear una cuenta nueva en la aplicación. \\
\hline
\textbf{\textit{Inbox}} & Etiqueta que indica la sección principal donde los correos temporales activos e inactivos son visibles. \\
\hline
\end{longtable}

El diseño de los sistemas de etiquetado en Temporaly facilita la navegación intuitiva y eficiente de los usuarios al emplear una terminología clara y coherente. Las etiquetas como "Sign In" y "Sign Up" guían a los usuarios en el acceso y creación de cuentas, mientras que "New Email" y "Delete Email" permiten una gestión sencilla de correos temporales. La sección "Email History" organiza los correos electrónicos generados, y "Settings" ofrece acceso a configuraciones importantes. Finalmente, "Inbox" proporciona una vista centralizada de los correos temporales activos e inactivos, asegurando una experiencia de usuario fluida y bien estructurada.

\newpage

#### *SEO Tags and Meta Tags*

En la aplicación *Temporaly*, los SEO Tags y Meta Tags juegan un rol crucial en la optimización de la visibilidad de la aplicación en motores de búsqueda y en proporcionar información esencial para su correcto funcionamiento en entornos web. Aunque *Temporaly* es principalmente una aplicación móvil, la landing page y cualquier página relacionada con el servicio puede beneficiarse enormemente del uso correcto de estas etiquetas.

::: box
***SEO Tags***
:::

Los *SEO (Search Engine Optimization) Tags* son utilizados para mejorar el posicionamiento de la landing page de Temporaly en motores de búsqueda como *Google*. Algunos ejemplos de *SEO Tags* utilizados incluyen:

- ***Title Tag:*** Especifica el título de la página que aparece en los resultados de búsqueda.

    ```html
       <title>Temporaly - Protección Temporal de Datos para Estudiantes</title>
    ```

- ***Meta Description:*** Proporciona un breve resumen del contenido de la página para los motores de búsqueda.

    ```html
       <meta name="description" content="Temporaly es una aplicación que permite la creación de correos temporales para proteger tu información personal de forma rápida y segura." />
    ```

- ***Header Tags (H1, H2, H3):*** Estas etiquetas son utilizadas para estructurar el contenido y mejorar la jerarquía de la información en la *landing page*.

    ```html
        <h1>Protege tu Privacidad con Correos Temporales</h1>
    ```

::: box
***Meta Tags***
:::

Los *Meta Tags* son etiquetas que proporcionan información adicional sobre la página web al navegador y a los motores de búsqueda. Estas etiquetas no afectan directamente al contenido visible por los usuarios, pero son esenciales para mejorar la experiencia en la web y optimizar el posicionamiento SEO. Algunos ejemplos de Meta Tags utilizados en Temporaly son:

- ***Charset Meta Tag:*** Define el conjunto de caracteres que la página está utilizando, esencial para evitar errores de visualización.
  
    ```html
       <meta charset="UTF-8">
    ```

- ***Viewport Meta Tag:*** Asegura que la página se vea bien en dispositivos móviles.

    ```html  
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ```

- ***Robots Meta Tag:*** Indica a los motores de búsqueda si deben o no indexar la página.

    ```html  
       <meta name="robots" content="index, follow">
    ```

- ***Canonical Tag:*** Evita contenido duplicado al especificar la URL principal.

    ```html 
        <link rel="canonical" href="https://temporaly.com">
    ```

Además de estas etiquetas clave, para la optimización específica de *Temporaly* como una aplicación móvil, se pueden añadir las siguientes etiquetas, especialmente en la *landing page* para maximizar la visibilidad y facilitar el acceso a la descarga de la app:

***Landing Page SEO Tags (para la aplicación móvil):***

- ***Title:*** *Temporaly* | Protección Temporal de Datos en tu Móvil

- ***Description:*** *Temporaly* - Crea correos temporales directamente desde tu móvil para proteger tu información personal de manera rápida y segura. Disponible para iOS y Android.

- ***Keywords:*** correos temporales, app móvil, protección de datos, privacidad, seguridad, estudiantes.

- ***Author:*** *CodeMinds*

- ***Canonical:*** https://temporaly.com/

***Meta Tags adicionales para la landing page:***

- ***og(Open Graph):*** *Temporaly* | Protección Temporal de Datos

- ***og(Open Graph):*** *Temporaly* te permite crear correos temporales directamente desde tu dispositivo móvil, disponible en las tiendas de apps.

- ***og(Open Graph):*** https://temporaly.com/assets/logo.png

- ***og(Open Graph):*** https://temporaly.com/

- ***app-download-url:***
    * Android: https://play.google.com/store/apps/details?id=com.temporaly
    * iOS: https://apps.apple.com/app/temporaly/id123456789

El uso adecuado de *SEO Tags* y *Meta Tags* garantiza que la *landing page* de *Temporaly* tenga un mayor alcance y visibilidad en los motores de búsqueda, permitiendo a los usuarios encontrar rápidamente la aplicación y acceder a sus servicios. Asimismo, estas etiquetas aseguran una experiencia optimizada para los usuarios que acceden desde dispositivos móviles, facilitando la descarga y el uso de la aplicación.

\newpage

#### *Searching Systems*

El sistema de búsqueda de Temporaly está diseñado para ofrecer una experiencia de usuario eficiente y sencilla, permitiendo a los usuarios acceder rápidamente a la información que necesitan. Dado que Temporaly es una aplicación enfocada en la generación y gestión de correos electrónicos temporales, los mecanismos de búsqueda dentro de la app son clave para la organización y recuperación de la información.


\begin{longtable}{|c|p{9cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{Filtro}} & \multicolumn{1}{c|}{\textbf{Definición}} \\
\hline
\endfirsthead
\textbf{\textit{Email Address}} & Filtro que permite buscar los correos electrónicos temporales generados por dirección de correo. \\
\hline
\textbf{\textit{Creation Date}} & Filtro que permite buscar los correos según la fecha en que fueron generados en la plataforma. \\
\hline
\textbf{\textit{Active/Inactive Status}} & Filtro que permite visualizar los correos según su estado: activos o inactivos. \\
\hline
\textbf{\textit{Duration}} & Filtro que permite buscar correos según el tiempo de validez seleccionado al momento de su creación (10, 30 o 60 minutos). \\
\hline
\textbf{\textit{Advanced Search}} & Opciones avanzadas de búsqueda que permiten combinar múltiples criterios como correo electrónico, estado y duración para obtener resultados más precisos. \\
\hline
\end{longtable}

\vspace{1em}

El sistema de búsqueda en Temporaly ha sido diseñado para optimizar la experiencia del usuario, proporcionando herramientas eficientes para la gestión y recuperación de información relacionada con correos electrónicos temporales. Los filtros como "Email Address" y "Creation Date" permiten a los usuarios localizar correos específicos por dirección o fecha de creación, mientras que el filtro de "Active/Inactive Status" facilita la clasificación según el estado de los correos. "Duration" ofrece la opción de buscar por el tiempo de validez de los correos, y la opción de "Advanced Search" permite una combinación más precisa de criterios, mejorando así la organización y la accesibilidad de la información dentro de la plataforma.

\newpage

#### *Navigation Systems*

El sistema de navegación en Temporaly está diseñado para ser intuitivo y accesible, ofreciendo a los usuarios una experiencia de uso fluida y sin complicaciones. La estructura de navegación asegura que los usuarios puedan desplazarse fácilmente entre las diferentes funcionalidades de la aplicación, optimizando la interacción y minimizando el tiempo de aprendizaje.

\begin{longtable}{|c|p{9cm}|}
\hline
\multicolumn{1}{|c|}{\textbf{Nombre}} & \multicolumn{1}{c|}{\textbf{Definición}} \\
\hline
\endfirsthead
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
\end{longtable}

El sistema de navegación en Temporaly está diseñado para ofrecer una experiencia fluida y accesible. El "Menú Lateral" facilita el acceso a secciones principales como Home, Contact Us, About Us, Terms and Conditions, y Settings, permitiendo una navegación eficiente. La "Barra de Navegación Inferior" proporciona acceso directo a funciones clave como Email y History, mejorando la accesibilidad a las características más utilizadas. La sección "Email" actúa como la vista principal para gestionar correos temporales, mientras que "History" organiza el historial de correos según su estado. Finalmente, "Settings" permite ajustar configuraciones de la cuenta, como notificaciones y opciones de cierre de sesión.

\newpage

### *Landing Page UI Design*

![Imagen extraída de Canva](src/img/Cap3/landingpageui.png)

En esta sección, abordaremos los aspectos clave del diseño de interfaces para landing pages. Nos centraremos en técnicas efectivas para estructurar contenido, optimizar elementos visuales y mejorar la experiencia del usuario con el objetivo de maximizar la conversión. Analizaremos enfoques prácticos y estrategias para crear landing pages impactantes y funcionales.

#### *Landing Page Wireframe*

::: warn
Para acceder al los Wireframes de trabajo, haga click a la [URL](https://www.figma.com/design/ofFIiA94N3qwhXABKh0Yie/Landing-App-movil?node-id=0-1&t=ZeaTDjPO2hi8tUPQ-1)
:::

\newpage

***Web Landing Page Wireframe***

![Hero Wireframe, Artefacto creado en Figma](src/img/Cap3/landing1.png)

![Features Wireframe, Artefacto creado en Figma](src/img/Cap3/landing2.png)

![Features Wireframe, Artefacto creado en Figma](src/img/Cap3/landing3.png)

![App Wireframes, Artefacto creado en Figma](src/img/Cap3/landing4.png)

![Testimonials Wireframe, Artefacto creado en Figma](src/img/Cap3/landing5.png)

![Pricing Wireframe, Artefacto creado en Figma](src/img/Cap3/landing6.png)

![Contact us Wireframe, Artefacto creado en Figma](src/img/Cap3/landing7.png)

![Contact us Wireframe, Artefacto creado en Figma](src/img/Cap3/landing8.png)

\newpage

***Mobile Landing Page Wireframe***

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap3/mob1.png}
    \caption{Hero Wireframe, Artefacto creado en Figma}
    \label{fig:hwacf1}
\end{figure}

![Features Wireframe, Artefacto creado en Figma](src/img/Cap3/mob2.png)

![Features Wireframe, Artefacto creado en Figma](src/img/Cap3/mob3.png)

![App Wireframes, Artefacto creado en Figma](src/img/Cap3/mob4.png)

![Testimonials Wireframe, Artefacto creado en Figma](src/img/Cap3/mob5.png)

![Pricing Wireframe, Artefacto creado en Figma](src/img/Cap3/mob6.png)

![Contact us Wireframe, Artefacto creado en Figma](src/img/Cap3/mob7.png)

![Contact us Wireframe, Artefacto creado en Figma](src/img/Cap3/mob8.png)

\newpage

#### *Landing Page Mock-up*

***Web Landing Page Mock-up***

![Hero Mockup, Artefacto creado en Figma](src/img/Cap3/lan1.png)

![Features Mockup, Artefacto creado en Figma](src/img/Cap3/lan2.png)

![Features Mockup, Artefacto creado en Figma](src/img/Cap3/lan3.png)

![App Mockup, Artefacto creado en Figma](src/img/Cap3/lan4.png)

![Testimonials Mockup, Artefacto creado en Figma](src/img/Cap3/lan5.png)

![Pricing Mockup, Artefacto creado en Figma](src/img/Cap3/lan6.png)

![Contact Us Mockup, Artefacto creado en Figma](src/img/Cap3/lan7.png)

![Contact Us Mockup, Artefacto creado en Figma](src/img/Cap3/lan8.png)

\newpage

***Mobile Landing Page Mock-up***

\begin{figure}[h!]
    \centering
    \includegraphics[width=1.0\textwidth, height=0.9\textheight]{src/img/Cap3/mobc1.png}
    \caption{Hero Mockup, Artefacto creado en Figma}
    \label{fig:hmacf1}
\end{figure}

![Features Mockup, Artefacto creado en Figma](src/img/Cap3/mobc2.png)

![Features Mockup, Artefacto creado en Figma](src/img/Cap3/mobc3.png)

![App Mockup, Artefacto creado en Figma](src/img/Cap3/mobc4.png)

![Testimonials Mockup, Artefacto creado en Figma](src/img/Cap3/mobc5.png)

![Pricing Mockup, Artefacto creado en Figma](src/img/Cap3/mobc6.png)

![Contact Us Mockup, Artefacto creado en Figma](src/img/Cap3/mobc7.png)

![Contact Us Mockup, Artefacto creado en Figma](src/img/Cap3/mobc8.png)

\newpage

***Mockup concepts:***

![Mockup concepts, Artefacto creado en canva](src/img/Cap3/Mockup_concepts.png)

\newpage

### *Mobile Application UX/UI Design*

![Recurso estraído de Canva](src/img/Cap3/mobiledesign.png)

En esta sección, exploraremos los aspectos clave del diseño de interfaces para aplicaciones móviles. Nos enfocaremos en técnicas efectivas para estructurar el contenido, optimizar los elementos visuales y mejorar la experiencia del usuario con el objetivo de maximizar la usabilidad. Analizaremos enfoques prácticos y estrategias para crear interfaces móviles atractivas y funcionales, adaptadas a las necesidades y comportamientos de los usuarios en dispositivos móviles.

::: warn
Para visualizar todo el diseño de los wireframes y mockups de la aplicación, haga click en la [URL](https://www.figma.com/design/3q2f24bDIbpzV5Xfnyw3cY/Temporaly?node-id=0-1&t=ADyy9ooMf3OcFAjA-1)
:::

\newpage

#### *Mobile Application Wireframes*

\begin{figure}[h!]
    \centering
    \includegraphics[height=0.4\textheight]{src/img/Cap3/wireframes/Frame246.png}
    \caption{SplashScreen Wireframe - Artefacto creado en Figma}
    \label{fig:maw1}
\end{figure}

\begin{figure}[h!]
    \centering
    \includegraphics[height=0.4\textheight]{src/img/Cap3/wireframes/Frame247.png}
    \caption{Biometric Access Wireframe - Artefacto creado en Figma}
    \label{fig:maw2}
\end{figure}

![Access via Google account Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame260.png)

![Sign Up Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame261.png)

![Sign Up Verification Code Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame262.png)

![Main Screen Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame248.png)

![Toolbar of Main Screen Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame252.png)

![Privacy and Policies Button Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame253.png)

![About Us redirection to Landing page Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame254.png)

![Privacy and Policies Screen Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame255.png)

![Settings Screen Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame256.png)

![Profile Settings Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame257.png)

![Close Account Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame258.png)

![Delete Account Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame259.png)

![History Temporary Email Screen Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame249.png)

![Temporary Email Inbox History Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame250.png)

![Email Details Wireframe - Artefacto creado en Figma](src/img/Cap3/wireframes/Frame251.png)

\newpage

#### *Mobile Applications Wireflow Diagrams*

![SplashScreen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame212.png)

![Biometric Access Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame213.png)

![Access via Google account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame214.png)

![Sign Up Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame215.png)

![Sign Up Verification Code Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame216.png)

![Main Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame217.png)

![Toolbar of Main Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame218.png)

![Privacy and Policies Button Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame219.png)

![About Us redirection to Landing page Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame220.png)

![Privacy and Policies Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame221.png)

![Settings Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame222.png)

![Profile Settings Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame223.png)

![Close Account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame224.png)

![Delete Account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame225.png)

![History Temporary Email Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame226.png)

![Temporary Email Inbox History Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame227.png)

![Email Details Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-wireframes/Frame228.png)

\newpage

#### *Mobile Applications Mock-Ups*

![SplashScreen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame263.png)

![Biometric Access Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame264.png)

![Access via Google account Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame277.png)

![Sign Up Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame278.png)

![Sign Up Verification Code Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame279.png)

![Main Screen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame265.png)

![Toolbar of Main Screen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame269.png)

![Privacy and Policies Button Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame270.png)

![About Us redirection to Landing page Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame271.png)

![Privacy and Policies Screen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame272.png)

![Settings Screen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame273.png)

![Profile Settings Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame274.png)

![Close Account Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame275.png)

![Delete Account Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame276.png)

![History Temporary Email Screen Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame266.png)

![Temporary Email Inbox History Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame267.png)

![Email Details Mockup - Artefacto creado en Figma](src/img/Cap3/mockups/Frame268.png)

\newpage

#### *Mobile Applications User Flow Diagrams*

![SplashScreen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame229.png)

![Biometric Access Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame230.png)

![Access via Google account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame243.png)

![Sign Up Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame244.png)

![Sign Up Verification Code Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame245.png)

![Main Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame231.png)

![Toolbar of Main Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame235.png)

![Privacy and Policies Button Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame236.png)

![About Us redirection to Landing page Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame237.png)

![Privacy and Policies Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame238.png)

![Settings Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame239.png)

![Profile Settings Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame240.png)

![Close Account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame241.png)

![Delete Account Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame242.png)

![History Temporary Email Screen Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame232.png)

![Temporary Email Inbox History Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame233.png)

![Email Details Wireflow - Artefacto creado en Figma](src/img/Cap3/wireflows-mockups/Frame234.png)

#### *Mobile Applications Prototyping*

::: warn
Para visualizar el video del prototipo de la aplicación,  haga click en la [URL](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210059_upc_edu_pe/EaarYyGV9fFJpLWK1u04GaIBtRlSoc7_affoLtT38NNzEQ?e=krmvNP&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
:::

\newpage

### *Domain-Driven Software Architecture*

![Imagen extraída de Canva](src/img/Cap3/dddimage.png)

En el desarrollo de *software*, la arquitectura impulsada por el dominio (*Domain-Driven Software Architecture*) se ha convertido en un enfoque esencial para crear soluciones robustas, escalables y alineadas con los objetivos del negocio. 

\begin{quote}
Este enfoque, popularizado por Eric Evans en su libro "*Domain-Driven Design*", se centra en modelar el *software* en torno a los conceptos y procesos que son fundamentales para el dominio del negocio.
\end{quote}

El corazón de la arquitectura impulsada por el dominio reside en su capacidad para reflejar de manera fiel las complejidades y las reglas del negocio en la estructura del sistema. En lugar de desarrollar soluciones tecnológicas genéricas, esta metodología fomenta una colaboración estrecha entre los expertos del dominio (aquellos con profundo conocimiento de los problemas del negocio) y los equipos de desarrollo, asegurando que el diseño del *software* esté íntimamente alineado con las necesidades reales de la organización.
Al adoptar un enfoque centrado en el dominio, se mejora la mantenibilidad del sistema, permitiendo a los equipos de desarrollo reaccionar rápidamente ante los cambios en los requerimientos de negocio, y favoreciendo una evolución constante del *software* sin comprometer la calidad. A medida que las organizaciones se enfrentan a entornos cambiantes y crecientes demandas de escalabilidad, la arquitectura impulsada por el dominio se presenta como una estrategia clave para el éxito a largo plazo de las soluciones tecnológicas.

\newpage

#### *Software Architecture Context Level Diagram*

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Contexto.png)

#### *Software Architecture Container Level Diagram*

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Contenedores.png)

#### *Software Architecture Components Diagram*

![Artefacto creado en Structurizr](src/img/Cap3/Diagrama_Componentes.png)

### *Software Object-Oriented Design*

![Imagen extraída de Canva](src/img/Cap3/soodesign.png)

El diseño orientado a objetos (OOD) es un enfoque clave en la ingeniería de software que se basa en la creación de sistemas mediante la conceptualización del mundo real a través de "objetos". Estos objetos son entidades que encapsulan tanto datos como comportamiento, facilitando la creación de software más modular, mantenible y escalable. A través de principios fundamentales como la encapsulación, la herencia y el polimorfismo, el diseño orientado a objetos permite la construcción de soluciones más flexibles y reutilizables. Este enfoque ha demostrado ser efectivo en la gestión de la complejidad en sistemas grandes y distribuidos, promoviendo un desarrollo más eficiente y alineado con las necesidades del negocio.

#### *Class Diagrams*
Nuestro dominio se divide en 4 Bounded Contexts:

1.- ***Login Bounded Context***: Centrado en los actores/usuarios que se autentican en la solución y la gestión del proceso de login y logout.

2.- ***Profile Settings Bounded Context***: Centrado en los cambios de configuración del perfil de los usuarios, incluyendo preferencias, ajustes y personalización.

3.- ***Privacy Policy Bounded Context***: Centrado en la gestión de las políticas de privacidad y la obtención o revocación de consentimiento por parte de los usuarios.

4.- ***Email History Management Bounded Context***: Centrado en el registro y seguimiento del historial de acciones de correo electrónico realizadas por el sistema y los usuarios.

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/iam_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/email_management_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/profile_settings_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/privacy_policy_bc.jpeg)

![Class diagram Temporaly, imagen creada en PlantUML](src/img/Cap3/email_history_bc.jpeg)

\newpage

#### *Class Dictionary*

##### *Email History Management Bounded Context*

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

#####  *Email Management Bounded Context*

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

##### *Login Bounded Context (Identity and Access Management)*

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

##### *Privacy Policy Bounded Context*

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


##### *Profile Settings Bounded Context*

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


#### *Database Design*

![Class diagram Temporaly, imagen creada en Mermaid](src/img/Cap3/database_desing.png)

#### *Database Diagram*

![Class diagram Temporaly, imagen creada en Mermaid](src/img/Cap3/database_diagram.png)

\newpage

# Capítulo IV: *Backend Configuration Management*

## *Software Configuration Management*

![Imagen extraída de Canva](src/img/Cap4/backendintro.png)

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

::: warn
Para acceder al flujo del *backend*, haga click a la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Temporaly-Backend)
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

::: warn
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

\begin{longtable}{|p{5cm}|p{9cm}|}
\hline
\textbf{Sprint Planning Background} & \\ \hline
\endfirsthead
\hline
\textbf{Sprint} & \textbf{Sprint 1} \\ \hline
\endfoot
\hline
\textbf{Date} & 15/09/2024 \\ \hline
\textbf{Time} & 21:00 \\ \hline
\textbf{Location} & Discord Virtual Meeting \\ \hline
\textbf{Prepared By} & Ortega Huaraca, Abel Angel \\ \hline
\textbf{Attendees (to planning meeting)} & Ortega Huaraca, Abel Angel / Avila Asto, Alex Ramon / Vilchez Rios, Mateo Alejandro / Ramos Rios, Belen del Rocio \\ \hline
\textbf{Sprint 1 Review Summary} & Implementación de los segmentos de investigación (Cap 1 y 2), Requirements Specification y primer Sprint de implementación \\ \hline
\textbf{Sprint 1 Retrospective Summary} & El trabajo se realizó a tiempo, y cada integrante terminó lo que se le encomendó. Asimismo, se trabajó en equipo cuando la situación del proyecto lo requería. \\ \hline
\textbf{Sprint Goal \& User Stories} & Implementar la landing page, avanzar una parte del backend de la aplicación y definir las tecnologías a emplear \\ \hline
\textbf{Sprint 1 Velocity} & 1 Sprint cada 2 semanas \\ \hline
\textbf{Sum of Story Points} & 93 \\ \hline
\end{longtable}

\newpage

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

\newpage

**Gestión del Sprint 1 (Tablero Kanban):**

Para mejorar la gestión y seguimiento de las tareas de este *sprint*, se implementó un tablero Kanban. Este tablero permite visualizar claramente los elementos clave a desarrollar, asignar responsables para cada tarea, y utilizar etiquetas *(labels)* que categorizan los Issues de forma precisa. Además, los *Milestones* fueron utilizados estratégicamente para planificar las fechas de entrega y gestionar los entregables, facilitando un control eficiente del progreso del proyecto.

![Tablero Kanban del equipo, imagen extraída de Github](src/img/Cap4/Sprint_Backlog1.png)

\newpage

#### *Development Evidence for Sprint Review*

Evidencia de colaboración en Equipo:

![Imagen extraída de Github](src/img/cap5/development-evidence.png)

\newpage

#### *Testing Suite Evidence for Sprint Review*

***Landing Page US - Gherkin***

```gherkin
US38 - Descubrimiento intuitivo

Feature: Descubrimiento intuitivo
  As a user
  I want to easily discover the main sections of the landing page
  So that I can navigate it intuitively

  Scenario: Successful navigation on landing page
    Given the user is on the landing page
    When they interact with the main navigation bar
    Then they should see links to the main sections of the website
    And the navigation should work smoothly
    
    Examples:
      | User action     | Expected result         |
      | Click "Home"    | Navigates to homepage   |
      | Click "Features"| Navigates to features   |
      | Click "About"   | Navigates to about page |

  Scenario: Responsive design adapts to screen size
    Given the user is accessing the landing page from a mobile device
    When they view the page
    Then the layout should adjust to fit the screen size appropriately
    And all sections should be accessible

    Examples:
      | Device      | Expected behavior                              |
      | Smartphone  | Layout adjusts, elements stack vertically      |
      | Tablet      | Layout adjusts, elements fit wider screen      |
```

```gherkin

US39 - Contenido informativo

Feature: Contenido informativo
  As a visitor
  I want to find clear and informative content on the landing page
  So that I can learn more about the application's features

  Scenario: Display clear content on application features
    Given the user is on the landing page
    When they scroll down to the information section
    Then they should see a clear explanation of the application's main features
    And the text should be easy to read and understand
    
    Examples:
      | Section        | Content                                             |
      | Features       | Explanation of core app functionalities             |
      | Benefits       | Description of the advantages for users             |
      | Testimonials   | Positive feedback from current users                |

  Scenario: Ensure content is displayed correctly across devices
    Given the user is on the landing page on a mobile device
    When they scroll through the information section
    Then the content should remain responsive and clear
    And images should load correctly
    
    Examples:
      | Device        | Expected result                            |
      | Mobile        | Text adjusts, images scale down            |
      | Desktop       | Text and images adjust to full-screen size |

```

```gherkin

US40 - Compatibilidad móvil

Feature: Compatibilidad móvil
  As a visitor
  I want to browse the landing page on my mobile device
  So that I can easily access it from any device

  Scenario: Responsive design for mobile devices
    Given the user accesses the landing page on a smartphone
    When they scroll through the content
    Then the page should display correctly without layout issues
    And images should be scaled appropriately

    Examples:
      | Device      | Expected behavior                                   |
      | iPhone 12   | Responsive, no text overlaps, easy to navigate      |
      | Galaxy S21  | All buttons are accessible, images fit screen size  |

  Scenario: Test page responsiveness for tablets and desktops
    Given the user accesses the page on a tablet or desktop
    When they resize the browser window
    Then the layout and content should adjust fluidly without breaking

    Examples:
      | Device      | Expected behavior                                   |
      | iPad        | Two-column layout, images scale appropriately       |
      | Desktop     | Three-column layout, full image resolution          |

```

```gherkin

US41 - Formulario de contacto

Feature: Formulario de contacto
  As a visitor
  I want to fill out the contact form on the landing page
  So that I can get in touch with the application team

  Scenario: Successful form submission
    Given the user is on the contact form page
    When they fill in all required fields and submit the form
    Then the system should display a confirmation message that the form has been successfully submitted
    And the submitted details should be sent to the application team

    Examples:
      | Name        | Email              | Message                 | Status        |
      | John Doe    | john@example.com   | Inquiry about services  | Submitted     |
      | Jane Smith  | jane@example.com   | Question about pricing  | Submitted     |

  Scenario: Missing required fields
    Given the user is filling out the contact form
    When they leave required fields empty
    Then the system should display an error message asking them to complete the missing fields
    
    Examples:
      | Name        | Email              | Message                 | Error message           |
      | John Doe    |                    | Inquiry about services  | "Email is required"     |
      |             | jane@example.com   |                         | "Name is required"      |

```

```gherkin

US42 - Contenido multimedia

Feature: Contenido multimedia
  As a visitor
  I want to find multimedia content on the landing page
  So that I can learn about the app features in a dynamic way

  Scenario: Display multimedia content successfully
    Given the user is on the landing page
    When they scroll through the multimedia section
    Then they should see images, videos, and icons that explain the app's functionality
    And the multimedia content should load quickly and properly

    Examples:
      | Media Type | Expected Behavior                              |
      | Images     | Display correctly, optimized for loading speed |
      | Videos     | Play smoothly, no buffering                    |
      | Icons      | Scale appropriately without distortion         |

  Scenario: Ensure multimedia content is responsive across devices
    Given the user accesses the landing page from different devices
    When they view the multimedia section
    Then the multimedia content should adjust to fit the screen size and resolution without losing quality

    Examples:
      | Device       | Expected Behavior                                   |
      | Mobile       | Images and videos scale down, responsive layout     |
      | Tablet       | Images and videos adapt to a medium screen layout   |
      | Desktop      | Full resolution, multimedia fills the space         |

```

```gherkin

US43 - Call-to-action claro

Feature: Call-to-action claro
  As a visitor
  I want to find clear call-to-action (CTA) buttons on the landing page
  So that I can take immediate action (e.g., request a demo)

  Scenario: Clear CTA buttons guide user actions
    Given the user is on the landing page
    When they see the "Request Demo" or "Sign Up" buttons
    Then the buttons should be visually prominent and lead to the correct sections of the website

    Examples:
      | CTA Text      | Expected Behavior                            |
      | Request Demo  | Redirects user to contact form               |
      | Sign Up       | Redirects user to registration page          |

  Scenario: CTA buttons work across devices
    Given the user accesses the landing page from different devices
    When they interact with CTA buttons
    Then the buttons should be responsive and work correctly on all screen sizes

    Examples:
      | Device       | Expected Behavior                            |
      | Mobile       | Buttons are visible and clickable             |
      | Tablet       | Buttons scale correctly, remain interactive   |
      | Desktop      | Full-size buttons, clear, and functional      |

```

***Backend US - Gherkin***

```gherkin

US32 - RESTful API Registro de usuario

Feature: Registro de usuario a través de la API RESTful
  As a developer
  I want to implement an API for user registration
  So that users can create an account in the application

  Scenario: Successful user registration
    Given the user has provided a valid email and password
    When the user submits a POST request to "/api/v1/users"
    Then the system should create a new user
    And respond with status 201 and user information

  Scenario: Failed registration due to duplicate email
    Given a user already exists with the provided email
    When the user submits a POST request to "/api/v1/users"
    Then the system should respond with status 400
    And return a message indicating email is already in use

Examples:
  | email             | password    |
  | existing@example.com | password123 |
  | newuser@example.com  | password456 |

```

```gherkin

US33 - RESTful API Inicio de sesión de usuario

Feature: User login through RESTful API
  As a developer
  I want to implement a login API
  So that users can securely log in to their accounts

  Scenario: Successful login
    Given the user exists with valid credentials
    When the user submits a POST request to "/api/v1/login"
    Then the system should authenticate the user
    And respond with status 200 and a JWT token

  Scenario: Failed login due to incorrect password
    Given the user exists with an incorrect password
    When the user submits a POST request to "/api/v1/login"
    Then the system should respond with status 401
    And return a message indicating invalid credentials

Examples:
  | email             | password    |
  | user@example.com  | correctpass |
  | user@example.com  | wrongpass   |

```

```gherkin

US34 - Autenticación basada en token JWT

Feature: JWT-based authentication for the API
  As a developer
  I want to implement JWT authentication
  So that I can secure API endpoints

  Scenario: Successful authentication with JWT
    Given the user is logged in with a valid JWT token
    When the user requests a protected resource "/api/v1/protected"
    Then the system should respond with status 200 and the resource

  Scenario: Failed authentication due to expired token
    Given the user has an expired JWT token
    When the user requests a protected resource "/api/v1/protected"
    Then the system should respond with status 401 and a message "Token expired"

Examples:
  | token_status | response |
  | valid        | 200      |
  | expired      | 401      |

```

```gherkin

US35 - Recuperación de contraseña

Feature: Password recovery via RESTful API
  As a developer
  I want to implement a password recovery API
  So that users can reset their forgotten passwords

  Scenario: Successful password recovery request
    Given the user has provided a valid email
    When the user submits a POST request to "/api/v1/password-recovery"
    Then the system should send a password reset link to the email
    And respond with status 200

  Scenario: Failed password recovery due to invalid email
    Given the user has provided an invalid email
    When the user submits a POST request to "/api/v1/password-recovery"
    Then the system should respond with status 404 and a message "User not found"

Examples:
  | email              |
  | valid@example.com  |
  | invalid@example.com|

```

```gherkin

US36 - RESTful API Creación de sesiones

Feature: Session creation through RESTful API
  As a developer
  I want to implement an API for session management
  So that users can create multiple sessions

  Scenario: Successful session creation
    Given the user has valid credentials
    When the user submits a POST request to "/api/v1/sessions"
    Then the system should create a new session
    And respond with status 201 and session details

  Scenario: Failed session creation due to missing data
    Given the user has not provided all necessary data
    When the user submits a POST request to "/api/v1/sessions"
    Then the system should respond with status 400 and an error message

Examples:
  | email              | session_id |
  | user@example.com    | session123 |
  | incomplete@example.com | N/A     |

```

```gherkin

US37 - Paginación y filtrado de resultados

Feature: Pagination and filtering of API results
  As a developer
  I want to implement pagination and filtering on the API
  So that users can retrieve data efficiently

  Scenario: Retrieve paginated results
    Given there are more than 10 users in the system
    When the user requests page 2 with 10 results per page
    Then the system should return 10 users from page 2
    And respond with status 200

  Scenario: Retrieve filtered results by role
    Given there are users with different roles
    When the user requests a filtered list of users by role "admin"
    Then the system should return only users with the "admin" role

Examples:
  | page | results_per_page | role   |
  | 2    | 10               | admin |
  | 1    | 5                | user  |

```

***Frontend US - Gherking***

```gherkin

US01 - Registro de usuario

Feature: Registro de usuario en la aplicación
  As a user
  I want to register by providing my email and password
  So that I can create an account in the application

  Scenario: Successful user registration
    Given the user has entered a valid email and password
    When the user submits the registration form
    Then the system should create a new user account
    And send a confirmation email to the user

  Scenario: Failed registration due to missing information
    Given the user has not entered an email or password
    When the user submits the registration form
    Then the system should display an error message "Email and password are required"

Examples:
  | email             | password    |
  | newuser1@example.com | pass12345 |
  |                   | pass12345   |

```

```gherkin

US02 - Confirmación de creación de cuenta

Feature: Confirmación de creación de cuenta
  As a user
  I want to receive a confirmation email after registering
  So that I know my account has been created

  Scenario: Successful confirmation email sent
    Given the user has registered successfully
    When the system sends a confirmation email
    Then the user should receive the email in their inbox
    And the email should contain a link to verify the account

  Scenario: Failed to send confirmation email
    Given the system is experiencing technical issues
    When the system tries to send the confirmation email
    Then the system should log an error
    And notify the user that the confirmation email could not be sent

Examples:
  | email             |
  | user@example.com  |
  | another@example.com |

```

```gherkin

US03 - Verificación de cuenta

Feature: Verificación de cuenta mediante correo electrónico
  As a user
  I want to verify my account using the link sent to my email
  So that I can activate my account

  Scenario: Successful account verification
    Given the user has received the confirmation email
    When the user clicks on the verification link
    Then the system should mark the account as verified
    And the user should be redirected to the login page

  Scenario: Failed verification due to invalid link
    Given the user has clicked on an expired or invalid verification link
    When the user tries to verify their account
    Then the system should display an error message "Verification link is invalid or expired"

Examples:
  | verification_status |
  | valid               |
  | invalid             |

```

```gherkin

US04 - Inicio de sesión de cuenta

Feature: Inicio de sesión de usuario
  As a user
  I want to log in using my email and password
  So that I can access my account

  Scenario: Successful login
    Given the user has entered the correct email and password
    When the user submits the login form
    Then the system should log the user in
    And redirect the user to the dashboard

  Scenario: Failed login due to incorrect password
    Given the user has entered an incorrect password
    When the user submits the login form
    Then the system should display an error message "Incorrect password"

Examples:
  | email             | password    |
  | user1@example.com | correctpass |
  | user1@example.com | wrongpass   |

```

```gherkin

US05 - Generación de correo temporal con un click

Feature: Generación de correo temporal
  As a user
  I want to generate a temporary email with one click
  So that I can use it for quick registrations on other websites

  Scenario: Generate temporary email successfully
    Given the user is on the temporary email generation page
    When the user clicks the "Generate Email" button
    Then the system should create a temporary email
    And display the email address to the user

Examples:
  | email               |
  | temp1@example.com   |
  | temp2@example.com   |

```

```gherkin

US06 - Duración específica del correo temporal

Feature: Especificar la duración de correos temporales  

  As a user  
  I want to specify the duration of my temporary email  
  So that the email expires after a set period 

  Scenario: Set a custom expiration time    
  Given the user is creating a temporary email    
  When the user selects a duration of 30 minutes    
  Then the system should set the expiration time to 30 minutes.

  Examples:  
  | duration | 
  | 10 min   |  
  | 30 min   |

```

```gherkin

Feature: Confirmación visual de creación de correo temporal

  As a user
  I want a visual confirmation when my temporary email is created
  So that I know the email is ready to use

  Scenario: Show visual confirmation after email creation
    Given the user has generated a temporary email
    When the email is created
    Then the system should display a confirmation message "Email created successfully"

  Examples:
  | confirmation_status |
  | success             |

```

```gherkin

US08 - Personalización del dominio del correo temporal

Feature: Personalización del dominio del correo temporal

  As a user
  I want to customize the domain of my temporary email
  So that I can choose from different domain options

  Scenario: User selects a custom domain for temporary email
    Given the user is creating a temporary email
    When the user selects a domain from the dropdown
    Then the system should generate the email with the chosen domain

  Examples:
  | domain        |
  | @tempmail.com |
  | @quickmail.io |

```

```gherkin

US09 - Generación múltiple de correos temporales

Feature: Generación múltiple de correos temporales
  As a user
  I want to generate multiple temporary emails in one session
  So that I can use different emails for various registrations

  Scenario: Generate multiple temporary emails
    Given the user is on the email generation page
    When the user requests 3 temporary emails
    Then the system should create and display 3 unique temporary emails

Examples:
  | email_count |
  | 3           |
  | 5           |

```

```gherkin

US10 - Copiar correo temporal al portapapeles

Feature: Copiar correo temporal al portapapeles
  As a user
  I want to copy my generated temporary email to the clipboard
  So that I can paste it easily on other websites

  Scenario: Copy email to clipboard
    Given the user has generated a temporary email
    When the user clicks the "Copy" button
    Then the system should copy the email to the clipboard
    And display a message "Email copied to clipboard"

Examples:
  | email               |
  | temp1@example.com   |
  | temp2@example.com   |

```

```gherkin

US11 - Visualización de correos temporales activos

Feature: Visualización de correos temporales activos
  As a user
  I want to see all my active temporary emails
  So that I can manage them effectively

  Scenario: Display list of active temporary emails
    Given the user has generated multiple temporary emails
    When the user navigates to the active emails page
    Then the system should display a list of active emails

Examples:
  | email_count |
  | 2           |
  | 5           |

```

```gherkin

US12 - Sugerencias automáticas de nombres para correos

Feature: Sugerencias automáticas de nombres para correos temporales
  As a user
  I want the system to suggest email names automatically
  So that I can quickly choose a temporary email name

  Scenario: System provides email name suggestions
    Given the user is generating a temporary email
    When the user clicks on the suggestion box
    Then the system should display a list of suggested email names

Examples:
  | suggestion_count |
  | 3                |
  | 5                |

```

```gherkin

US13 - Proceso de generación rápido y fluido

Feature: Proceso de generación rápido y fluido
  As a user
  I want the temporary email generation process to be fast and smooth
  So that I can generate emails without delays

  Scenario: Generate temporary email in less than 5 seconds
    Given the user is on the temporary email page
    When the user clicks "Generate Email"
    Then the system should create the email within 5 seconds

Examples:
  | generation_time |
  | 3 seconds       |
  | 4.5 seconds     |

```

```gherkin

US14 - Advertencia de expiración de correo temporal

Feature: Advertencia de expiración de correo temporal
  As a user
  I want to be notified when my temporary email is about to expire
  So that I can take necessary actions before it expires

  Scenario: Notify user before email expiration
    Given the user has an active temporary email
    When the email is 5 minutes away from expiration
    Then the system should display a warning message "Email is about to expire"

Examples:
  | warning_time |
  | 5 minutes    |
  | 10 minutes   |

```

```gherkin

US15 - Acceso a bandeja de entrada de correos temporales

Feature: Acceso a bandeja de entrada de correos temporales
  As a user
  I want to access a specific inbox for my temporary emails
  So that I can view and manage the emails received without mixing them with my personal emails

  Scenario: User accesses the inbox for temporary emails
    Given the user has generated one or more temporary emails
    When the user navigates to the "Temporary Inbox" section
    Then the system should display a list of received temporary emails in the inbox

  Scenario: No temporary emails in the inbox
    Given the user has not generated or received any temporary emails
    When the user navigates to the "Temporary Inbox" section
    Then the system should display a message "No emails received"

  Scenario: User opens a specific email from the inbox
    Given the user has received temporary emails
    When the user selects a specific email from the list
    Then the system should display the full content of the selected email

Examples:
  | email_count | email_subject           | sender                | received_date |
  | 5           | "Welcome to TempMail"   | welcome@tempmail.com  | 2024-09-10    |
  | 0           |                         |                       |               |
  | 3           | "Verify your account"   | no-reply@webservice.io| 2024-09-09    |

```

```gherkin

US16 - Visualización de correos recibidos

Feature: Visualización de correos recibidos en la bandeja de entrada
  As a user
  I want to view a list of emails I have received in my temporary inbox
  So that I can manage important messages

  Scenario: Display list of received emails
    Given the user has received emails in the temporary inbox
    When the user opens the inbox
    Then the system should show a list of received emails with subject, sender, and date

  Scenario: View details of a received email
    Given the user is viewing the list of received emails
    When the user selects a specific email
    Then the system should display the full content of the selected email

Examples:
  | email_subject           | sender           | date         |
  | "Welcome"               | welcome@site.com | 2024-09-10   |
  | "Confirm your account"  | no-reply@site.io | 2024-09-11   |

```

\newpage

#### *Execution Evidence for Spring Review*
Durante este primer sprint se realizó la implementación de la landing page, incluyendo las siguientes features:

* Se implementó un menú superior que permite un acceso rápido a las diferentes secciones de la página.
* Cada sección de la landing page tiene partes funcionales según las características deseadas para cada una.

Además, se implementó el backend con gestión de usuarios a través de IAM (Identity and Access Management), integrando OAuth para la autenticación y autorización segura.

En las imágenes y videos adjuntos se podrá apreciar de mejor manera los avances mencionados.

**Implementación de la Landing Page**

![Landing Page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_1.png)

![Landing Page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_2.png)

![Landing Page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_3.png)

\newpage

**Implementación del Backend**

![Landing Page: Imagen extraída del navegador](src/img/Cap4/cap4_backend_1.png)

\newpage

#### *Services Documentation Evidence for Sprint Review*

En esta seccion, se muestra la documentacion de los servicios del back end de la aplicación móvil, asi como tambien se muestra el uso de Swagger para la documentacion de los servicios.

Utilizamos *SpringBoot*, *Spring Security*, *Spring Mongo*, *Spring Oauthclient*, *JWToken* y *Spring Data*

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

\newpage

#### *Software Deployment Evidence for Sprint Review*

***Landing Page deployment***

::: warn
Para visualizar la Landing Page, haga click en la [URL](https://temporaly.netlify.app/) o copie y pegue el link https://temporaly.netlify.app/
:::

![Landing page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_deploy_1.jpeg)

![Landing page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_deploy_2.jpeg)

![Landing page: Imagen extraída del navegador](src/img/Cap4/cap4_landing_deploy_3.jpeg)

\newpage

***Backend deployment***

::: warn
Para visualizar el backend, haga click en la [URL](https://temporally-api.ryzeon.me/documentation) o copie y pegue el link https://temporally-api.ryzeon.me/documentation 
:::

![Backend: Imagen extraída del IDEA](src/img/Cap4/cap4_backend_deploy_1.png)

![Backend: Imagen extraída del IDEA](src/img/Cap4/cap4_backend_deploy_2.png)

![Backend: Imagen extraída del IDEA](src/img/Cap4/cap4_backend_deploy_3.png)

![Backend: Imagen extraída del navegador](src/img/Cap4/cap4_backend_deploy_4.png)

\newpage

#### *Team Collaboration Insights During Sprint*

::: warn
Para acceder a la visualización del flujo del trabajo, haba click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1/views/2)
:::

![Imagen extraída de Github](src/img/Cap4/colaboracion.png)

\newpage

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

\newpage

# Bibliografía
