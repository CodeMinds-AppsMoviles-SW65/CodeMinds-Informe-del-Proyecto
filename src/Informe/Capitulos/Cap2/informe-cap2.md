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
  \usepackage{float} 
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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *User Personas*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

### *User Task Matrix*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

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

### *User Stories*

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.

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
