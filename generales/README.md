# Preguntas para entrevistas de Frontend
## Generales

*** Este set de preguntas generales considera preguntas abiertas a propósito. ***
*** Busca generar una conversación, más que escuchar al entrevistado dar una respuesta unitaria o exacta ***
*** La idea es que con estas preguntas pueda el entrevistado expresarse y mostrar su conocimiento de una manera relajada y con menos presión ***

### Preguntas
1. [ ] [¿Qué es lo que más te gusta de codear / programar?](#1)
1. [ ] [¿Cuál fue el último desafío técnico que tuviste?](#2)
1. [ ] [¿Cuál ha sido el desafío tecnológico más grande que has enfrentado?](#3)
1. [x] [¿Qué consideraciones tendrías que tener para hacer para que tu sitio Web tenga mejor rendimiento?](#4)
1. [ ] [¿Qué consideraciones de Seguridad, SEO, Performance, UI, UX, Tecnología, Mantenibilidad y Tamaño debes tener para hacer una Webapp?](#5)
1. [ ] [¿Cómo debugueas tu Webapp?](#6)
1. [ ] [¿Qué aprendiste esta semana?](#7)
1. [ ] [¿Cuál es tu stack de desarrollo actual?](#8)
1. [ ] [¿Cuál es tu stack de desarrollo preferido?](#9)
1. [ ] [Si tuvieras 4 hojas de estilo que tu sitio usa, ¿cómo las integrarías?](#10)
1. [ ] [Tu sitio está funcionando lento, ¿Cómo lo arreglas?](#11)
1. [ ] [¿Cómo optimizarías los assets de un sitio Web? (CSS / JS).](#12)
1. [ ] [Nombra 3 maneras de disminuir el tiempo de carga de un sitio Web (Tiempo de carga real o el percibido por el usuario).](#13)
1. [ ] [¿Cómo crearías un slideshow / carrusel de imágenes?](#14)
1. [ ] [Llegas a tu nuevo trabajo y ves que todo el codebase usa tabs, pero tú usas espacios. ¿Qué haces?](#15)
1. [ ] [¿Qué es el FOUC? (`Flash of unstyled content` o `Flash de Contenido sin Estilar`).](#16)
1. [x] [¿Qué es `ARIA` y `Screen Readers`?](#17)
1. [ ] [¿Cómo haces un sitio Web accesible?](#18)
1. [ ] [¿Cuáles son los pros y contras de usar animaciones de CSS vs animaciones de JavaScript?](#19)
1. [ ] [¿Qué es CORS?](#20)


### Respuestas
1. [¿Qué es lo que más te gusta de codear / programar?](#1)
    <div id="1" />
    ** Pregunta personal, la idea es con esto generar una conversación **

1. [¿Cuál fue el último desafío técnico que tuviste?](#2)
    <div id="2" />
    ** Pregunta personal, la idea es con esto generar una conversación **

1. [¿Cuál ha sido el desafío tecnológico más grande que has enfrentado?](#3)
    <div id="3" />
    ** Pregunta personal, la idea es con esto generar una conversación **

1. [¿Qué consideraciones tendrías que tener para hacer para que tu sitio Web tenga mejor rendimiento?](#4)
    <div id="4" />
    Existen muchas respuestas correctas, sobretodo considerando que en una entrevista no tienes 3 horas para hablar de todas las formas en que podrías mejorar el rendimiento de una aplicación.
    (Ojo, que esta pregunta no se trata de decir "Usaría google-pagespeed y seguiría las recomendaciones")

    Algunas sugerencias de temas que impactan al rendimiento:
    - Relacionado a la Red
      - Revisar la compresión de los archivos que estás descargando (¿Tu servidor los comprime previamente?)
      - ¿Está el navegador cacheando archivos que no cambiarán tan seguido?
      - ¿Estás minificando tus CSS/JS en producción?

    - Relacionado al tiempo hasta el primer renderizado
      (En esta parte influye el [critical rendering path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/))
      - ¿Estás "demorando" el parseo de archivos de JS que no son necesarios para la carga inicial de la página? [<script defer src="..." />](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)
      - ¿Estás "demorando" el parseo de archivos de JS hasta que sea absolutamente necesario? [<script async src="..." />](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)
      - ¿Estás descargando CSS necesario para el renderizado incial? ¿O todo el CSS del sitio?
      - ¿Estás dividiendo tus CSS o JS en archivos mas pequeños y manejables?
      - ¿Estás tomando en cuenta la latencia de la Red? (¿WiFi v/s 3G?)

    - JS
      - ¿Estás bloqueando el eventloop con alguna tarea demasiado larga? (Prueba usando [WebWorkers](https://developer.mozilla.org/es/docs/Web/Guide/Performance/Usando_web_workers) para esto, tienen [excelente compatibilidad](http://caniuse.com/#feat=webworkers)).
      - Estás usando o ['eval'](http://stackoverflow.com/a/86580)

    - CSS
      - Reducir la cantidad de selectores para aplicar un estilo ayuda bastante [***Cuantas menos reglas se requieran para un elemento dado, más rápida será su resolución***](https://developer.mozilla.org/es/docs/Web/CSS/Escribir_CSS_eficiente)

1. [¿Qué consideraciones de Seguridad, SEO, Performance, UI, UX, Tecnología, Mantenibilidad y Tamaño debes tener para hacer una Webapp?](#5)
    <div id="5" />

1. [¿Cómo debugueas tu Webapp?](#6)
    <div id="6" />

1. [¿Qué aprendiste esta semana?](#7)
    <div id="7" />

1. [¿Cuál es tu stack de desarrollo actual?](#8)
    <div id="8" />
    ** Pregunta personal, la idea es con esto generar una conversación **

1. [¿Cuál es tu stack de desarrollo preferido?](#9)
    <div id="9" />
    ** Pregunta personal, la idea es con esto generar una conversación **

1. [Si tuvieras 4 hojas de estilo que tu sitio usa, ¿cómo las integrarías?](#10)
    <div id="10" />

1. [Tu sitio está funcionando lento, ¿cómo lo arreglas?](#11)
    <div id="11" />

1. [¿Cómo optimizarías los assets de un sitio Web? (CSS / JS).](#12)
    <div id="12" />

1. [Nombra 3 maneras de disminuir el tiempo de carga de un sitio Web (Tiempo de carga real o el percibido por el usuario).](#13)
    <div id="13" />

1. [¿Cómo crearías un slideshow / carrusel de imágenes?](#14)
    <div id="14" />

1. [Llegas a tu nuevo trabajo, todo el codebase usa tabs pero tú usas espacios. ¿Qué haces?](#15)
    <div id="15" />

1. [¿Qué es el FOUC? (`Flash of unstyled content` o `Flash de Contenido sin Estilar`).](#16)
    <div id="16" />
    [FUOC](https://es.qwe.wiki/wiki/Flash_of_unstyled_content) Flash de contenido sin estilo

1. [¿Qué es `ARIA` y `Screen Readers`?.](#17)
    <div id="17" />

    [Aria](https://developer.mozilla.org/es/docs/Web/Accessibility/ARIA) define como crear contenido Web para personas con discapacidad, para esto usa un conjunto de atributos que se pueden agregar a las etiquetas HTML.

    [Screen readers](https://es.wikipedia.org/wiki/Lector_de_pantalla) es un software que interpreta lo que aparece en la pantalla y lo expresa con voz.

    Puedes aprender algo más de ARIA y Accesibilidad en el siguiente tutorial https://teachaccess.github.io/tutorial/

1. [¿Cómo haces un sitio Web accesible?](#18)
    <div id="18" />

1. [¿Cuáles son los pros y contras de usar animaciones de CSS vs animaciones de JavaScript?](#19)
    <div id="19" />

1. [¿Qué es CORS?](#20)
    <div id="20" />
