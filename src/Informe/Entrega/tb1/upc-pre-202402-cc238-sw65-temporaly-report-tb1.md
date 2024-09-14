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
bibliography: src/Informe/Entrega/tb1/bibliografia.bib
csl: src/Informe/Entrega/tb1/apa.csl
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

**Registro de Versiones del Informe**

\begin{longtable}{|c|c|c|p{6cm}|}
  \hline
  \textbf{Versión} & \textbf{Fecha} & \textbf{Autor} & \textbf{Descripción de Modificación} \\
  \hline
  tb1 & 27/08/2024 & Ortega Huaraca, Abel & Ayudé con la estructura del informe en general. Respecto a los puntos específicos, contribuí con la elaboración del \textit{Solution Profile}, \textit{Startup Profile}, Segmentos objetivo, \textit{User Stories} y una introducción para los \textit{Requirements Specification}. \\
  \hline
  tb1 & 27/08/2024 & Ramos Rios, Belén del Rocio & Realice la descripción de competidores, análisis competitivo y las estrategias frente a competidores. También aporté en la creación de los \textit{User Journey Mapping}, \textit{To-Be Scenario Mapping} y el \textit{Product Backlog}. \\
  \hline
  tb1 & 27/08/2024 & Vilchez Rios, Mateo Alejandro & Capitulo 1: \textit{Lean UX Process} - Antecendentes y Problemática, Capitulo 2: Registro de Entrevista - \textit{Empathy Map} - \textit{As-is} - \textit{Scenario Mapping} - \textit{Impact Mapping}. \\
  \hline
  tb1 & 27/08/2024 & Avila Asto, Alex Ramon Alberto & Realicé el análisis de entrevistas, \textit{netfinding}, la creación de \textit{User Personas} y la tabla de \textit{User Task Matrix}. \\
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
\parbox[t]{4cm}{
\textit{Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.}
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

\hline

\parbox[t]{4cm}{
\textit{Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de software.}
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

# Bibliografía
