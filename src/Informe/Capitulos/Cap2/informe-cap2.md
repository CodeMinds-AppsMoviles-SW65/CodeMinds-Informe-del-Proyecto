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

# Capítulo II: *Needfinding*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

## Competidores


![Recurso extraído de Canva](src/img/cap2/competidores-introduccion.png)

En un mercado donde la privacidad y la seguridad de los datos personales se han convertido en pilares fundamentales. Un análisis detallado de las soluciones existentes es esencial para identificar oportunidades de diferenciación e innovación, garantizando así que la propuesta de CodeMinds no solo cumpla con las expectativas de los usuarios, sino que también sobresalga en un entorno competitivo y exigente.

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


### Estrategias y tácticas frente a Competidores

::: info
Según Kašparová (2022), en el contexto de la gestión estratégica moderna, la inteligencia empresarial se ha convertido en un componente clave para desarrollar y mantener una ventaja competitiva sostenible. La autora argumenta que la capacidad de una empresa para analizar grandes volúmenes de datos y convertirlos en información accionable es crucial para tomar decisiones estratégicas efectivas. Este enfoque permite a las empresas anticipar movimientos de la competencia, adaptar sus estrategias en tiempo real y responder de manera proactiva a las oportunidades y amenazas del mercado, lo que es esencial para asegurar el éxito a largo plazo en un entorno empresarial altamente dinámico.
:::


Teniendo en cuenta el análisis SWOT previamente presentado para CodeMinds, proponemos las siguientes estrategias competitivas:

**Estrategias competitivas para CodeMinds**

1. **Diferenciación a través de la Innovación:**

::: norm
**Estrategia:** *CodeMinds* debe destacarse en el mercado por ofrecer soluciones de privacidad y seguridad digital que no solo cumplan con las expectativas actuales, sino que también anticipen las necesidades futuras. La innovación continua en la protección de datos es crucial para mantener una ventaja competitiva. 

**Tácticas:**

   - Identificar tendencias emergentes y nuevas amenazas en el ámbito de la seguridad digital, asegurando que CodeMinds siempre esté un paso adelante.
  
   - Invertir en I+D para crear herramientas de protección de datos y correos temporales que ofrezcan funcionalidades únicas y altamente efectivas.

   - Implementar un ciclo regular de lanzamientos de nuevas funcionalidades, promoviendo activamente estas innovaciones a través de campañas de marketing dirigidas.

:::

2. **Enfoque en Segmentos Específicos del Mercado:**
   
::: norm
**Estrategia:** *CodeMinds* debe personalizar sus soluciones para segmentos específicos, como estudiantes de todos los niveles educativos que requieren herramientas confiables y fáciles de usar para proteger su información. 

**Tácticas:**

   - Desarrollar características específicas para estudiantes y académicos, como bandejas de entrada seguras y correos temporales con mayor control.
  
   - Establecer asociaciones con instituciones educativas para integrar CodeMinds en sus plataformas tecnológicas y ofrecer servicios exclusivos.
  
   - Dirigir campañas publicitarias específicamente a estudiantes, resaltando la relevancia y el valor de CodeMinds en sus actividades académicas diarias.

:::

3. **Alianzas Estratégicas:**
   
::: norm
**Estrategia:** Formar alianzas con empresas y organizaciones clave en el sector de la tecnología y la ciberseguridad para mejorar la oferta de CodeMinds y expandir su presencia en el mercado.  

**Tácticas:**

   - Integrar soluciones de seguridad avanzadas de socios estratégicos, fortaleciendo así la propuesta de valor de CodeMinds.
  
   - Trabajar con plataformas de e-learning y universidades para ofrecer paquetes combinados de servicios educativos y protección de datos.

:::

4. **Expansión Internacional:**
   
::: norm
**Estrategia:** *CodeMinds* debe considerar la expansión hacia mercados internacionales, adaptando sus productos y servicios a las necesidades de usuarios en diferentes regiones y culturas. 

**Tácticas:**

   - Adaptar la interfaz, el contenido y las funcionalidades de CodeMinds a diferentes idiomas y normas culturales para facilitar su adopción en mercados extranjeros.
  
   - Identificar y evaluar oportunidades en mercados emergentes donde la demanda de soluciones de privacidad digital está en crecimiento, y adaptar la estrategia de entrada según las condiciones locales.
  
   - Establecer alianzas con empresas locales en mercados objetivo para facilitar la entrada y acelerar la adopción de CodeMinds.

:::

**Tácticas Específicas para CodeMinds**

1. **Inversión en Marketing Diferenciado:**

::: info
**Táctica:** Desarrollar una identidad de marca que subraye la superioridad técnica y la confiabilidad de CodeMinds en el ámbito de la privacidad y la seguridad digital. 

