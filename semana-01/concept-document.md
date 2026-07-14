# Concept Document — CALLA O CORRE

**Equipo:** Iron Pixels  
**Integrantes:** Cristian Sahon, Marcos Sulugüi, Nahum Albeño, Gilmar Maldonado
**Fecha:** [14/07/2026]

---

## 1. Nombre del juego

**CALLA O CORRE**

---

## 2. Género

Horror · Supervivencia · Exploración

---

## 3. Sinopsis

Tras un misterioso apagón provocado por un experimento fallido en un edificio corporativo de cinco niveles, un ente desconocido quedó atrapado en el interior y comenzó a cazar a cualquiera que intentara escapar. El jugador despierta solo, sin comunicación con el exterior y con una linterna casi sin batería; su única oportunidad es descender por el edificio mientras evita ser detectado por una criatura que se guía por el sonido y la luz.

---

## 4. Mecánica principal

El jugador debe explorar cada nivel del edificio para encontrar llaves, baterías y fragmentos del código de activación del sistema de emergencia. Durante el recorrido deberá administrar la batería de su linterna, evitar hacer ruido y decidir constantemente entre correr o avanzar en silencio, ya que cualquier sonido o fuente de luz puede atraer al monstruo.

### Loop de juego

1. Explorar el nivel.
2. Buscar llaves, baterías y recursos.
3. Administrar la batería de la linterna.
4. Evitar al monstruo utilizando el sigilo.
5. Encontrar un fragmento del código de activación.
6. Abrir la salida hacia el siguiente nivel.
7. Repetir el proceso hasta llegar al lobby.

---

## 5. Personaje principal

**Nombre:** Daniel *(nombre provisional)*

**Descripción visual:** Empleado del edificio con ropa formal, una mochila pequeña y una linterna como herramienta principal.

**Habilidades:**

- Correr para escapar rápidamente.
- Agacharse para reducir el ruido y evitar ser detectado.
- Administrar el uso de la linterna.
- Interactuar con puertas, llaves y objetos.

**Controles básicos:**

- **WASD:** Movimiento.
- **Shift:** Correr.
- **Ctrl:** Agacharse.
- **E:** Interactuar.
- **F:** Encender o apagar la linterna.

---

## 6. Pantallas / Niveles

### Nivel 1 – Tutorial

El jugador aprende los controles básicos, el funcionamiento de la linterna, la administración de la batería y cómo el monstruo detecta el sonido y la luz.

### Nivel 2 – Oficinas Administrativas

Se introducen las primeras llaves, puertas bloqueadas y rutas alternativas mientras el monstruo comienza a patrullar. Al finalizar el nivel se obtiene el primer fragmento del código.

### Nivel 3 – Área de Laboratorios

El jugador debe recorrer zonas más oscuras y administrar cuidadosamente sus recursos mientras el enemigo responde con mayor rapidez al sonido y a la luz. Aquí encuentra el segundo fragmento del código.

### Nivel 4 – Centro de Operaciones

Los recursos son más escasos y la dificultad aumenta. El jugador obtiene el último fragmento necesario para completar el código de activación.

### Nivel 5 – Lobby Principal

El jugador llega al lobby del edificio, donde se encuentra el panel del sistema de emergencia que controla la puerta principal. Mientras el monstruo lo persigue constantemente, deberá ingresar rápidamente el código que fue reuniendo durante toda la partida. Si logra introducirlo correctamente antes de ser alcanzado, la puerta se abrirá y escapará del edificio; de lo contrario, el monstruo lo atrapará y perderá la partida.

---

## 7. Elemento de Inteligencia Artificial

El enemigo utilizará una **Máquina de Estados (Finite State Machine)** basada en percepción.

### Estados del enemigo

- Patrullar.
- Investigar sonidos.
- Detectar la luz de la linterna.
- Perseguir al jugador.
- Buscar en la última posición conocida.
- Regresar a la patrulla.

La IA reaccionará dinámicamente a los sonidos producidos por correr, abrir puertas o interactuar con objetos, así como al uso de la linterna, haciendo que cada partida sea diferente.

---

## 8. Motor de videojuego

**Unity** *(propuesto; sujeto a la decisión del equipo de Programación de Videojuegos).*

---

## 9. Público objetivo

Jóvenes y adultos entre 15 y 30 años que disfrutan videojuegos de horror, exploración y supervivencia con sesiones cortas de entre 15 y 20 minutos.

---

## 10. ¿Por qué es viable en 20 semanas?

El proyecto tiene un alcance realista para un equipo universitario de cuatro integrantes. Todo el juego se desarrolla en un único edificio dividido en cinco niveles, utiliza un solo enemigo principal y mecánicas sencillas como exploración, gestión de recursos y sigilo. La inteligencia artificial se implementará mediante una máquina de estados, una solución ampliamente utilizada y alcanzable dentro del tiempo disponible. Además, la duración máxima de 20 minutos permite concentrar el desarrollo en una experiencia completa sin requerir una gran cantidad de contenido.

---

## 11. Riesgos identificados

### Riesgo 1

**Descripción:** La inteligencia artificial del enemigo puede resultar más compleja de implementar de lo esperado.

**Mitigación:** Desarrollar primero una versión básica con patrullaje y persecución, agregando posteriormente los comportamientos de investigación y búsqueda.

### Riesgo 2

**Descripción:** El desarrollo de todos los niveles podría tomar más tiempo del previsto.

**Mitigación:** Diseñar un piso base reutilizable y modificar únicamente la distribución, iluminación y objetivos de cada nivel.

---

## 12. Retroalimentación recibida en clase

**Pendiente de completar después de la presentación del pitch.**
