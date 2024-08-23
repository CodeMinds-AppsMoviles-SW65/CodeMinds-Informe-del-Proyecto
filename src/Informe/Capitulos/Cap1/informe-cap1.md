---
title: "Universidad Peruana de Ciencias Aplicadas - Informe de Trabajo Final"
author: 
  - "Startup: CodeMinds"
  - "Producto: Temporaly"
  - "Profesor: Mayta Guillermo, Jorge Luis"
  - "Integrantes:"
  - "Ortega Huaraca, Abel Angel - U20201B380"
  - "Avila Asto, Alex Ramon - u20221a322"
  - "[Name]"
  - "[Name]"
  - "[Name]"
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
  \usepackage{multirow}
  \usepackage{longtable}
  \usepackage{geometry}
 
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
  tb1 & 20/08/2024 & Ortega Huaraca, Abel & Falta escribir uu. \\
  \hline
  tb1 & lorem & lorem, lorem & lorem. \\
  \hline
  tb1 & lorem & lorem, lorem & lorem. \\
  \hline
  tb1 & lorem & lorem, lorem & lorem. \\
  \hline
\end{longtable}

\newpage

***Student Outcome***

El curso contribuye al cumplimiento del Student Outcome ABET: *ABET-EAC - Student Outcome 7*

* **Criterio:** *La capacidad de adquirir y aplicar nuevos conocimientos según sea necesario, utilizando estrategias de aprendizaje apropiadas*.

En el siguiente cuadro se describe las acciones realizadas y enunciadas de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro de ***ABET - EAC - Student Outcome 7.***

\begin{longtable}{|p{4cm}|p{6cm}|p{5cm}|}
\hline
\textbf{Criterio Específico} & \textbf{Acciones Realizadas} & \textbf{Conclusiones} \\
\hline
\endfirsthead

\hline
\textbf{Criterio Específico} & \textbf{Acciones Realizadas} & \textbf{Conclusiones} \\
\hline
\endhead

\multirow{3}{*}{
\parbox[t]{4cm}{
Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.
}} 
&  
\parbox[t]{6cm}{
\textbf{TB1:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Coordiné y realicé la reunión inicial del proyecto, explicando claramente los objetivos y el plan de trabajo. Cree diferentes reuniones para clarificar los roles de cada integrante del equipo. \\
\textbf{Belen} \\
lorem ipsum. \\
\textbf{Mateo} \\
lorem ipsum. \\
\textbf{Alex} \\
lorem ipsum. \\} 
&
\parbox[t]{5cm}{
\textbf{TB1:} \\
Falta escribir las conclusiones uu. \\
} \\ 

\hline

\multirow{3}{*}{
\parbox[t]{4cm}{
Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de software.
}}
&  
\parbox[t]{6cm}{
\textbf{TB1:} \\
\textbf{Abel Angel Ortega Huaraca} \\
Cree repositorios para almacenar nuestro informe con un registro de versiones constante, además de comenzar un registro de los puntos que nos falta completar. \\
\textbf{Belen} \\
lorem ipsum. \\
\textbf{Mateo} \\
lorem ipsum. \\
\textbf{Alex} \\
lorem ipsum. \\}
&
\parbox[t]{5cm}{
\textbf{TB1:} \\
falta escribir las conclusiones uu. \\
} \\ 
\hline
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
\textbf{Fecha de inicio:} 28-08-2024 \\
\textbf{Fecha de entrega:} 02-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 28-08-2024 \\
\textbf{Fecha de entrega:} 02-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 28-08-2024 \\
\textbf{Fecha de entrega:} 02-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 28-08-2024 \\
\textbf{Fecha de entrega:} 02-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} 28-08-2024 \\
\textbf{Fecha de entrega:} 02-09-2024 \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Belen
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Mateo \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\cline{2-4}
&
\parbox[t]{3cm}{
Alex \\
}
&
\parbox[t]{5cm}{
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. \\
}
&
\parbox[t]{3cm}{
\textbf{Fecha de inicio:} dd-mm-aaaa \\
\textbf{Fecha de entrega:} dd-mm-aaaa \\
} \\
\hline

\end{longtable}

\newpage

***Project Report Collaboration Insights***

::: warn
Falta adjuntar el github de la organizacion
:::

\newpage

*Actividades Colaborativas* ***(Github Kanban)***

::: warn
Falta adjuntar las fotos y para cada foto su descripcion de colaboracion
:::

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
\includegraphics[width=\linewidth]{src/img/Integrantes/gato.png}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Belen} \\
\textit{Ingeniera de Software} \\
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac.
\end{minipage}
}
\end{tcolorbox}

\begin{tcolorbox}[colframe=mybackground, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
\begin{minipage}[c]{0.3\textwidth}
\includegraphics[width=\linewidth]{src/img/Integrantes/gato.png}
\end{minipage}
\hfill
\begin{minipage}[c]{0.65\textwidth}
\textbf{Mateo} \\
\textit{Ingeniero de Software} \\
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac.
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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *Lean UX Process*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

#### *Lean UX Problem Statements*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

#### *Lean UX Assumptions*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

#### *Lean UX Hypothesis Statements*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

#### *Lean UX Canvas*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

\newpage

## Segmentos Objetivo

En CodeMinds, nuestro enfoque está en atender a un público clave: estudiantes de todos los niveles educativos. Desde estudiantes escolares que están dando sus primeros pasos en el mundo digital, hasta aquellos en niveles superiores como pregrado y postgrado que buscan herramientas avanzadas para proteger su información. Nuestro objetivo es ofrecer soluciones de seguridad que se adapten a las necesidades específicas de cada grupo, garantizando que todos puedan proteger sus datos con confianza y facilidad.

![Tabla del segmento objetivo 1 - Elaboración propia](src/img/Cap1/segmento-objetivo-1.png)

![Tabla del segmento objetivo 2 - Elaboración propia](src/img/Cap1/segmento-objetivo-2.png)
