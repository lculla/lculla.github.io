# Registro de sesiones

Este documento recoge el trabajo realizado, las decisiones tomadas y los próximos pasos. Se actualiza al cerrar cada sesión.

## 2026-11-04 — Configuración inicial de la documentación

### Trabajo realizado
- Se revisó la estructura inicial del repositorio.
- Se confirmó que todavía no existía documentación de definición del proyecto.
- Se estableció una carpeta `documentacion/` para separar la documentación del código de la web.
- Se crearon los documentos `personalidad.md`, `contexto.md`, `criterio.md` y este registro.

### Contexto recuperado
- El foco actual del proyecto es la economía de mensajes: estudiar el ahorro asociado al uso de abreviaciones en WhatsApp.
- Se han compartido tres chats (Natiss, Raúl y el grupo "Les calamardes"). La persona cuyos mensajes se analizan es Lucía.
- Un primer análisis estimó 99.480 mensajes, 13 abreviaciones, 29.466 usos y 59.787 letras ahorradas. Son cifras provisionales, pendientes de ampliar y validar.
- La web debe priorizar la interacción y la exploración atractiva de los resultados. El juego de preguntas queda en segundo plano.

### Decisiones tomadas
- La documentación vivirá en `documentacion/`.
- Antes de cada sesión se leerán los cuatro documentos para recuperar contexto y decisiones.
- Al finalizar cada sesión se actualizará `log.md`.
- Las ideas provisionales se mantendrán diferenciadas de las decisiones confirmadas.

### Pendiente
- Revisar y completar el inventario de abreviaciones de los chats.
- Validar el criterio de cálculo del ahorro de caracteres.
- Revisar especialmente los casos ambiguos como "xq" y "x".
- Explorar maneras atractivas de visualizar y navegar los resultados acumulados.
- Definir la siguiente iteración de la experiencia web a partir de la exploración de datos.

### Estado al cerrar la sesión
Documentación inicial creada. No se han modificado `index.html`, `script.js` ni `style.css`.

## 2026-11-18 — Análisis de la documentación y registro de mensajes importantes

### Trabajo realizado
- Se revisaron los documentos de contexto, criterios, personalidad y registro del proyecto.
- Se confirmó que el repositorio de GitHub es `lculla/lculla.github.io` y que contiene este archivo.

### Preferencia de registro
- Lucía solicita que, cuando escriba la palabra «importante» en el chat, el contenido de ese mensaje se registre en este log.
- Esta regla describe una preferencia de trabajo para las conversaciones con el asistente; el registro en GitHub se realizará cuando el asistente pueda acceder al repositorio durante esa conversación.

## SESIÓN 18/11 — Diseño de la web y vista previa local

### Trabajo realizado
- Se diseñó una primera versión larga de la web «Lo que no escribí», organizada en scrolls.
- Scroll 1: portada a pantalla completa con fondo ilustrado, la frase «¿Y si todo el tiempo que ahorras escribiendo pudieras utilizarlo para vivir otras cosas?» y el botón «Descubre más...» con flecha hacia abajo.
- Scroll 2: pregunta de investigación en mayúsculas: «¿CUÁNTO TIEMPO ME AHORRO AL ABREVIAR EN WHATSAPP, Y EN QUÉ PODRÍA IMPLEMENTAR ESTE TIEMPO?». Se recolocó al principio del scroll y se redujo su altura para que solo ocupe el contenido de la pregunta y la animación.
- Bajo la pregunta se añadió una animación de bocadillos de chat. Los mensajes aparecen escalonados y se desvanecen. Incluye «q tal?», «xq no?», «q haces?», «xq llegas?», «y q?», «xq?», «xfaaa», «m gusta» y «sii tbb». La nota aclaratoria visible bajo la animación se eliminó a petición de Lucía.
- Scrolls siguientes: ahorro estimado de 59.787 caracteres; resumen de 99.480 mensajes, 29.466 usos y 13 abreviaciones; comparación interactiva por conversación; criterios de validación pendientes; y cierre que explica que el tiempo ahorrado aún no está calculado.
- Comparación preliminar de mensajes de Lucía con abreviaciones: Natiss 8,57%; Les calamardes 7,49%; Raúl 6,62%.
- Se conservaron avisos de que las cifras son preliminares y no se inventaron equivalencias de caracteres a tiempo.

### Vista previa local y archivos
- URL local para abrir la web: http://localhost:8765/
- Enlace directo al segundo scroll y a la animación: http://localhost:8765/#pregunta
- Archivo actual del prototipo en el espacio de trabajo de Codex: `work/preview/index.html`.
- El servidor local se inició en el puerto 8765 con `ruby -run -e httpd work/preview -p 8765`. Es una vista previa local de esta sesión, no un sitio publicado; la URL localhost solo está disponible mientras el servidor siga ejecutándose en el equipo.
- El prototipo está en el espacio de trabajo local y todavía no se ha integrado en el `index.html` del repositorio.

### Próximos pasos
- Revisar la secuencia completa y editar cada scroll según los comentarios de Lucía.
- Validar el inventario real de abreviaciones antes de presentar los bocadillos como ejemplos extraídos de los chats.
- Validar el cálculo de caracteres ahorrados y determinar si existe una forma defendible de estimar el tiempo.

### Prototipo guardado en GitHub
- Para conservar la web al cerrar el chat, se guardó el prototipo completo en `prototipos/lo-que-no-escribi-preview.html` en la rama `main`.
- Archivo: https://github.com/lculla/lculla.github.io/blob/main/prototipos/lo-que-no-escribi-preview.html
- Este archivo conserva los scrolls y la animación actual. Es una copia de prototipo; no sustituye la página principal `index.html` ni cambia la publicación principal.
- La vista previa interactiva local sigue en http://localhost:8765/ mientras el servidor permanezca activo. Si el servidor se detiene, se puede volver a servir el archivo guardado desde la carpeta local del proyecto al descargarlo de GitHub.

