# segundo-parcial-sistemas-Digitales
Chatbot creacion
https://511c54c0-1ebc-4a62-8eb9-b5f19c00e4c6-00-kghrue99axfj.spock.replit.dev/
<img width="514" height="348" alt="image" src="https://github.com/user-attachments/assets/7f779883-583d-470e-996a-e723c63cf6b7" />

1. Latch Diferencias Flip-Flop
Latch: funciona por nivel (mientras la señal está activa cambia).
Flip-Flop: funciona por flanco (solo cambia en subida o bajada del reloj).

Tipos de Latch:

SR: básico, puede ser inestable.
D: evita errores del SR (más usado).

Tipos de Flip-Flop:

SR: igual que latch pero con reloj.
D: el más usado (guarda un dato).
JK: mejora del SR (no tiene estado inválido).
T: cambia de estado (toggle).

Características Latch
Sensible a nivel (no usa reloj como tal)
Cambia mientras la señal esté activa
Más rápido pero menos estable
Puede generar errores (rebotes o cambios no deseados)
Más simple de implementar

Características Flip-Flop
Sensible a flancos (subida o bajada del reloj)
Solo cambia en un instante específico
Más estable y controlado
Ideal para circuitos secuenciales
Usa señal de reloj (clock)

en pocas palabras

Latch = rápido pero menos control
Flip-Flop = más preciso y seguro


2. Multiplexor Diferencias Demultiplexor
Multiplexor (MUX): muchas entradas igual una salida
Demultiplexor (DEMUX): una entrada igual muchas salidas

MUX 8 a 1:

8 entradas, 3 selectores
Los selectores eligen cuál entrada sale

DEMUX 1 a 8:

1 entrada, 3 selectores
La entrada se envía a una sola salida según el selector

3. Sumadores y secuenciales
Sumador medio: suma 2 bits (sin acarreo de entrada)
Sumador completo: suma 3 bits (incluye acarreo)
Circuitos secuenciales: tienen memoria (ej: flip-flops)

Qué significa que tienen memoria?

Que el circuito recuerda lo que pasó antes.

 Ejemplo:
Si un flip-flop guardó un 1, ese valor se queda ahí hasta que algo lo cambie.


Ejemplo 2

Antes: tenía guardado un 1
Ahora: llega una señal
Resultado: depende de ese 1 que ya tenía

