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

# Capítulo II: *Needfinding*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

## Competidores

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### Análisis competitivo

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### Estrategias y tácticas frente a Competidores

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

\newpage

## Entrevistas

![Recurso extraído de Canva](src/img/Cap2/entrevistas-introduccion.png)

::: note
Para acceder al video de las entrevistas, haga click en la [URL](https://www.github.com)
(falta definir la url)
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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### Análisis de entrevistas

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

## *Needfinding*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *User Personas*

Presentaremos los User Persona por cada segmento objetivo, en los cuales nos basamos en los usuarios
ideales de cada segmento. A continuación, los presentamos:

*User Persona 1* - Segmento de Estudiantes de secundaria: John Doe

aca la img xd

*User Persona 2* - Segmento de Estudiantes de universidad-postgrado: John Doe 2

// img

### *User Task Matrix*

*User Task Matrix*: John Doe 2 y John Doe 3

### *User Journey Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *Empathy Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *As-Is Scenario Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

\newpage

## *Requirements specification*

En este capítulo, nos adentramos en la identificación detallada de los requisitos esenciales que permitirán a los usuarios interactuar de manera efectiva y satisfactoria con nuestra aplicación. Es fundamental comprender las necesidades y expectativas de quienes utilizarán nuestra mobile application, lo que nos guiará en la creación de una experiencia de usuario óptima.

![Recurso extraído de Canva](src/img/Cap2/requeriments-specification.png)

### *To-Be Scenario Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *User Stories*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *Impact Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *Product Backlog*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