### Ajuste posterior — cursiva en la cifra acumulada
- A petición de Lucía, la frase «letras que no llegué a escribir» aparece en cursiva bajo la cifra 59.787.
- El cambio se aplicó tanto a la vista previa local como al prototipo guardado en GitHub: `prototipos/lo-que-no-escribi-preview.html`.
- La vista previa local continúa en http://localhost:8765/ mientras el servidor siga activo.

## 2026-11-18 — Documento inicial de la idea del juego

### Trabajo realizado
- Se creó `documentacion/juego.md` como documento vivo para definir la futura experiencia web interactiva basada en los datos del proyecto.
- Se incorporaron el contexto, los objetivos, las cifras preliminares y los criterios de rigor ya documentados.
- Se dejaron las mecánicas, el recorrido, el público y el alcance como decisiones pendientes para completarlos con Lucía, sin inventar reglas del juego.

### Próximo paso
- Recoger la idea concreta de Lucía sobre cómo se juega y completar el documento antes de analizar y programar la experiencia.

## 2026-11-18 — Ampliación del concepto del juego

### Trabajo realizado
- Se revisó la conversación de ChatGPT «Proyecto Personal» y se incorporaron a `documentacion/juego.md` los detalles disponibles sobre el juego, junto con las respuestas de Lucía en esta conversación.
- Se documentó el inicio con Start, la aparición de la mascota, el presupuesto de 88 minutos, las actividades, el final con recopilación de acciones, el público joven y el estilo pixel art.
- Se separaron las ideas por confirmar de las decisiones expresadas por Lucía. Se señaló que la equivalencia entre los 88 minutos y el ahorro real todavía necesita método y periodo de referencia.
- Se añadió como posibilidad futura un modo de datos propios procesado localmente, sin convertirlo en requisito de la primera versión.

### Próximos pasos
- Confirmar el título, definir la mascota y escenario, completar las ocho actividades y establecer la relación verificable entre los datos y el tiempo de juego.


## 2026-11-18 — Registro del desarrollo de LITTLE TIME

### Trabajo realizado
- Se creó `documentacion/Procesojuego.md` para dejar registrado el proceso completo de la primera versión del juego, desde la idea hasta la disposición final de la partida.
- El documento recoge el flujo Start → aparición de la mascota → habitación de juego → resumen, los costes de las ocho actividades, las iteraciones visuales, los textos finales y las cuestiones todavía abiertas.
- Se dejó constancia de que el prototipo se implementó como HTML, CSS y JavaScript en `outputs/little-time/`, está disponible mediante vista previa local y aún no se ha publicado ni integrado en la página principal del repositorio.
- Se registró que los 88 minutos son una cantidad provisional y que su equivalencia con el ahorro real todavía no está validada.

### Documento de proceso
- `documentacion/Procesojuego.md`

## SESIÓN 22/11 — Respaldo del HTML y referencias visuales

### Estado guardado
- Se conserva el prototipo actual como HTML autónomo en el espacio de trabajo: `outputs/lo-que-no-escribi.html`.
- Se actualizó también el respaldo permanente en GitHub: `prototipos/lo-que-no-escribi-preview.html` (rama `main`). La página principal `index.html` no se ha reemplazado.
- Vista previa privada en este equipo: http://localhost:8765/lo-que-no-escribi.html. El servidor local debe seguir activo para que el enlace funcione; el HTML guardado puede abrirse directamente en un navegador.
- El prototipo incluye los scrolls ya diseñados, la animación de mensajes abreviados y el texto «letras que no llegué a escribir» en cursiva.

### Referencias visuales recibidas
- Se recibieron cuatro imágenes como referencias para el siguiente trabajo visual: `DONT EDIT OR REPOST.jpeg`, `_ (26).jpeg`, `_ (27).jpeg` y `concept text.jpeg`, ubicadas en la carpeta Descargas de Lucía.
- Las imágenes quedan anotadas como referencias visuales para retomar el diseño; aún no se han incorporado al HTML.
- Registro solicitado con el título «22/11» y completado el 23/11/2026.

## SESIÓN 23/11 — Fichas giratorias y equivalencias

### Trabajo realizado
- Las tres fichas de equivalencia de la penúltima pantalla ahora giran al pasar el cursor. También se pueden abrir y cerrar con toque o botón, para funcionar en pantallas táctiles.
- En la ficha de cine se muestra una combinación exacta: `Barbie` (1 h 54 min) + `Spider-Man: Across the Spider-Verse` (2 h 20 min) + 1 h 00 min 53 s de otra película = 5 h 14 min 53 s. Se enlazan las fichas de duración de Netflix y Disney+.
- En la ficha musical: 89 canciones de 3 min 30 s + 3 min 23 s de la canción 90 = 5 h 14 min 53 s. La referencia de 3:30 es «BIRDS OF A FEATHER» de Billie Eilish y se enlaza Spotify.
- En la ficha de clases: 6 clases de 50 min + 14 min 53 s de la siguiente = 5 h 14 min 53 s. La duración de 50 minutos está marcada explícitamente como una suposición.
- Las equivalencias están presentadas como aproximaciones para explorar y se aclara que se pueden redefinir.

### Archivos y vista previa
- HTML actualizado: `outputs/lo-que-no-escribi-v2.html` en el espacio de trabajo local.
- Host privado local: http://localhost:8765/lo-que-no-escribi-v2.html#equivalencias
- La página actual es la versión local descargable; no se ha publicado como web pública.
- Registro añadido el 23/11/2026.