**Acciones:**

   - Crear y distribuir contenido que no solo promueva CodeMinds, sino que también eduque a los usuarios sobre la importancia de la seguridad digital.
  
   - Aprovechar testimonios de usuarios clave y casos de éxito para generar confianza y credibilidad en la marca.

:::

2. **Monitoreo Competitivo Continuo:**

::: info
**Táctica:** Mantener un análisis constante de las acciones de los competidores para anticipar movimientos en el mercado y ajustar las estrategias de CodeMinds en consecuencia.  

**Acciones:**

   - Monitorizar continuamente los nuevos productos, precios y promociones de los competidores para ajustar las ofertas de CodeMinds en tiempo real.

   - Utilizar herramientas avanzadas de inteligencia de mercado para identificar oportunidades y amenazas emergentes.

:::

3. **Optimización de la Experiencia del Usuario (UX):**

::: info
**Táctica:** Mejorar continuamente la experiencia del usuario en la aplicación de CodeMinds para aumentar la retención y satisfacción de los clientes.  

**Acciones:**

   - Implementar sistemas para recopilar y analizar feedback de los usuarios, utilizando esta información para realizar mejoras iterativas en la interfaz y funcionalidades.

   - Realizar pruebas A/B para experimentar con diferentes diseños y flujos de usuario, identificando las configuraciones que maximicen la satisfacción y el uso efectivo de la aplicación.

:::

4. **Fomento de la Fidelización del Cliente:**

::: info
**Táctica:** Implementar programas y estrategias para aumentar la fidelidad del cliente y promover la retención a largo plazo.  

**Acciones:**

   - Desarrollar programas de fidelización que ofrezcan recompensas a los usuarios por su lealtad, como descuentos, acceso a funciones premium o beneficios exclusivos.

   - Enviar comunicaciones personalizadas a los clientes basadas en su comportamiento y uso de la aplicación, ofreciendo sugerencias de uso, actualizaciones de productos y promociones adaptadas a sus necesidades.

:::

5. **Estrategias de Precios y Paquetes Competitivos:**

::: info
**Táctica:** Ajustar estratégicamente los precios y paquetes de servicios para competir de manera efectiva en el mercado.  

**Acciones:**

   - Realizar análisis de precios comparativos y ajustar los precios de acuerdo con el valor percibido por los clientes.

   - Ofrecer paquetes personalizados que se ajusten a las necesidades específicas de diferentes tipos de clientes, como estudiantes y profesionales.

:::

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

**Segmento 1: Estudiantes de nivel escolar**

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
Pol Adriano Ramos Ríos, un joven de 14 años, utiliza principalmente su laptop HP para realizar tareas escolares y, ocasionalmente, su celular. Aunque no ha activado medidas de seguridad adicionales en su dispositivo, confía en las configuraciones predeterminadas de Windows y actualiza su sistema operativo con poca frecuencia. Pol tiene entre 12 y 15 aplicaciones instaladas en su dispositivo y guarda su información en la nube, específicamente en OneDrive, como medida de respaldo.
En cuanto a la navegación por internet, Pol utiliza el navegador Brave, que prefiere por su VPN integrada y su capacidad para bloquear anuncios y cookies, lo que le brinda una sensación de mayor seguridad. No ha sentido que su información personal esté en riesgo, excepto en ocasiones al utilizar Chrome u Opera, y evita aceptar cookies por preocupaciones de rastreo. Sus sitios web favoritos son Twitch y YouTube, donde sigue transmisiones de videojuegos y busca contenido educativo. Pol ha utilizado el modo incógnito para explorar herramientas como Tor y valora las extensiones de privacidad que le ofrece Brave.
Pol se asegura de que un sitio web sea seguro antes de ingresar información personal utilizando un correo secundario o falso. No ha recibido formación específica sobre privacidad en internet, pero es cauteloso al interactuar con sitios que solicitan demasiada información personal. En cuanto a las aplicaciones, Pol prefiere no descargar muchas, pero cuando lo hace, las prueba exhaustivamente antes de confiar en ellas, llegando incluso a resetear su computadora como medida de precaución.
Pol considera que iOS es más seguro que Android, pero cuando se trata de usar dispositivos, prefiere su computadora porque siente que le ofrece un mayor control sobre sus actividades y datos. Para sus tareas escolares, prefiere utilizar sitios web como YouTube y ChatGPT, que le brindan explicaciones directas y fáciles de entender.
Finalmente, Pol confía en su capacidad para evaluar nuevas aplicaciones y sitios web a través de reseñas y calificaciones antes de instalarlas. Aunque no ha dejado de usar ninguna aplicación por motivos de seguridad, siempre verifica su confiabilidad antes de continuar usándolas.

