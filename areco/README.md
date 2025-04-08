Guía de Uso para SCSS
Introducción a SCSS

SCSS (Sassy CSS) es una extensión de CSS que agrega funcionalidades adicionales como variables, anidamiento de reglas, mixins, funciones y herencia. Estas características permiten escribir código CSS más organizado, reutilizable y eficiente.
Beneficios de SCSS:

    Variables: Guarda valores reutilizables (colores, tamaños, etc.) que pueden ser usados en todo el archivo.

    Anidamiento: Permite escribir reglas dentro de otras, reflejando la estructura HTML, lo que mejora la legibilidad.

    Mixins: Define bloques de código reutilizables que pueden ser incluidos en cualquier parte.

    Operaciones matemáticas: Puedes realizar operaciones dentro de SCSS (suma, resta, multiplicación, etc.) para trabajar dinámicamente con tamaños y valores.

Instalación de Herramientas

Antes de empezar a escribir y compilar SCSS, necesitas instalar algunas herramientas esenciales: Node.js, npm y SASS. Aquí te dejo los pasos para instalar en Linux y Windows.
1. Instalación en Linux

    Instalar Node.js y npm:

sudo apt update
sudo apt install nodejs npm

Instalar SASS (usando npm):

    sudo npm install -g sass

2. Instalación en Windows

    Instalar Node.js:

        Ve a Node.js y descarga la última versión estable. Luego, sigue las instrucciones del instalador.

    Instalar SASS:

    Abre el terminal y ejecuta el siguiente comando:

    npm install -g sass

Estructura del Proyecto

La estructura básica de un proyecto SCSS puede ser algo como esto:

mi-proyecto/
├── index.html                # Archivo HTML
├── css/
│   └── estilos.css           # Archivo CSS generado
├── scss/
│   └── estilo.scss           # Archivo SCSS
└── README.md                 # Guía del proyecto

Archivos principales:

    index.html: Contiene el contenido de la página web.

    estilos.scss: El archivo principal donde se escriben los estilos SCSS.

    estilos.css: El archivo CSS generado después de compilar SCSS. Este es el archivo que se incluye en la página HTML.

Compilación de SCSS a CSS

Una de las tareas más importantes al trabajar con SCSS es compilar los archivos SCSS a CSS, ya que los navegadores solo entienden CSS. Existen diferentes maneras de hacer esto, y aquí te explico cómo hacerlo de manera manual y automática.
Compilación Manual

    Accede al directorio donde está el archivo SCSS. Abre la terminal y navega al directorio que contiene el archivo estilo.scss.

    Ejecuta el siguiente comando para compilar SCSS a CSS:

    sass scss/estilo.scss css/estilos.css

    Este comando convierte el archivo estilo.scss en estilos.css en la carpeta css/.

Compilación Automática

Para automatizar la compilación de SCSS cada vez que guardas el archivo, usa el siguiente comando. Esto hará que SCSS se compile automáticamente cada vez que haya cambios:

sass --watch scss/estilo.scss:css/estilos.css

Esto asegura que siempre que guardes cambios en estilo.scss, el archivo estilos.css se actualice en consecuencia.
