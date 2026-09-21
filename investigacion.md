# Investigación: ¿esto ya existe? ¿quién lo dice?

**Autor:** Andrés Mejía  
**Fecha:** 20 de septiembre de 2026  
**Ideas analizadas:** ver [ideas-proyecto.md](ideas-proyecto.md)

---

## Parte 1. Un ejemplo que ya existe, por cada idea

### Idea 1: Diana electrónica para practicar la precisión del saque

- **Qué encontré:** USA Volleyball propone ejercicios específicos para entrenar la colocación del saque mediante zonas objetivo. En uno de sus recursos explica que se pueden colocar botes, tiras de alfombra u otros objetos como blancos y llevar un registro de cuántas veces se acierta.
- **Enlace:** https://usavolleyball.org/resource/time-to-close-the-serving-gap/
- **Qué hace:** convierte la precisión del saque en un ejercicio medible, porque el jugador intenta servir hacia zonas concretas y registra sus aciertos.
- **Por qué no resuelve mi caso:** el ejercicio depende de objetos pasivos y del conteo manual. Mi propuesta mantendría la idea de entrenar hacia un objetivo, pero agregaría sensores que detecten automáticamente el impacto y un contador digital para dar retroalimentación inmediata.

### Idea 2: Medidor portátil de salto para ataque y bloqueo

- **Qué encontré:** el VERT Wearable Jump Monitor, un dispositivo utilizado para registrar saltos. Existe un estudio realizado con jugadores juveniles de voleibol de alto nivel en el que se comparó VERT con un dispositivo VERTEC durante saltos de ataque y bloqueo.
- **Enlace:** https://pmc.ncbi.nlm.nih.gov/articles/PMC5676319/
- **Qué hace:** permite cuantificar el rendimiento de salto y registrar datos durante acciones específicas de voleibol.
- **Por qué no resuelve mi caso:** es un dispositivo comercial especializado y utiliza una tecnología diferente a la que se plantea para el prototipo. Mi propuesta busca una solución más sencilla, fabricable y enfocada solamente en obtener una estimación del salto durante una prueba.

### Idea 3: Aro inteligente para entrenar pase y colocación

- **Qué encontré:** VolleyballUSA comercializa un Passing / Setting Target, una estructura ajustable con una zona objetivo de aproximadamente 4 x 4 pies que sirve para practicar pase y colocación hacia un punto específico.
- **Enlace:** https://www.volleyballusa.com/pst-large-passing-setting-target/
- **Qué hace:** proporciona un objetivo físico ajustable en altura y ángulo para que los jugadores repitan pases y colocaciones buscando una ubicación determinada.
- **Por qué no resuelve mi caso:** el producto funciona como objetivo físico, pero no detecta automáticamente cada acierto ni muestra estadísticas. Mi propuesta incorporaría sensores y un contador para convertir el ejercicio en una práctica medible.

---

## Parte 2. Fuentes de la idea que elegí

### Fuente 1

| Campo | Contenido |
|---|---|
| Autor u organización | USA Volleyball |
| Título | Time to Close the Serving Gap |
| Año | 2011 (publicación original indicada por el sitio) |
| Enlace | https://usavolleyball.org/resource/time-to-close-the-serving-gap/ |
| Tipo | Sitio institucional / recurso de entrenamiento |
| Por qué le creo | Es material publicado por USA Volleyball y describe métodos utilizados para entrenar el saque y su precisión. |
| Qué dato me dio | Explica que se pueden colocar objetivos en la cancha y llevar un registro de cuántos saques llegan a esas zonas. Esto respalda la idea de medir la precisión del saque mediante objetivos concretos. |

### Fuente 2

| Campo | Contenido |
|---|---|
| Autor u organización | USA Volleyball |
| Título | USA Volleyball Skills Contest |
| Año | s. f. (consultado en 2026) |
| Enlace | https://usavolleyball.org/resource/skills-contest/ |
| Tipo | Sitio institucional / recurso de entrenamiento |
| Por qué le creo | Es un recurso publicado por la organización nacional de voleibol de Estados Unidos y presenta ejercicios para evaluar habilidades específicas del deporte. |
| Qué dato me dio | En la prueba de servicio se busca desarrollar precisión de colocación y se pide servir balones hacia seis zonas diferentes de la cancha. Esto me dio una referencia para pensar en una diana con zonas y puntuación. |

### Fuente 3

| Campo | Contenido |
|---|---|
| Autor u organización | Arduino |
| Título | Knock Sensor |
| Año | s. f. (consultado en 2026) |
| Enlace | https://docs.arduino.cc/built-in-examples/sensors/Knock/ |
| Tipo | Documentación técnica |
| Por qué le creo | Es documentación oficial del ecosistema Arduino y muestra un ejemplo práctico de cómo leer un elemento piezoeléctrico como sensor de golpes o vibraciones. |
| Qué dato me dio | El ejemplo muestra que un piezoeléctrico puede conectarse a una entrada analógica, comparar la lectura con un umbral y activar una respuesta cuando se detecta un golpe. Esa lógica puede adaptarse para detectar el impacto de un balón sobre una diana. |

---

## Parte 3. Qué haría distinto

Mi propuesta tomaría una práctica que ya se utiliza en voleibol —servir hacia zonas específicas y contar los aciertos— y la convertiría en un sistema electrónico sencillo. En lugar de colocar solamente un objeto en el piso y contar manualmente, construiría una diana con una o varias zonas capaces de detectar el impacto del balón. El microcontrolador confirmaría el acierto mediante un LED y llevaría el conteo en una pantalla. También buscaría que el sistema fuera portátil, resistente y económico, de manera que pudiera utilizarse durante una práctica individual sin necesidad de que otra persona lleve las estadísticas.

## Parte 4. Qué me falta averiguar

- [ ] ¿Qué sensor de impacto funciona mejor con un balón de voleibol: un piezoeléctrico, un sensor de vibración u otra alternativa?
- [ ] ¿Qué material puede proteger el sensor y al mismo tiempo transmitir suficientemente bien el golpe del balón?
- [ ] ¿Qué tamaño y ubicación de las zonas objetivo serían adecuados para que el ejercicio realmente entrene precisión de saque?
- [ ] ¿Cómo evitar que una sola vibración produzca varios registros del mismo impacto?

---

[Volver a las ideas](ideas-proyecto.md) · [Volver al README](README.md)

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT de OpenAI.
- **Qué le pedí:** Utilicé la IA como apoyo en la redacción y organización de la investigación y para orientarme sobre qué documentación técnica, proyectos similares y fuentes relacionadas con voleibol podía consultar para investigar las propuestas que yo ya había planteado.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** Tomé las recomendaciones solamente como apoyo para saber qué investigar. Entré a las fuentes para corroborar la información y revisé que los enlaces y datos fueran útiles antes de incluirlos. También rechacé o corregí cambios que no correspondían con mis propuestas o que modificaban el enfoque que yo quería darle al proyecto. La selección final de la información y de la idea a desarrollar fue realizada por mí.
