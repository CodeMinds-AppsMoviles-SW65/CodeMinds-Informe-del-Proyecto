---
title: "Universidad Peruana de Ciencias Aplicadas - Informe de Trabajo Final"
author: 
  - "Startup: [Startup Name]"
  - "Producto: [Software Name]"
  - "Profesor: [Professor Name]"
  - "Integrantes:"
  - "[Name]"
  - "[Name]"
  - "[Name]"
  - "[Name]"
  - "[Name]"
date: "[Date]"
subject: "Markdown"
keywords: [Markdown, Report]
subtitle: "[Course Name] - [Seccion Code] - [Course Code]"
lang: "es"
colorlinks: true
footer-left: "[Startup Name]"
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

# Cap 1

## (SubCap) 1.1

### (SubCap) 1.1.1

#### (SubCap) 1.1.1.1

#### (SubCap) 1.1.1.2

### (SubCap) 1.1.2

### (SubCap) 1.1.3

## (SubCap) 1.2

## (SubCap) 1.3

# Cap 2

# Cap 3

# Cap 4

# Cap 5


**Negritas**

*Cursivas*

***Negritas y Cursivas***

- Lista normal

* Lista con asterisco

1. Lista numerica

1) Lista numerica

::: box
Texbox de tipo: **box**
:::

::: info
Texbox de tipo: **info**
:::

::: error
Texbox de tipo: **error**
:::

::: norm
Texbox de tipo: **norm**
:::

::: warn
Texbox de tipo: **warn**
:::

::: attn
Texbox de tipo: **attn**
:::

::: code
Texbox de tipo: **code**
:::

::: learn
Texbox de tipo: **learn**
:::

::: scenario
Texbox de tipo: **scenario**
:::

::: outline
Texbox de tipo: **outline**
:::

::: prereqs
Texbox de tipo: **prereqs**
:::

::: labtime
Texbox de tipo: **labtime**
:::

::: note
Specialbox de tipo: **note**
:::

::: tip
Specialbox de tipo: **tip**
:::

::: warning
Specialbox de tipo: **warning**
:::

::: caution
Specialbox de tipo: **caution**
:::

::: important
Specialbox de tipo: **important**
:::

Bloque de codigo solo:

```python
# Solicitar al usuario que ingrese dos números
numero1 = float(input("Ingrese el primer número: "))
numero2 = float(input("Ingrese el segundo número: "))

# Sumar los números
suma = numero1 + numero2

# Mostrar el resultado
print(f"La suma de {numero1} y {numero2} es: {suma}")
```

Bloque de codigo dentro de un texbox:

::: box 
```java
import java.util.Scanner;

public class SumarNumeros {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número: ");
        double numero1 = scanner.nextDouble();

        System.out.print("Ingrese el segundo número: ");
        double numero2 = scanner.nextDouble();

        double suma = numero1 + numero2;

        System.out.println("La suma de " + numero1 + " y " + numero2 + " es: " + suma);
    }
}
```
:::

Bloque de codigo dentro de un specialbox:

::: note
```cpp
#include <iostream> // Incluye la biblioteca de entrada/salida

int main() {
    // Imprime "Hola Mundo" en la consola
    std::cout << "Hola Mundo" << std::endl;

    // Declarar dos variables enteras
    int a = 5;
    int b = 10;

    // Sumar las variables y almacenar el resultado en una tercera variable
    int suma = a + b;

    // Imprimir el resultado de la suma
    std::cout << "La suma de " << a << " y " << b << " es: " << suma << std::endl;

    // Indicar que el programa terminó correctamente
    return 0;
}
```
:::

Como utilizar LINKS:

::: note
Para acceder al Github de la organización, haga click a la [URL](https://github.com/)
:::

Para acceder al Github de la organización, haga click a la [URL](https://github.com/)

Como utilizar Imagenes:

Ruta directa:

![](color-naranja.png)

Imagen dentro de carpeta(s):

![](img/color-naranja.png)

Imagen con pie:

![Imagen de elaboración propia](img/color-naranja.png)

Marco de integrante:

\definecolor{mybackground}{HTML}{f2e7e5}

\begin{tcolorbox}[colframe=black, colback=mybackground, boxrule=0.8mm, width=\textwidth, sharp corners]
{
    \begin{minipage}[c]{0.3\textwidth}
        \includegraphics[width=\linewidth]{gato.png}
    \end{minipage}
    \hfill
    \begin{minipage}[c]{0.65\textwidth}
        \textbf{Nombre del Integrante} \\
        \textit{Profesión} \\
        Descripción general: Aquí puedes colocar una breve descripción del integrante, su rol en el equipo, y cualquier otra información relevante.
    \end{minipage}
}
\end{tcolorbox}

::: important

Comando para la conversion de archivos markdown a pdf: 

```bash
pandoc "name.md" -o "name.pdf" --from markdown+yaml_metadata_block+raw_html --template eisvogel --filter pandoc-latex-environment --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src
```
:::



