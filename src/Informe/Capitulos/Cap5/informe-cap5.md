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
\textbf{Tiempo de entrevista} & inicio - fin           \\ \hline
\end{tabular}
\end{center}
\end{table}



### Evualuaciones segun heuristicas


