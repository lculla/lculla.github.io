# 18/11 — Proceso de creación del juego

Este documento registra el trabajo realizado el 18/11 para convertir la idea del juego en una primera versión web jugable. Resume el concepto, las decisiones tomadas, las iteraciones visuales, el contenido implementado y lo que queda por definir.

## Resumen

Se creó una primera versión de LITTLE TIME, un juego web de escritorio con estética pixel art. La mascota central puede realizar ocho actividades que consumen un presupuesto de 88 minutos. Al terminar la partida, se muestra un resumen de los planes realizados.

El prototipo funciona en el navegador y se ha dejado en una carpeta local separada del sitio principal. No se ha publicado en GitHub ni se ha creado nada en Figma.

## 1. Punto de partida

Se consultó la conversación de ChatGPT «Proyecto Personal» y se integraron los detalles compartidos por Lucía:

- El juego es una experiencia interactiva en la que se cuida o acompaña a una mascota.
- El tiempo disponible representa el ahorro asociado a abreviar al escribir.
- La persona decide cómo gastar ese tiempo en actividades.
- Las actividades se representan con animaciones y pequeños premios.
- No hay respuestas correctas o incorrectas.
- La partida termina cuando ya no se puede elegir otra actividad.
- El público previsto es gente joven y el dispositivo prioritario es el ordenador.
- La referencia visual elegida es pixel art.
- El nombre LITTLE TIME se usa como nombre de trabajo; falta confirmar si será el definitivo.

## 2. Flujo implementado

### Pantalla de inicio

- Presenta el título LITTLE TIME, una caja de regalo pixel art y el botón **Start**.
- Al pulsar Start, la tapa de la caja se abre y se pasa a la aparición de la mascota.

### Aparición e introducción

- Aparece una criatura provisional dibujada con formas pixeladas.
- El título de la escena es: **«¡Hola! ¿Tienes tiempo para mí?»**
- El texto introductorio actual dice: **«Hay tiempo que se queda escondido entre las palabras. El que Lucía ahorra al abreviar, hoy se ha convertido en tiempo para compartir conmigo.»**
- Se muestra un saldo inicial de **88 minutos** y se invita a entrar en la habitación.

La forma final de la mascota, el objeto del que aparece y si la introducción incluirá un chat interactivo siguen pendientes.

### Pantalla de juego

La partida se organizó en una sola escena integrada:

- El contador y la barra de tiempo están en la parte superior.
- La mascota ocupa el centro de la habitación.
- Las ocho actividades aparecen en dos columnas laterales, en orden equilibrado alrededor de la mascota.
- El fondo conserva el dormitorio cálido del diseño anterior: pared rosa con cuadrícula, suelo de madera, ventana, estantería, reloj, planta, cama y alfombra.
- Las tarjetas de actividad conservan el tratamiento anterior: formato rectangular, fondo claro, pequeño recuadro de icono, nombre, descripción y coste.
- El botón de reinicio permite volver al inicio.

Esta organización se ajustó después de que Lucía aclarara que la captura compartida era una referencia de disposición, no de estética. Se descartó el fondo azul oscuro y los botones rosas redondeados; se mantuvo la distribución integrada y se recuperaron el dormitorio y las tarjetas originales.

## 3. Actividades y costes

Los costes añadidos por Lucía en juego.md se incorporaron a la versión jugable:

| Actividad | Coste |
| --- | ---: |
| Leer | 10 min |
| Escuchar música | 3 min |
| Pintar | 5 min |
| Pescar | 20 min |
| Dormir / siesta | 10 min |
| Plantar o cuidar una planta | 15 min |
| Comer | 5 min |
| Jugar a un videojuego | 15 min |

Las actividades se pueden repetir mientras quede tiempo suficiente. Cada elección descuenta su coste, actualiza el contador y registra el plan. La mascota cambia de animación, expresa una reacción y aparece un mensaje de actividad o premio; las elecciones también se resumen durante la partida y al final.

Los costes suman 83 minutos si se realiza cada actividad una sola vez. Con el saldo inicial de 88 minutos, repetir actividades permite gastar más tiempo. Si quedan menos minutos que el coste de cualquier actividad disponible, la partida termina y el resumen muestra el tiempo que quedó sin gastar.

## 4. Resumen final

Al terminar, la pantalla final:

- Agrupa las actividades por tipo y muestra cuántas veces se realizaron.
- Muestra los minutos usados.
- Si queda un resto inferior al coste mínimo de otra actividad, lo indica en el resumen.
- Permite volver a jugar.

El texto de cierre actualizado por Lucía es:

> Has ahorrado tiempo escribiendo. Ahora tienes tiempo para vivir otras cosas.

## 5. Relación con los datos

El saldo de 88 minutos es provisional. El prototipo lo usa como presupuesto de juego fijo; todavía no calcula esa cifra a partir de las conversaciones analizadas.

Antes de afirmar que los 88 minutos son una equivalencia real, habrá que definir el periodo de análisis y un método defendible para convertir el ahorro de caracteres en tiempo. Mientras esto no se valide, la interfaz lo describe como cantidad de juego provisional.

La primera versión no importa conversaciones ni pide datos a las personas que juegan. No contiene mensajes literales de los chats.

## 6. Archivos y ejecución

El prototipo se creó como una página web estática con HTML, CSS y JavaScript, sin framework ni servidor de aplicación:

- `outputs/little-time/index.html` — estructura y textos de las pantallas.
- `outputs/little-time/style.css` — paleta, dormitorio, tarjetas, mascota, animaciones y adaptación a distintos tamaños.
- `outputs/little-time/game.js` — actividades, costes, contador, animaciones, registro de acciones y resumen final.

Vista previa local usada durante la sesión: http://localhost:8766/

La vista previa depende de que el servidor local siga activo. Los archivos del juego continúan en el espacio de trabajo de Codex y aún no se han incorporado al repositorio GitHub ni a la página principal. El estado de una partida se guarda en memoria del navegador y se reinicia al volver a jugar o recargar.

No fue necesario utilizar Figma para programar esta versión.

## 7. Estado al cerrar el trabajo del 18/11

**Implementado:**

- Pantalla Start, caja que se abre, aparición de la mascota y texto introductorio.
- Escena de juego integrada con el dormitorio cálido anterior.
- Contador de 88 minutos y barra de progreso.
- Ocho actividades con sus costes, posibilidad de repetir y animaciones de la mascota.
- Registro de actividades y resumen de final de partida.
- Texto final solicitado por Lucía.
- Diseño adaptable a pantallas pequeñas y respeto por la preferencia de movimiento reducido del sistema.

**Pendiente de definir o revisar:**

- Confirmar LITTLE TIME como nombre definitivo.
- Elegir el diseño final de la mascota y del objeto del que aparece.
- Afinar los premios y cambios que deja cada actividad en el dormitorio.
- Decidir cómo dar variabilidad a una segunda partida.
- Validar las cifras de análisis y la relación entre el ahorro real y los 88 minutos.
- Decidir si el prototipo se integrará en el sitio principal y se publicará desde GitHub.
