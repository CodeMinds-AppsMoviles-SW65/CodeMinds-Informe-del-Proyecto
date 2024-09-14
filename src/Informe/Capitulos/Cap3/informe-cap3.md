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