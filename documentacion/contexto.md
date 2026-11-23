# Contexto del proyecto

## Concepto
Proyecto web experimental sobre la **economía de mensajes**: investigar cuánto texto (y esfuerzo de escritura, entendido de forma aproximada) ahorramos al utilizar abreviaciones en WhatsApp.

El punto de partida es un gesto muy cotidiano: escribir "xq" en lugar de "porque", "q" en lugar de "que", etc. La web busca hacer visible ese ahorro y convertir los hábitos de escritura en una experiencia de exploración.

## Pregunta de partida
¿CUÁNTO TIEMPO ME AHORRO AL ABREVIAR EN WHATSAPP, Y EN QUÉ PODRÍA IMPLEMENTAR ESTE TIEMPO?

## Objetivo
Transformar datos reales de conversaciones en una experiencia visual e interactiva que permita descubrir:
- Qué abreviaciones utiliza una persona.
- Con qué frecuencia aparecen.
- Cuántas letras/caracteres se ahorran al utilizarlas.
- Cómo se acumula ese ahorro en el conjunto de los mensajes.
- Que el usuario pueda visualizar las equivalencias de forma visual de mi ahorro.

## Los datos:

Material de investigación
Se han aportado tres conversaciones de WhatsApp:
- Una conversación individual con Natiss.
- Una conversación individual con Raúl.
- Una conversación grupal llamada "Les calamardes".

- Se han leído los mensajes de las tres conversaciones.
- Se han separado los mensajes según quién los envía.
- Se han seleccionado exclusivamente los mensajes escritos por Lucía.
- Se han unido las líneas de los mensajes que ocupaban más de una línea.
- Se han excluido los mensajes de los demás participantes y las notificaciones del sistema.

La autora de los mensajes que se analizan es Lucía. Es imprescindible distinguir sus mensajes de los del resto de participantes y no atribuirle mensajes ajenos.

Datos preliminares
Un primer análisis de los archivos arrojó estos resultados provisionales para los mensajes de Lucía:
- 99.443 mensajes escritos por Lucía.
- 13 abreviaciones identificadas.
- 29.466 usos contabilizados.
- 62.975 caracteres ahorrados estimadas, aprox 49 al día.
- 2.099.653 carácteres escritos en total.
- 1.286 días de periodo analizado.
- 77,3 mensajes diarios de media. 
- Proporción de abreviaciones por conversación: Natiss 8,57% (23.900 mensajes de Lucía = 452.824 caracteres) ; grupo 7,49% (29.479 mensajes de Lucía = 632.915 caracteres); Raúl 6,62% (99.443 mensajes de Lucía = 2.099.653 caracteres).

Cómo se calcula la media diaria:
\[99.443 \div 1.286 = 77,33\]
Por tanto, has enviado una media de 77 mensajes al día en las tres conversaciones analizadas.

Estas cifras son una primera aproximación, no resultados definitivos. El inventario de abreviaciones puede ampliarse y es necesario revisar el contexto de formas ambiguas como "xq" y "x", así como comprobar el método de cálculo antes de publicar cifras.

Análisis abreviaciones:
Se seleccionan 13 abreviaciones habituales de mi manera de escribir y se buscan cuántas veces aparecía cada una en mis mensajes.
Criterio: 
- Se buscaron palabras completas, no letras que apareciesen dentro de otras palabras.
- La búsqueda no distinguió entre mayúsculas y minúsculas.
- Se comparó cada abreviación con su forma desarrollada.
- Se calculó cuántos caracteres se ahorraban en cada uso.

q (que) - 14.781 usos , 2 caracteres ahorrados por uso
m (me) - 2.414 usos , 1 caracter ahorrado por uso
esq (es que) - 2.176 usos , 3 caracteres ahorrados por uso
t (te) - 1.753 usos , 1 caracter ahorrado por uso
xq (porque) - 1.611 usos , 4 caracteres ahorrados por uso
x (por) - 1.426 usos , 2 caracteres ahorrados por uso
ns (no sé) - 1.121 usos , 3 caracteres ahorrados por uso
d (de) - 1.191 usos , 1 caracter ahorrado por uso
n (en) - 1.044 usos , 1 caracter ahorrado por uso
tb (también) - 894 usos , 5 caracteres ahorrados por uso
vd (verdad) - 681 usos , 4 caracteres ahorrados por uso
qn (quién) - 168 usos , 3 caracteres ahorrados por uso
xra (para) - 126 usos , 1 caracter ahorrado por uso

- 29.386 abreviaciones en total.
- 22,85 abreviaciones diarias de media.
- Aproximadamente una abreviación cada 3,4 mensajes.
- La abreviación más utilizada es «q», con 14.781 apariciones, presenta el 50,3%

Para calcularla multiplicamos el número de usos de cada abreviación por la diferencia entre la longitud de la expresión completa y la abreviación.

Por ejemplo:
- «q» se utiliza 14.781 veces.
- «que» tiene 3 caracteres y «q» tiene 1.
- Cada uso ahorra 2 caracteres.
- 14.781 × 2 = 29.562 caracteres ahorrados.
Repetimos la operación con las 13 abreviaciones.

De caracteres a tiempo:
Para convertir los caracteres ahorrados en tiempo necesitamos establecer una velocidad de escritura. Hemos decidido utilizar 200 caracteres por minuto como velocidad de referencia. \[\text{Tiempo (minutos)} =\frac{\text{Caracteres ahorrados}}{200}\]

## Estado actual de la web
El repositorio contiene una estructura inicial muy sencilla:
- `index.html`: título "Lo que no escribí", una frase introductoria, un botón y una pregunta desplegable.
- `script.js`: controla la aparición y ocultación de la pregunta.
- `style.css`: estilos básicos.

Texto actual de presentación: "Todo lo que me he ahorrado abreviando en whatsapp."

## Tono
- Juvenil, llamativo, colorido, atractivo a la vista, genera mucha curiosidad y ganas de interactuar.

## Estado de las decisiones
Confirmado:
- El foco elegido por ahora es la economía de mensajes.
- La web debe priorizar la interacción y la exploración atractiva de los resultados.
- El juego de preguntas se considera secundario, no el centro de la experiencia.
- Experimentación estética
- Datos visualizados
Falta:
- Cómo representar visualmente el ahorro acumulado.
- Qué comparaciones cotidianas pueden dar escala a las cifras sin resultar forzadas pero que sean divertidas y llamativas para el usuario. 
- Qué visualizaciones y formas de exploración tendrán más sentido con los datos.
- El alcance definitivo del análisis de abreviaciones y la validación de las cifras.