![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_AdrianoRamos.png)


**Entrevista #2**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Grecia Jazmín Capristán Yepes \\ \hline
\textbf{Edad}                 & 14 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & inicio - fin           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**
Grecia Jazmín Capristán Yepes, una joven de 14 años, utiliza principalmente su iPhone para acceder a internet. Aunque su dispositivo cuenta con medidas de seguridad activadas, Grecia no está completamente segura de cuáles son. Sin embargo, se asegura de mantener su sistema operativo actualizado, siguiendo las indicaciones de su teléfono cada vez que se le solicita. En su dispositivo, solo tiene instaladas cinco aplicaciones, entre las cuales usa regularmente TikTok, Instagram y WhatsApp. Para navegar por internet, prefiere utilizar Google Chrome, confiando en las herramientas de seguridad del navegador para bloquear sitios peligrosos, lo que le proporciona una sensación de tranquilidad al sentir que su información no está en riesgo.
Grecia es selectiva al aceptar cookies: solo las permite en sitios web en los que confía y las rechaza en aquellos que le generan desconfianza. Aunque no suele usar el modo de navegación incógnito, ha experimentado con bloqueadores de anuncios. A pesar de no haber recibido formación específica sobre protección de la privacidad en internet, Grecia evita proporcionar información personal en sitios que le generan sospechas. En cuanto a las aplicaciones, confía únicamente en algunas para mantener su información segura, y prefiere utilizar un correo electrónico secundario al registrarse en aquellas que no le inspiran total confianza.
Grecia reconoce que, si su información personal llegara a ser comprometida, no estaría segura de cómo manejar la situación, ya que nunca ha enfrentado un problema de este tipo. No ha utilizado VPNs y, por el momento, no tiene preocupaciones particulares sobre su seguridad en línea. Tampoco sabría qué hacer si alguien intentara acceder a su información sin su permiso.
Grecia prefiere iOS como sistema operativo y considera que su dispositivo móvil es más seguro que una computadora. Para sus tareas escolares, opta por utilizar sitios web en lugar de aplicaciones, ya que considera que estos le ofrecen mayor información. Aunque no utiliza aplicaciones específicas para proteger su privacidad, se mantiene informada sobre nuevas herramientas a través de recomendaciones de sus compañeros o anuncios. Antes de instalar una nueva aplicación, Grecia se asegura de que esta solicite únicamente los permisos adecuados. En el pasado, ha dejado de usar aplicaciones cuando no se sentía segura, como en una ocasión en la que se filtraron sus contactos, lo que la llevó a cambiar su número de teléfono.


![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_GreciaCapristan.png)


**Entrevista #3**

\begin{table}[H]
\begin{center}  % Centrar la tabla
\begin{tabular}{|p{5cm}|p{6cm}|}  % Ajusta los anchos de las columnas
\hline
\textbf{Nombre y Apellido}    & Carlet Gil Olivera \\ \hline
\textbf{Edad}                 & 17 años                \\ \hline
\textbf{Ubicación geográfica} & Trujillo, Perú         \\ \hline
\textbf{Grado}                & Secundaria             \\ \hline
\textbf{Tiempo de entrevista} & inicio - fin           \\ \hline
\end{tabular}
\end{center}
\end{table}

**Resumen de la entrevista**
Carlet, de 17 años, utiliza su celular para acceder a internet y confía en las medidas de seguridad que vienen preinstaladas en su dispositivo Apple. Debido a que no comparte su celular con otras personas, siente que su información personal está más protegida. Para navegar por internet, utiliza el navegador Safari, aunque no está muy informada sobre sus características de seguridad. En ocasiones, ha sentido que su información podría estar en riesgo al visitar sitios con numerosos anuncios emergentes, y admite que suele aceptar cookies sin leer los términos y condiciones.
Carlet utiliza el modo de navegación privada de manera ocasional, sobre todo cuando accede a páginas que podrían contener virus o para ver películas. Sin embargo, nunca ha utilizado bloqueadores de anuncios ni extensiones de privacidad, optando en su lugar por salir de los sitios que considera inseguros. Aunque reconoce el ícono del candado en la barra de direcciones como un indicador de seguridad en sitios web, no ha recibido ninguna educación formal sobre cómo proteger su privacidad en línea.
Tiende a desconfiar de los sitios web que solicitan demasiada información personal y evita proporcionar datos sensibles. Aunque no confía completamente en las aplicaciones para mantener su información segura, suele descargarlas por entretenimiento, después de investigar brevemente sobre ellas. En caso de que su información personal fuera comprometida, investigaría más a fondo y consideraría presentar una denuncia.
Carlet nunca ha utilizado una VPN, pero expresa preocupación por la posible filtración de su información privada. Para mitigar estos riesgos, evita compartir datos excesivos y abandona aplicaciones o sitios web sospechosos. Prefiere utilizar dispositivos con el sistema operativo iOS y valora la protección adicional que ofrecen las contraseñas. Para realizar sus tareas escolares, prefiere utilizar sitios web en lugar de aplicaciones y no emplea herramientas específicas para proteger su privacidad en línea.


