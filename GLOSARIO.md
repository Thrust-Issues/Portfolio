# Glosario — términos que mencioné (explicado sin jerga)

No necesitas saber programar para entender esto. Cada término está explicado en una oración simple, con un ejemplo de por qué importa para tu portafolio.

## Lo básico del sitio

**HTML** — el "esqueleto" de la página: el texto, las secciones, las imágenes. Es lo que hace que el navegador sepa "aquí va un título, aquí va un párrafo, aquí va una foto".

**CSS** — el "vestuario": colores, tamaños, espaciados, animaciones. Todo lo que hace que tu sitio se vea con la estética verde/terminal en vez de texto negro plano.

**JS (JavaScript)** — el "comportamiento": lo que hace que las cosas reaccionen cuando haces click, como abrir la foto en grande o cambiar de pestaña en la galería.

**Un solo archivo (`index.html`)** — tu sitio entero (HTML + CSS + JS) vive en un solo documento, en vez de estar repartido en varios archivos. Ventaja: fácil de subir y entender. Desventaja: si crece mucho, se vuelve largo de scrollear.

## Cómo te encuentra la gente (SEO)

**SEO** (Search Engine Optimization) — todo lo que ayuda a que Google (u otros buscadores) muestren tu sitio cuando alguien busca tu nombre o "portafolio ingeniería mecánica UPRM".

**Meta tags** — información "invisible" en la página que no se ve al mirarla, pero que Google y otras webs sí leen. Por ejemplo, una descripción corta de quién eres, que aparece debajo del link en resultados de búsqueda.

**Open Graph / Twitter Card** — son meta tags especiales que le dicen a LinkedIn, WhatsApp o Twitter/X qué imagen, título y descripción mostrar cuando alguien pega el link de tu portafolio en un mensaje o post. Sin esto, se ve como un link pelado o con una vista previa fea.

**Favicon** — el iconito pequeño que aparece en la pestaña del navegador (al lado del título). Ahora mismo tu sitio no tiene uno, así que sale un ícono genérico.

**`alt` (texto alternativo)** — una descripción de texto que se le pone a cada imagen, para que (a) Google entienda qué muestra la foto y (b) las personas con discapacidad visual que usan lectores de pantalla sepan qué hay ahí aunque no puedan verla.

**`sitemap.xml` / `robots.txt`** — dos archivos pequeños que le dicen a Google "estas son todas las páginas de mi sitio" y "puedes/no puedes indexar esto". Ayudan a que te encuentren más rápido en buscadores.

## Velocidad (rendimiento)

**Rendimiento** — qué tan rápido carga tu sitio. Importa porque si tarda mucho, la gente se va antes de verlo (especialmente reclutadores revisando muchos portafolios).

**Lazy loading** ("carga perezosa") — en vez de cargar TODAS las fotos de tu galería apenas alguien entra al sitio, solo carga las que están a la vista y va cargando el resto según la persona hace scroll. Ahorra datos y tiempo de carga, sobre todo cuando tengas muchas fotos de CAD/renders.

**Comprimir / WebP** — reducir el tamaño de archivo de una imagen sin que se vea peor. Una foto de SolidWorks exportada como PNG puede pesar 2-5 MB; comprimida o en formato WebP puede pesar 200-500 KB, cargando mucho más rápido.

**Canvas** — un "lienzo" donde JavaScript dibuja gráficos en tiempo real. Lo uso para el efecto de "lluvia digital" (estilo Matrix) que se ve de fondo en tu sitio.

**`setInterval`** — una instrucción que repite algo cada cierto tiempo (en tu caso, redibuja la lluvia digital 60 veces por segundo). El problema es que sigue corriendo aunque tengas la pestaña minimizada, gastando batería sin necesidad.

## Accesibilidad

**Accesibilidad** — que tu sitio se pueda usar bien sin importar las capacidades de quien lo visita: gente con baja visión, que no puede usar el mouse, que tiene el movimiento reducido activado, etc. Además de ser lo correcto, Google también valora esto para el SEO.

**Contraste (WCAG AA)** — WCAG es el estándar internacional de accesibilidad web; "AA" es un nivel de cumplimiento. El contraste mide qué tan fácil es leer texto claro sobre fondo oscuro (o viceversa). Si el contraste es muy bajo, el texto se ve "lavado" y cuesta leerlo, sobre todo con brillo de pantalla alto o luz de sol.

**`prefers-reduced-motion`** — una preferencia que la persona activa en su computadora/teléfono cuando le marean o incomodan las animaciones. Tu sitio ya respeta esto para la intro, pero no para el fondo animado — hay que arreglarlo para que también se apague ahí.

**Lightbox** — la ventana que aparece cuando haces click en una foto de la galería y se agranda sobre un fondo oscuro. Ahora mismo solo se puede cerrar con click; falta que también se pueda cerrar con la tecla `Esc` (accesibilidad de teclado).

## Funcionalidad adicional

**Formulario de contacto (Formspree/Getform)** — servicios gratuitos/baratos que reciben los datos de un formulario web y te los envían por email, sin que tengas que programar un servidor. Alternativa a que la persona tenga que abrir su propio correo con el link `mailto:`.

**Analytics (Plausible / Google Analytics)** — una herramienta que cuenta cuántas personas visitan tu sitio, desde dónde (LinkedIn, Google, directo) y qué páginas ven. Te dejaría saber, por ejemplo, si un reclutador visitó tu sitio después de que le mandaste tu resume.

---

Si quieres, puedo implementar cualquiera de estos cambios directamente en `index.html` — dime cuáles te interesan y los explico paso a paso mientras los hago, o simplemente los hago y te digo qué cambió.
