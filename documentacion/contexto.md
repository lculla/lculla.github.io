# Contexto del proyecto

## Concepto
Proyecto web experimental sobre la **economía de mensajes**: investigar cuánto texto (y esfuerzo de escritura, entendido de forma aproximada) ahorramos al utilizar abreviaciones en WhatsApp.

El punto de partida es un gesto muy cotidiano: escribir "xq" en lugar de "porque", "q" en lugar de "que", etc. La web busca hacer visible ese ahorro y convertir los hábitos de escritura en una experiencia de exploración.

## Pregunta de partida
¿Cuánto esfuerzo de escritura me ahorro al abreviar en WhatsApp, y qué significa esa cifra en comparación con textos o tareas cotidianas?

## Objetivo
Transformar datos reales de conversaciones en una experiencia visual e interactiva que permita descubrir:
- Qué abreviaciones utiliza una persona.
- Con qué frecuencia aparecen.
- Cuántas letras/caracteres se ahorran al utilizarlas.
- Cómo se acumula ese ahorro en el conjunto de los mensajes.
- Que el usuario pueda visualizar las equivalencias de forma visual de mi ahorro.

## Material de investigación
Se han aportado tres conversaciones de WhatsApp:
- Una conversación individual con Natiss.
- Una conversación individual con Raúl.
- Una conversación grupal llamada "Les calamardes".

La autora de los mensajes que se analizan es Lucía. Es imprescindible distinguir sus mensajes de los del resto de participantes y no atribuirle mensajes ajenos.

## Datos preliminares
Un primer análisis de los archivos arrojó estos resultados provisionales para los mensajes de Lucía:
- 99.480 mensajes analizados.
- 13 abreviaciones identificadas.
- 29.466 usos contabilizados.
- 59.787 letras ahorradas estimadas.
- Proporción de abreviaciones por conversación: Natiss 8,57%; grupo 7,49%; Raúl 6,62%.

Estas cifras son una primera aproximación, no resultados definitivos. El inventario de abreviaciones puede ampliarse y es necesario revisar el contexto de formas ambiguas como "xq" y "x", así como comprobar el método de cálculo antes de publicar cifras.

## Estado actual de la web
El repositorio contiene una estructura inicial muy sencilla:
- `index.html`: título "Lo que no escribí", una frase introductoria, un botón y una pregunta desplegable.
- `script.js`: controla la aparición y ocultación de la pregunta.
- `style.css`: estilos básicos.

Texto actual de presentación: "Todo lo que me he ahorrado abreviando en whatsapp."

## Estado de las decisiones
Confirmado:
- El foco elegido por ahora es la economía de mensajes.
- La web debe priorizar la interacción y la exploración atractiva de los resultados.
- El juego de preguntas se considera secundario, no el centro de la experiencia.

Abierto:
- Cómo representar visualmente el ahorro acumulado.
- Qué comparaciones cotidianas pueden dar escala a las cifras sin resultar forzadas pero que sean divertidas y llamativas para el usuario. 
- Qué visualizaciones y formas de exploración tendrán más sentido con los datos.
- El alcance definitivo del análisis de abreviaciones y la validación de las cifras.
