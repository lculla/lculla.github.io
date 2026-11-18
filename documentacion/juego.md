# Juego — idea y definición

> Documento vivo para definir una experiencia web interactiva basada en los datos del proyecto. Las decisiones confirmadas se separan de las ideas propuestas y de las cuestiones pendientes.

## 1. Idea general

Una mascota de pixel art convierte en tiempo para jugar el tiempo que Lucía ahorra al abreviar en WhatsApp. Quien juega decide cómo gastarlo en actividades para cuidar y entretener a la mascota; cuando se agota, ve reunido todo lo que hizo.

La experiencia debe ser entretenida y, al mismo tiempo, ayudar a entender que pequeñas abreviaciones pueden acumular un ahorro.

**Nombre de trabajo visto en otra conversación:** LITTLE TIME. Pendiente de confirmar como título definitivo.

## 2. Objetivo de la experiencia

- Mostrar cuánto tiempo ahorra Lucía al escribir con abreviaciones en un periodo que todavía hay que definir.
- Dejar que la persona decida en qué actividades gastar ese tiempo dentro del juego.
- Cuidar o acompañar a una mascota mediante acciones sencillas y animadas.
- Al final, reunir visualmente las acciones realizadas y hacer visible el uso del tiempo ahorrado.
- Ofrecer una experiencia amable, entretenida y sin respuestas correctas o incorrectas.

## 3. Público y formato

- **Público previsto:** gente joven.
- **Dispositivo principal:** ordenador.
- **Estética de referencia:** pixel art.
- **Formato:** comienza con unas pantallas de introducción; después, el juego principal transcurre en una misma pantalla.
- **Tono:** cercano, lúdico y curioso, siguiendo personalidad.md.

## 4. Recorrido del juego

### Inicio

1. La persona ve un botón **Start**.
2. Al pulsarlo, aparece una caja, un huevo u otro objeto por decidir.
3. El objeto se abre y aparece por primera vez la mascota.
4. Una introducción breve explica de forma indirecta que el tiempo disponible procede del tiempo que Lucía ahorra al abreviar. El texto exacto está pendiente.

En otra conversación se exploró introducir el concepto mediante un chat ficticio entre dos personas que hablan de un juego nuevo y usan abreviaciones. También se propuso resaltar las abreviaciones y revelar su significado al pulsarlas. Es una propuesta para la introducción, no una decisión cerrada.

### Juego principal

1. Se muestra un contador o presupuesto de tiempo disponible.
2. La persona elige una actividad para la mascota.
3. La actividad consume una cantidad de ese tiempo.
4. La mascota realiza la actividad mediante una animación y obtiene algún premio, objeto o cambio visual.
5. La persona puede seguir eligiendo actividades mientras le quede tiempo.

La actividad no tiene aciertos ni fallos. El reto consiste en decidir cómo gastar el tiempo y cuidar o entretener a la mascota hasta agotarlo.

### Final

Cuando el tiempo llega a cero, se muestra una recopilación de las actividades realizadas. La forma visual del resumen y el mensaje final están pendientes de diseñar.

Se podrá volver a jugar, aunque la variabilidad entre partidas aún no está definida.

## 5. Tiempo disponible y relación con los datos

En el diseño actual se ha planteado empezar con **88 minutos** para gastar. El tiempo funciona como el recurso o moneda del juego: cada actividad tiene un coste y reduce el saldo disponible.

La cifra de 88 minutos es una cantidad planteada para el juego, pero todavía no está documentado cómo se calcula a partir del ahorro real de Lucía. Antes de presentarla como equivalencia exacta, hay que definir:

- A qué periodo de conversaciones corresponde (por ejemplo, un día, una semana o todo el conjunto analizado).
- Cómo se transforma el ahorro de caracteres en minutos.
- Si el saldo inicial será siempre fijo o cambiará al elegir otro periodo o conjunto de datos.
- Cómo se explicará la estimación para que no parezca una medición exacta si no lo es.

Hasta validar esa relación, el juego debe describir los 88 minutos como una cantidad de diseño o una estimación, no como un resultado demostrado.

## 6. Actividades y recompensas

Se han mencionado actividades como:

- Comer.
- Pintar o dibujar.
- Pescar.
- Plantar o cuidar una planta.
- Dormir.
- Escuchar música.
- Jugar a un videojuego.

Se había planteado contar con **ocho actividades** en total. La lista definitiva, el coste de cada actividad y los premios o cambios que desbloquea siguen pendientes de confirmar.

Cada actividad debería especificar:

| Elemento | Definición pendiente |
| --- | --- |
| Nombre y acción | Qué hace la mascota |
| Coste | Cuántos minutos consume |
| Animación | Qué ocurre en pantalla |
| Premio o cambio | Qué aparece, se consigue o cambia después |
| Repetición | Si se puede elegir varias veces |

