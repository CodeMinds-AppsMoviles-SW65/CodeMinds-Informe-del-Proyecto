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
  tb2 & 15/09/2024 & Ortega Huaraca, Abel Angel & falta completar \\
  \hline
  tb2 & 15/09/2024 & Avila Asto, Alex Ramon Alberto & falta completar \\
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
Coordiné y realicé la reunión inicial del proyecto, explicando claramente los objetivos y el plan de trabajo. Cree diferentes reuniones para clarificar los roles de cada integrante del equipo y organicé los flujos de trabajas de un tablero Kanban (Scrum). Respecto al informe, culminé en tiempo y forma las pendientes que se me asignaron. Todo esto aportando claramente en mi actualización de ciertos conceptos y metodologías necesarios para mi desarrollo profesional. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
\textbf{Belen del Rocio Ramos Rios} \\
En esta entrega, me enfoqué en el diseño de la arquitectura de la landing page, trabajando en sistemas de organización, etiquetado y navegación. Apliqué nuevas herramientas de documentación y diseñé la arquitectura de información, lo que fue clave para mejorar la experiencia de usuario. Además, participé activamente en la creación de wireframes y mockups para asegurar la coherencia visual y funcional del proyecto. \\
\textbf{Mateo Alejandro Vilchez Rios} \\
Para esta entrega, me enfoqué en profundizar mis conocimientos en la configuración de software y la documentación de la arquitectura. Trabajé en la creación y diseño de los diagramas de arquitectura (diagrama de contexto, de contenedor y de componentes), aplicando metodologías ágiles para organizar el flujo de trabajo. Además, implementé mejoras en la UI de la landing page mediante wireframes y mockups, siguiendo las guías de estilo establecidas. \\
\textbf{Alex Avila Asto} \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
\\} 
&
\parbox[t]{5cm}{
\textbf{TB2:} \\
(NO EDITAR)
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
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
Cree repositorios para almacenar nuestro informe con un registro de versiones constante, además de comenzar un registro de los puntos que nos falta completar.Siempre monitoreando y asesorando a mi equipo acerca de sus avances. En donde, la necesidad del aprendizaje permanente nos llevó al uso de mejores herramientas para la solución del proyecto.  \\
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
En conjunto, hemos comprendido que el aprendizaje permanente no solo es un requisito para mantenernos actualizados, sino también un pilar que nos permite enfrentar desafíos con soluciones innovadoras y eficientes, garantizando así el éxito y la relevancia de nuestros proyectos. \\
} \\

\cline{2-3}

&  
\parbox[t]{6cm}{
\textbf{TB2:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
\textbf{Belen del Rocio Ramos Rios} \\
Reconocí la necesidad de seguir aprendiendo y optimizando las herramientas de documentación y los procesos de desarrollo, específicamente en la gestión de etiquetas SEO y sistemas de búsqueda. Este enfoque me ayudó a asegurar que la landing page esté bien organizada y sea accesible, cumpliendo con los estándares de navegación y experiencia del usuario.\\
\textbf{Mateo Alejandro Vilchez Rios} \\
Identifiqué la importancia de seguir aprendiendo sobre gestión del código fuente y configuración del entorno de desarrollo, lo que me permitió mejorar mis contribuciones al proyecto. También trabajé en la integración de buenas prácticas de gestión de código y configuración de despliegue, asegurando que el proceso de desarrollo sea más eficiente y colaborativo. \\
\textbf{Alex Avila Asto} \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
}
&
\parbox[t]{5cm}{
\textbf{TB2:} \\
(NO EDITAR)
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. \\
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
Contribuir a la mejora del informe del proyecto a través del uso de nuevas herramientas, preparando el camino para participar en el desarrollo del frontend y en la estructuración de la base de datos en futuras etapas del proyecto. \\
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
Aportar en la mejora del informe del proyecto y asegurar la correcta aplicación de metodologías relevantes, con la vista puesta en fortalecer mi participación en el desarrollo del backend en futuras fases del proyecto. \\
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
El éxito se medirá a través de la calidad del informe entregado y la planificación efectiva para próximas fases. \\
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
El éxito se medirá por la calidad del informe entregado y la preparación para contribuir al backend en las siguientes etapas. \\
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
Este objetivo implica tanto la consolidación del trabajo actual como la preparación para tareas más técnicas. \\
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
Este objetivo desafía a avanzar en áreas técnicas mientras se asegura la calidad del trabajo actual. \\
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
A lo largo del desarrollo del proyecto, he enfocado mis esfuerzos en asegurar que cada acción esté en sintonía con los objetivos estratégicos de \textit{Laurate} Perú. La planificación rigurosa y la atención a los detalles han sido claves para contribuir al cumplimiento de los lineamientos que la universidad establece como prioritarios.\\
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
 El proyecto que hemos realizado no solo es un reflejo de nuestro esfuerzo individual, sino también de nuestra capacidad para alinear nuestras acciones con los objetivos estratégicos de \textit{Laurate} Perú. \\
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
 Para esta entrega, logré cumplir con todas mis responsabilidades dentro del plazo acordado, asegurando que cada tarea se completara según lo previsto. La claridad en las fechas límite desde el principio me permitió organizar mi trabajo de manera efectiva. \\
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
En esta entrega, logré cumplir con mis tareas dentro de los tiempos previstos, manteniendo un enfoque constante en las fechas límite. Esto no solo me permitió finalizar mis responsabilidades a tiempo, sino también estar disponible para asistir a mi equipo. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
}}
&  
\parbox[t]{3cm}{
Abel Ortega Huaraca \\
}
&
\parbox[t]{5cm}{
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
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
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 21-08-2024 \\
\textbf{Fecha de entrega:} 28-08-2024 \\
} \\
\bottomrule

\end{longtable}

\newpage

***Project Report Collaboration Insights***

::: warn
Para mayor información, haga click en la [URL](https://github.com/CodeMinds-AppsMoviles-SW65/CodeMinds-Informe-del-Proyecto/pulse) 
:::

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/insights-2.png)

\newpage

*Actividades Colaborativas* ***(Github Kanban)***

::: warn
Para mayor información, haga click en la [URL](https://github.com/orgs/CodeMinds-AppsMoviles-SW65/projects/1)
:::

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-1.png)

![Imagen extraída de Github - Codeminds](src/img/Cap1/report-collaboration-2.png)

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
