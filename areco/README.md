# Guía de Uso - Proyecto con SASS

Este archivo tiene como objetivo proporcionar una guía general para trabajar con proyectos que utilizan preprocesadores CSS como SASS (Syntactically Awesome Style Sheets). Como ejemplo, utilizaremos un proyecto que contiene una página web con planes de hosting y sus respectivos estilos, y que usa SASS para la creación de los estilos.

## ¿Qué es SASS?

SASS es un preprocesador CSS que permite escribir código CSS de manera más eficiente y estructurada. Con SASS, podemos usar características como variables, anidamiento de reglas, mixins, entre otras, para hacer que nuestro código sea más limpio y reutilizable.

### Características clave de SASS:
- **Variables**: Permiten almacenar valores como colores, tamaños y fuentes para reutilizarlos en todo el proyecto.
- **Anidamiento**: Nos permite anidar las reglas de CSS dentro de otras reglas para una estructura más clara.
- **Mixins y funciones**: Facilitan la reutilización de bloques de código y cálculos.

## Estructura General del Proyecto

Aquí te mostramos la estructura del proyecto:


### Archivos principales:

1. **`arecoplanes.html`**: Archivo HTML que contiene la estructura de la página web, en este caso, los planes de hosting.
2. **`arecoplanes.scss`**: Archivo SCSS donde están definidos los estilos, utilizando variables, anidamiento y otros conceptos de SASS.
3. **`arecoplanes.css`**: Archivo CSS generado después de compilar el archivo SCSS. Este es el archivo que se utiliza en la página web.

## Pasos para Trabajar con SASS

### 1. Instalación de Herramientas

Para compilar los archivos SASS a CSS, necesitas tener instalados Node.js, npm y SASS. Aquí te mostramos cómo instalarlos en Linux y Windows.

#### En Linux:

1. **Instalar Node.js y npm** (si aún no están instalados):

   ```bash
   sudo apt update
   sudo apt install nodejs npm

Instalar SASS:

    sudo npm install -g sass

En Windows:

    Instalar Node.js y npm:

        Dirígete a Node.js y descarga la última versión estable.

        Sigue las instrucciones del instalador.

    Instalar SASS:

    Abre la terminal y ejecuta:

    npm install -g sass

2. Compilación de SCSS a CSS

En nuestro ejemplo, el archivo SCSS principal es arecoplanes.scss, el cual debe ser compilado para generar el archivo CSS correspondiente. Para hacerlo, seguimos estos pasos:
En Linux:

    Navega al directorio scss donde está el archivo arecoplanes.scss:

cd /var/www/html/tarea3/areco/scss

Ejecuta el siguiente comando para compilar el archivo SCSS:

    sass arecoplanes.scss ../arecoplanes.css

    Esto generará el archivo arecoplanes.css en el directorio principal del proyecto.

En Windows:

    Abre la terminal en el directorio donde se encuentra el archivo arecoplanes.scss.

    Ejecuta el siguiente comando para compilar el archivo SCSS:

    sass arecoplanes.scss ..\arecoplanes.css

    Esto generará el archivo arecoplanes.css en la raíz del proyecto.