## 7. Mascota y espacio

- **Mascota:** puede ser un personaje, un animalito o una forma abstracta. El diseño concreto sigue abierto.
- **Aparición inicial:** sale de una caja, un huevo u otro objeto al comenzar.
- **Espacio de juego:** pendiente de definir (por ejemplo, una habitación, un jardín o un escenario que evoluciona).
- **Premios y cambios visuales:** se quiere que las actividades dejen una huella visible, pero falta especificar cuáles y si se conservan en la partida.
- **Estilo:** pixel art.

## 8. Datos disponibles y rigor

El proyecto analiza los mensajes escritos por Lucía en tres conversaciones: Natiss, Raúl y el grupo «Les calamardes».

Cifras preliminares documentadas:

- 99.480 mensajes analizados.
- 13 abreviaciones identificadas.
- 29.466 usos contabilizados.
- 59.787 letras ahorradas estimadas.
- Porcentaje preliminar de mensajes con abreviaciones: Natiss 8,57 %, Les calamardes 7,49 % y Raúl 6,62 %.

Estas cifras siguen pendientes de validación. Hay que revisar el inventario, el contexto de formas ambiguas como «xq» y «x» y el método de cálculo. El periodo exacto que abarcan los datos también debe quedar claro si se utilizará para calcular el saldo del juego.

## 9. Datos de Lucía y posible modo para otras personas

La primera versión puede utilizar los datos de Lucía, sin pedir información a quien juega. Así cualquier persona puede probar la experiencia de inmediato y el juego puede explicar que el tiempo representa el ahorro de Lucía.

Como posible ampliación, se podría permitir que cada persona pegue o cargue una exportación de su propio chat y calcular el resultado en el navegador. Para que sea comprensible y respetuoso con la privacidad, esa opción requeriría:

- Procesar el archivo localmente en el dispositivo, sin subir la conversación a un servidor.
- Identificar solo los mensajes escritos por la persona usuaria.
- Explicar qué datos se analizan y permitir borrarlos al terminar.
- Avisar que el resultado es una estimación y depende de las abreviaciones reconocidas.

Este modo es una idea futura, no parte confirmada de la primera versión. Una opción más sencilla sería dejar que la persona introduzca o pegue solo sus propios textos, en lugar de importar una conversación completa.

## 10. Primera versión

**Elementos indicados como imprescindibles en la primera pantalla:**

- La mascota o personaje.
- El botón **Start**.

**Para que la partida pueda jugarse también habrá que definir e incluir:**

- La breve introducción.
- El saldo inicial de tiempo y su explicación.
- Las ocho actividades o la selección inicial que se acuerde.
- El coste y la animación de cada actividad.
- El estado final y la recopilación de acciones.

La prioridad y el alcance exacto de esta primera versión todavía deben cerrarse.

## 11. Contenido y privacidad

En la introducción se ha explorado una conversación ficticia que explique el concepto con naturalidad y que pueda incluir abreviaciones del análisis. No se ha confirmado que se vayan a mostrar fragmentos literales de chats personales.

Antes de incluir mensajes reales, habrá que acordar qué se puede mostrar y cómo anonimizarlo. La experiencia no debe atribuir a Lucía mensajes escritos por otras personas.

## 12. Decisiones pendientes

- Confirmar si el título será **LITTLE TIME**.
- Elegir el aspecto de la mascota y el objeto del que aparece.
- Definir el escenario donde transcurre la partida.
- Escribir el texto introductorio y decidir si incluirá el chat ficticio interactivo.
- Aclarar qué representa exactamente el saldo de 88 minutos y qué periodo de datos utiliza.
- Definir las ocho actividades, sus costes, animaciones y recompensas.
- Decidir cómo se comportan las actividades cuando queda menos tiempo que su coste.
- Diseñar el resumen final y qué muestra además de la lista de acciones.
- Decidir qué aporta una segunda partida y cómo dar variedad.
- Confirmar si se usarán solo los datos de Lucía o si se explorará más adelante un modo para datos propios.
- Validar las cifras y el método antes de afirmar una equivalencia exacta entre abreviaciones y minutos.

## 13. Criterios para considerar la idea lista para programar

Antes de programar, el documento debe dejar claro:

- El recorrido desde **Start** hasta el resumen final.
- Cómo funciona el saldo de tiempo y cómo se relaciona con los datos.
- La lista de actividades, sus costes y sus respuestas visuales.
- El aspecto y el espacio de la mascota, aunque sea mediante una referencia inicial.
- Qué se considera imprescindible para la primera versión.
- Qué datos y mensajes se mostrarán, con qué nivel de privacidad y qué grado de certeza.
