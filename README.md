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

 Ejemplo 1
Si un flip-flop guardó un 1, ese valor se queda ahí hasta que algo lo cambie.


Ejemplo 2

Antes: tenía guardado un 1
Ahora: llega una señal
Resultado: depende de ese 1 que ya tenía

¿Qué es un mapa de Karnaugh?
Un mapa de Karnaugh es una tabla que se usa para simplificar funciones lógicas.
Permite reducir expresiones booleanas y hacer circuitos digitales más simples, rápidos y eficientes.
donde organizar valores (0 y 1) de una función lógica para verla más fácil.

 ¿Para qué sirve?
Simplificar funciones booleanas
Reducir compuertas
Hacer circuitos más simples y rápidos
Convierte una ecuación larga y complicada en una más corta y fácil

en contexto:
Es una herramienta para simplificar circuitos digitales.

SEGUNDO PUNTO

Desarrollo de la ecuación

Ecuación original:

X = [A B' ((C + BD) + A'B')] C
 Paso 1: Expandir términos
X = A B' (C + BD + A'B') C
 Paso 2: Aplicar propiedad de C

Como todo está multiplicado por C:

X = A B' C (C + BD + A'B')
Paso 3: Simplificación

Sabemos que:

C (C + algo) = C

Entonces:

X = A B' C
 Resultado final
X = A B' C
 Forma para circuito
X = AND(A, NOT(B), C)


Tabla de verdad

Ecuación simplificada:

X = A B' C

Tabla:

A | B | C | X
--------------
0 | 0 | 0 | 0
0 | 0 | 1 | 0
0 | 1 | 0 | 0
0 | 1 | 1 | 0
1 | 0 | 0 | 0
1 | 0 | 1 | 1
1 | 1 | 0 | 0
1 | 1 | 1 | 0
 Explicación corta
La salida X solo es 1 cuando:
A = 1, B = 0 y C = 1
En cualquier otro caso es 0
 Circuito lógico (descripción)
1. Invertir B → obtener B'
2. Conectar:
   - A
   - B'
   - C
   a una compuerta AND de 3 entradas
3. La salida de la AND es X
 Diagrama (tipo texto para GitHub)
 A ----------\
              \
                 AND ------- X
               /
B -- NOT ---- 
           \
            C
   
 
Ecuación: X = A B' C
Compuertas: 1 NOT + 1 AND
Salida activa: solo en (1,0,1)

<img width="791" height="624" alt="image" src="https://github.com/user-attachments/assets/03e9d26e-1c1b-426a-8cad-4c409a38b2ee" />

<img width="672" height="627" alt="image" src="https://github.com/user-attachments/assets/9c10d7dd-ee72-4f15-bc0c-7f01fc791541" />

Preguntas del chatbot
1. ¿Qué son los semiconductores?
2. ¿Qué empresas fabrican semiconductores?
3. ¿Cómo afectan los semiconductores a la educación?
4. ¿Cuál es el futuro de los semiconductores?
   
 Variantes (para que no falle)
- semiconductores
- empresas de chips
- uso en educación
- futuro de la tecnología
- 
  Cómo funciona (lógica)
Si el usuario escribe "semiconductores" → responde definición

Si escribe "empresas" → responde Intel, NVIDIA, etc.

Si escribe "educación" → responde impacto educativo

Si escribe "futuro" → responde tendencias


