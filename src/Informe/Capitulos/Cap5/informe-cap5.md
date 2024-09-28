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

#### *Development Evidence for Sprint Review*

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

\vspace{2cm}

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

