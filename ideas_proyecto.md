# Tres ideas de proyecto

**Autor:** Andrés Mejía  
**Fecha:** 20 de septiembre de 2026

---

## Criterios de viabilidad

Una idea es viable para esta materia si cumple los cuatro criterios:

1. Atiende un **problema concreto de mi entorno** y no solamente un tema general.
2. Tiene una **parte física fabricable** con impresión 3D, corte láser o router CNC.
3. Usa **al menos un sensor o un actuador** controlado por un microcontrolador pequeño.
4. La puede construir un **equipo de principiantes en unas ocho sesiones**, con materiales accesibles.

---

## Idea 1: Diana electrónica para practicar la precisión del saque

**Problema.** Cuando practico saque en voleibol puedo intentar dirigir el balón a una zona específica de la cancha, pero si entreno solo es difícil llevar un registro exacto de cuántos intentos realmente llegaron al objetivo. Normalmente tendría que colocar conos, mochilas u otros objetos y contar los aciertos manualmente.

**A quién le pasa.** A jugadores de voleibol que quieren mejorar la precisión de su saque, sobre todo cuando practican por su cuenta o no tienen a otra persona que registre sus resultados.

**Dónde lo he visto.** Lo he visto en las canchas donde practico voleibol, cuando se colocan objetos o se elige una zona de la cancha para intentar dirigir el saque. Al entrenar sin alguien que lleve el conteo, es fácil perder el registro de los aciertos y solamente queda una impresión general de si se está mejorando.

**Cómo funcionaría.**
- **Qué mide o detecta (sensor):** sensores piezoeléctricos o de vibración detectarían el impacto del balón sobre una o varias zonas de una diana.
- **Qué hace con eso (actuador, aviso, pantalla):** un microcontrolador registraría cada impacto válido, encendería un LED para confirmar el acierto y mostraría en una pequeña pantalla el número de intentos, aciertos y posiblemente el porcentaje de precisión.
- **Qué pieza habría que fabricar:** una carcasa para proteger los sensores y la electrónica, además de soportes impresos en 3D para fijar las zonas de impacto a una estructura ligera o a un marco.

---

## Idea 2: Medidor portátil de salto para ataque y bloqueo

**Problema.** El salto es una parte importante del ataque y el bloqueo en voleibol, pero normalmente no tengo una forma rápida de medir si mi salto está mejorando durante los entrenamientos. Sin un aparato específico, la medición termina siendo aproximada o depende de marcar una pared manualmente.

**A quién le pasa.** A jugadores de voleibol que quieren monitorear su salto vertical y no tienen acceso a equipos profesionales de medición.

**Dónde lo he visto.** Lo he visto durante entrenamientos y pruebas de voleibol en los que el alcance de ataque o bloqueo es importante, pero no siempre existe un dispositivo disponible para medir el salto de manera rápida y repetir la prueba varias veces.

**Cómo funcionaría.**
- **Qué mide o detecta (sensor):** un sensor de distancia tipo Time-of-Flight, como el VL53L1X, mediría cambios de distancia durante el salto desde una posición fija.
- **Qué hace con eso (actuador, aviso, pantalla):** el microcontrolador tomaría una medida de referencia y compararía el punto más alto detectado durante el salto. Una pantalla mostraría el resultado estimado y podría guardar el mejor intento de la sesión.
- **Qué pieza habría que fabricar:** una carcasa para el sensor y el microcontrolador, junto con un soporte ajustable impreso en 3D para mantener el sensor en una posición estable.

---

## Idea 3: Aro inteligente para entrenar pase y colocación

**Problema.** En voleibol no basta con controlar el balón; también hay que dirigirlo hacia una zona útil para el colocador o hacia un objetivo específico. Cuando entreno solo o sin un entrenador observando cada repetición, no siempre tengo una forma objetiva de saber cuántos pases o colocaciones llegaron realmente al lugar deseado.

**A quién le pasa.** A jugadores que quieren mejorar la precisión del pase de antebrazos o la colocación y necesitan repetir muchas veces el mismo gesto.

**Dónde lo he visto.** Lo he visto en ejercicios de pase y colocación donde una persona, un aro o un punto de referencia funciona como objetivo. Cuando se practica sin otra persona que evalúe cada balón, se pierde parte de la retroalimentación sobre la precisión.

**Cómo funcionaría.**
- **Qué mide o detecta (sensor):** uno o dos sensores infrarrojos colocados en el aro detectarían cuando el balón pasa correctamente por la zona objetivo.
- **Qué hace con eso (actuador, aviso, pantalla):** cada acierto encendería un LED y aumentaría un contador. Una pantalla podría mostrar aciertos consecutivos, total de intentos y mejor racha.
- **Qué pieza habría que fabricar:** un aro o marco ligero con soportes impresos en 3D para los sensores, una caja para la electrónica y un sistema sencillo para ajustar la altura.

---

## Tabla de viabilidad

| Criterio | Idea 1 | Idea 2 | Idea 3 |
|---|---|---|---|
| Problema concreto de mi entorno | Sí | Sí | Sí |
| Parte física fabricable | Sí | Sí | Sí |
| Sensor o actuador | Sí | Sí | Sí |
| Construible en ocho sesiones por principiantes | Sí | Parcial | Sí |
| Qué tan seguro estoy de lo anterior (alto / medio / bajo) | Alto | Medio | Alto |

## Mi elección

**Idea elegida:** Diana electrónica para practicar la precisión del saque.

**Por qué.** Es la idea que considero más clara y realista para construir dentro del tiempo de la materia. El problema es fácil de observar cuando se entrena saque y el funcionamiento se puede comprobar de manera directa: si el balón golpea la zona correcta, el sistema registra un acierto. También permite integrar programación, sensores, una respuesta visual y una pieza física fabricada sin necesitar un sistema demasiado complejo. Además, el prototipo se podría probar directamente con un balón de voleibol y modificar la sensibilidad de los sensores a partir de los resultados.

**Qué todavía no sé.** Necesito probar qué tipo de sensor detecta mejor un impacto de balón sin registrar demasiadas vibraciones falsas, decidir qué material debe tener la superficie de la diana para resistir los golpes y determinar qué tamaño de objetivo sería suficientemente exigente sin volver el ejercicio poco práctico. También tendría que probar si conviene usar una sola zona de impacto o varias zonas con diferente puntuación.

---

[Ir a la investigación](investigacion.md)

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT de OpenAI.
- **Qué le pedí:** Utilicé la IA como apoyo para mejorar la redacción y organización de las propuestas que yo planteé y para orientarme sobre posibles sensores, materiales y componentes que podían utilizarse para convertir las ideas en prototipos realizables.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** Las propuestas y el enfoque en voleibol fueron definidos por mí. Rechacé cambios que modificaban mis ideas sin que yo lo hubiera solicitado y adapté la redacción para que representara lo que quería desarrollar. También revisé por mi cuenta los componentes sugeridos y la información técnica antes de decidir qué conservar en el documento.
