# Plantilla LaTeX para Memorias UAL

![foto portada plantilla](https://github.com/jnl941/memoria-ual-light-overleaf/blob/main/portada.png)
Esta plantilla está diseñada para la elaboración de memorias académicas para la Universidad de Almería (UAL). La plantilla es ligera y compatible con la versión gratuita de Overleaf. Hay un ejemplo visible en [UALmemoriaPlantilla.pdf](UALmemoriaPlantilla.pdf)


## Estructura de la plantilla

```
├── Main.tex                  # Archivo principal de compilación
├── content.tex               # Contenido de la memoria (capítulos)
├── titlepage.tex             # Configuración de la portada
├── defs.tex                  # Definiciones matemáticas y colores
├── estiloscodigoprogramacion.tex # Estilos para insertar código fuente
├── configuracioninicial.tex  # Configuración general del documento
├── UAL.sty                   # Estilo personalizado para la UAL
└── Figuras/
    └── logos/                # Logotipos e imágenes institucionales
```

## Características

- Diseño institucional con colores oficiales de la UAL
- Estilo personalizado para cabeceras y pies de página
- Soporte para inserción de código fuente con resaltado de sintaxis
- Formato adecuado para capítulos, secciones y subsecciones
- Compatible con la versión gratuita de Overleaf

## Cómo usar esta plantilla

### En Overleaf

1. Descarga todos los archivos de esta plantilla
2. Crea un nuevo proyecto en Overleaf
3. Sube todos los archivos al proyecto
4. Define Main.tex como archivo principal de compilación
5. Compila el documento con el botón "Compilar" o "Compile"

### Personalizando la portada

Edita el archivo titlepage.tex para personalizar:

```tex
\textbf{\huge{Título de la memoria}}\\
\vspace{30pt}
\LARGE Subtítulo de la memoria \\
```

Y también actualiza la información personal:

```tex
Asignatura: & Nombre de la asignatura\\
Estudiante: & Javier Navarro Lázaro\\
Fecha: & \today
```

### Añadiendo contenido

El contenido principal se encuentra en content.tex. Puedes editar este archivo para añadir tus capítulos, secciones y subsecciones:

```tex
\chapter{Título del capítulo}
\section{Título de la sección}
\subsection{Título de la subsección}
```

### Insertando código fuente

La plantilla incluye soporte para incluir código fuente con resaltado de sintaxis para varios lenguajes. Ejemplo:

```tex
\begin{codelisting}[style=C-color, caption=Código en C, firstnumber=1, label=lst:ejemplo]
#include <stdio.h>
int main() {
   printf("Hello, World!");
   return 0;
}
\end{codelisting}
```

Estilos disponibles:
- C-color, C++, C++-color
- Python, Python-color
- Java, Java-color
- R, R-color
- Matlab, Matlab-color
- Latex, Latex-color

## Personalización adicional

Si deseas personalizar más elementos:

- Los colores principales están definidos en defs.tex y UAL.sty
- El formato de cabeceras y pies de página se encuentra en Main.tex
- Los estilos de código están definidos en estiloscodigoprogramacion.tex

## Compilación

Esta plantilla está optimizada para compilar con pdfLaTeX. En Overleaf, puedes seleccionar este compilador en la configuración del proyecto.

## Créditos

Esta plantilla está realizada por Javier Navarro Lázaro, actual estudiante de máster de Ingeniería Informática de la Universidad de Almería. 

Se ha usado de apoyo parte de la plantilla TFG/TFM para el formato de código de Jose Manuel Requena Plens y parte de la configuración de paquetes, de la Escuela Politécnica Superior de la Universidad de Alicante.
