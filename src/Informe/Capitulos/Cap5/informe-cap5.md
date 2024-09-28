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

### Sprint 2

#### Sprint Planning 2

#### Sprint Backlog 2

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

#### *Development Evidence for Sprint Review*

#### *Testing Suite Evidence for Sprint Review*

#### *Execution Suite for Sprint Review*

#### *Services Documentation Evidence for Sprint Review*

#### *Software Deployment Evidence for Sprint Review*

#### *Team Collaboration Insights during Sprint*

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