![Imagen extraída del video de entrevistas](src/img/Cap2/segmento1_CarletOlivera.png)


### Análisis de entrevistas

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

## *Needfinding*

En el cambiante panorama digital de hoy, CodeMinds se destaca por su compromiso con la excelencia al abordar las necesidades de seguridad y privacidad de los usuarios. Esta sección, denominada Needfinding, subraya nuestra firme creencia en la importancia de comprender y escuchar a fondo las preocupaciones y requerimientos de nuestros usuarios.

En CodeMinds, estamos convencidos de que el éxito de nuestras soluciones radica en nuestra capacidad para responder eficazmente a los desafíos relacionados con la protección de datos y la gestión de la privacidad. A través de investigaciones exhaustivas y la recopilación de información valiosa, hemos desarrollado una comprensión profunda de las necesidades y deseos de los estudiantes, quienes enfrentan riesgos significativos en su interacción con la tecnología. Este conocimiento nos impulsa a ofrecer herramientas y características que se alinean perfectamente con las expectativas de nuestros usuarios, asegurando que CodeMinds sea una solución esencial para la protección de datos en el entorno digital.

En la siguiente sección de Needfinding, exploraremos cómo CodeMinds se dedica a comprender y abordar proactivamente las necesidades cambiantes de nuestros usuarios, permitiéndoles gestionar su información personal de manera más segura y eficiente que nunca.

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

:::info

Kalbach (2016) señala que el *User Journey Mapping* es una herramienta fundamental en el diseño de experiencias de usuario, ya que permite visualizar de manera clara y detallada las etapas por las que pasa un usuario antes de decidir utilizar un producto o servicio. En el contexto de *CodeMinds*, donde ofrecemos soluciones de correos temporales para estudiantes, este mapeo nos permite identificar los puntos de contacto críticos y los posibles obstáculos que enfrentan los estudiantes de nivel secundario y universitario antes de utilizar nuestra aplicación. Este enfoque nos permite desarrollar estrategias más efectivas para atraer y retener usuarios, alineando nuestras soluciones con sus necesidades específicas y mejorando su experiencia general.

:::

Las siguientes secciones detallan los *User Journey Maps* de cada segmento de usuarios, mostrando cómo los estudiantes pasan por etapas de concienciación, investigación y evaluación antes de adoptar los correos temporales como una solución segura para proteger su información en línea.


***User Journey Mapping:*** John Doe

![](src/img/Cap2/jm_codeminds.png)

![Artefacto creado en UXPressia](src/img/Cap2/journeymap-segmento1.png)

***User Journey Mapping*** Nombre del user persona del segundo segmento

![](src/img/Cap2/jm_codeminds.png)

![Artefacto creado en UXPressia](src/img/Cap2/journeymap-segmento2.png)


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
\hline
\end{longtable}

\begin{longtable}{|>{\centering\arraybackslash}p{1cm}|>{\centering\arraybackslash}p{3cm}|>{\centering\arraybackslash}p{4cm}|>{\centering\arraybackslash}p{5cm}|>{\centering\arraybackslash}p{1cm}|}
\hline
\textbf{ID} & \textbf{Título} & \textbf{Descripción} & \textbf{Criterios de Aceptación} & \textbf{Epic} \\
\hline
\endfirsthead
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
\hline
\end{longtable}

\newpage

### *Impact Mapping*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *Product Backlog*

:::info

Una de las técnicas más utilizadas para estimar el esfuerzo necesario para completar cada tarea es la escala de Fibonacci, la cual permite asignar puntos de historia de manera proporcional a la complejidad y tiempo requerido. Como señala Smith (2020), esta escala no lineal facilita la identificación de tareas que requieren un mayor esfuerzo, lo que resulta en una planificación más precisa y eficiente

:::

A continuación, se presenta la tabla de nuestro *Product Backlog*, demostrando cómo se alinean nuestros recursos con las necesidades más urgentes de nuestros usuarios.

\begin{longtable}{|c|p{4cm}|p{7cm}|c|}
\hline
\textbf{ID} & \textbf{Título} & \textbf{Descripción} & \textbf{Story Points} \\
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
\hline
\end{longtable}
