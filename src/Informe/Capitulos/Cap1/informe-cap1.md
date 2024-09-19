---
title: "Universidad Peruana de Ciencias Aplicadas - Informe de Trabajo Final"
author: 
  - "Startup: CodeMinds"
  - "Producto: Temporaly"
  - "Profesor: Mayta Guillermo, Jorge Luis"
  - "Integrantes:"
  - "Ortega Huaraca, Abel Angel - U20201B380"
  - "Avila Asto, Alex Ramon - u20221a322"
  - "Vilchez Rios, Mateo Alejandro - u202210059"
  - "Ramos Rios, Belén del Rocio - u202216246"

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
  \usepackage{longtable}
  \usepackage{array}
  \usepackage{lscape}
  \usepackage{float} 
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

*Actividades Colaborativas* ***(Github Kanban)***

::: warn
Para mayor información, haga click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

**TB1:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-2.png)

**TB2:**

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-3.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-4.png)

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
