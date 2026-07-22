# Product Backlog v1 — Dead Harvest

**Equipo:** Iron Pixels | **Fecha:** 21 de julio de 2026

## Paso 1: Definir la Visión

**Misión:** Crear una experiencia de supervivencia y acción 2D de ritmo rápido, donde los jugadores pongan a prueba sus reflejos y estrategia a través de un combate cuerpo a cuerpo desafiante. El equipo se enfoca en desarrollar mecánicas de control precisas, una IA enemiga dinámica y un sistema de progresión por oleadas que garantice partidas rejugables, donde la gestión de recursos y la habilidad sean fundamentales para resistir el apocalipsis.

**Visión:** Posicionar a Dead Harvest como un título indie destacado dentro del género de supervivencia cenital, reconocido por la fluidez de su combate cuerpo a cuerpo y el diseño inteligente de su curva de dificultad. El equipo aspira a entregar un juego altamente pulido que atrape a los jugadores que buscan retos directos, construyendo una experiencia adictiva que los motive a superar sus propios límites en cada partida.

## Paso 2: Identificar Épicas

1. **Movimiento y Control del Jugador** — mecánicas de desplazamiento, esquiva y control del personaje.
2. **Sistema de Combate** — armas cuerpo a cuerpo, sistema de daño, estamina y eliminación de enemigos.
3. **IA de Enemigos** — comportamiento de los distintos tipos de zombis mediante máquina de estados y sistema de oleadas.
4. **Progresión y Mejoras** — mejoras temporales entre rondas y aumento gradual de dificultad.
5. **Interfaz y Flujo del Juego** — menú principal, HUD, pantalla de victoria/derrota y estadísticas.

### Elaboración de épicas

**Épica 1 — Movimiento y Control del Jugador**

El movimiento es la base sobre la que se construye toda la experiencia de Dead Harvest: al no existir armas a distancia, la supervivencia del jugador depende casi por completo de su capacidad para posicionarse correctamente frente a la horda. El personaje se desplaza en ocho direcciones sobre la vista cenital mediante WASD, con una velocidad constante que debe sentirse ágil pero controlable, evitando que el jugador pueda simplemente "correr en círculos" para evadir cualquier peligro sin costo alguno.

El dash (esquiva) es la herramienta reactiva principal: permite atravesar brevemente una zona de peligro o escapar de un ataque inminente a cambio de un consumo de estamina, el mismo recurso que comparte con el sistema de combate. Esto obliga al jugador a decidir constantemente entre atacar, esquivar o retirarse, en lugar de abusar de cualquiera de las tres opciones. El movimiento también debe integrarse con el entorno de la arena (colisiones con barricadas, cuellos de botella y trampas), de modo que el posicionamiento táctico —y no solo los reflejos— sea parte central de la estrategia de supervivencia.

**Épica 2 — Sistema de Combate**

El sistema de combate de Dead Harvest constituye el corazón de la experiencia de acción y supervivencia. Desarrollado exclusivamente alrededor de armas cuerpo a cuerpo, busca entregar combates intensos, estratégicos y fluidos contra oleadas de zombis, donde la gestión de la estamina y la elección oportuna de arma determinan la supervivencia del jugador.

El sistema de estamina funciona como recurso central y limitado: se consume al atacar (ataques ligeros o pesados) y al esquivar (dash), y se regenera gradualmente cuando el personaje deja de actuar de forma agresiva. Si se agota, el jugador entra en un estado de recuperación temporal que reduce su velocidad de ataque y movimiento, aumentando el riesgo frente a la horda. Las armas ligeras consumen menos estamina con daño moderado; las armas pesadas (como hachas o mazos) consumen más a cambio de mayor daño en área y posibles efectos de aturdimiento.

Cada arma tiene valores diferenciados de alcance, velocidad, daño base y efectos adicionales (sangrado, knockback), lo que fomenta la adaptación estratégica: un arma rápida para corredores ágiles, un arma pesada para grupos de caminantes o acorazados resistentes. El sistema de daño considera la dirección del ataque en la vista cenital y las resistencias particulares de cada tipo de zombi (los acorazados ignoran parcialmente ataques ligeros; los explosivos deben eliminarse antes de que se acerquen demasiado). Al eliminar enemigos se generan recompensas de recursos que alimentan el sistema de mejoras entre oleadas, reforzando el bucle roguelite del juego.

**Épica 3 — IA de Enemigos**

La inteligencia artificial de los zombis se implementa mediante una máquina de estados finitos (patrullar, perseguir, atacar y reaccionar al daño recibido), lo que permite comportamientos creíbles y variados sin requerir técnicas de aprendizaje automático. Cada zombi comienza en un estado de patrulla o reposo dentro de la arena; al detectar al jugador dentro de un radio de percepción, transiciona a persecución, y al estar en rango de ataque, ejecuta su rutina de combate correspondiente.

La diversidad de enemigos es lo que mantiene el desafío evolucionando partida tras partida: los Caminantes son lentos pero peligrosos en grupo; los Corredores obligan al jugador a mantenerse en movimiento constante; los Acorazados requieren armas contundentes para romper su resistencia; y los Explosivos añaden un elemento de gestión de riesgo, ya que detonan al morir y deben eliminarse a distancia o dirigirse hacia otros enemigos. El sistema de oleadas coordina cuándo y cuántos enemigos de cada tipo aparecen, y sirve como base para el incremento progresivo de dificultad, de modo que cada ronda superada se sienta como un logro medible.

**Épica 4 — Progresión y Mejoras**

La progresión de Dead Harvest sigue la estructura clásica de un roguelite: al finalizar cada oleada, el jugador recibe un breve respiro y debe elegir una mejora temporal entre varias opciones presentadas (por ejemplo, mayor velocidad de movimiento, reducción del consumo de estamina, o efectos adicionales en los ataques). Estas mejoras se acumulan a lo largo de la partida, permitiendo que el jugador desarrolle una "build" distinta cada vez que juega, lo cual fomenta la rejugabilidad.

En paralelo, la dificultad aumenta de forma gradual: cada oleada incrementa la cantidad y/o agresividad de los enemigos, obligando al jugador a usar las mejoras obtenidas de manera efectiva en vez de depender solo de la habilidad inicial. El balance entre la velocidad de esta curva de dificultad y la generosidad del sistema de mejoras es uno de los aspectos que el equipo deberá ajustar mediante pruebas de juego constantes, ya que de esto depende que la experiencia se sienta justa y no frustrante.

**Épica 5 — Interfaz y Flujo del Juego**

La interfaz de Dead Harvest debe comunicar de forma clara e inmediata el estado del jugador durante partidas de ritmo rápido: la barra de vida, el nivel de estamina y el número de ronda actual se muestran en un HUD minimalista que no debe distraer de la acción en pantalla, dado que el jugador necesita reaccionar en fracciones de segundo ante la horda.

El flujo general del juego inicia en un menú principal donde el jugador puede iniciar partida, ajustar opciones o salir de la aplicación. Al concluir una partida —ya sea por derrota o por vencer al jefe final— se presenta una pantalla de resultados con estadísticas relevantes (tiempo de supervivencia, enemigos eliminados, mejoras obtenidas), que además de cerrar la experiencia de forma satisfactoria, invita al jugador a intentar superar su propio desempeño en la siguiente partida, reforzando el carácter rejugable del título.

## Paso 3: Historias de Usuario

**Épica 1 — Movimiento y Control del Jugador**
- **HU-01 — Desplazamiento del personaje:** Como jugador, quiero mover a mi personaje en 8 direcciones usando las teclas WASD, para moverme con libertad por la arena de juego.
- **HU-02 — Habilidad de esquiva (Dash):** Como jugador, quiero realizar una esquiva tipo Dash al presionar la barra espaciadora, para evitar ataques directos de los zombis con un costo de estamina.

**Épica 2 — Sistema de Combate**
- **HU-03 — Ataque cuerpo a cuerpo:** Como jugador, quiero infligir daño a los zombis haciendo clic izquierdo, para eliminarlos y defender mi posición.
- **HU-04 — Cambio de armamento:** Como jugador, quiero alternar entre diferentes armas cuerpo a cuerpo mediante las teclas Q y E, para adaptarme a la velocidad y resistencia de los distintos enemigos.
- **HU-05 — Recolección de botiquines:** Como jugador, quiero agarrar curas dispersas por la arena, para recuperar puntos de vida durante los enfrentamientos.

**Épica 3 — IA de Enemigos**
- **HU-06 — Detección y persecución básica:** Como jugador, quiero que los zombis vigilen y me persigan al detectarme, para sentir la constante amenaza de la horda.
- **HU-07 — Diversidad de enemigos:** Como jugador, quiero enfrentar distintos tipos de zombis (Caminante, Corredor, Acorazado y Explosivo), para adaptar mi estrategia según el comportamiento de cada uno.
- **HU-08 — Enfrentamiento contra el jefe final:** Como jugador, quiero enfrentar a un jefe con ataques y patrones únicos en la fase final, para tener un reto definitivo que me permita escapar de la zona.

**Épica 4 — Progresión y Mejoras**
- **HU-09 — Selección de mejoras entre rondas:** Como jugador, quiero elegir una mejora temporal al finalizar cada oleada, para potenciar las estadísticas o habilidades de mi personaje.
- **HU-10 — Incremento de la dificultad por oleadas:** Como jugador, quiero que la cantidad y agresividad de los enemigos aumente con cada ronda, para mantener el nivel de desafío y tensión.

**Épica 5 — Interfaz y Flujo del Juego**
- **HU-11 — Visualización del HUD en combate:** Como jugador, quiero ver en pantalla mi barra de vida, nivel de estamina y el número de la ronda actual, para gestionar mis recursos en tiempo real.
- **HU-12 — Menú Principal:** Como jugador, quiero acceder a un menú principal para iniciar partida, ajustar opciones o salir, para navegar fácilmente por las funciones básicas del juego.
- **HU-13 — Pantalla de resultado final:** Como jugador, quiero ver un resumen de estadísticas como tiempo de supervivencia, enemigos eliminados y resultado al ganar o morir, para evaluar mi rendimiento en la partida y poco a poco ir mejorando.

## Paso 4: Priorización del Product Backlog

Se utilizará GitHub Projects con un tablero Kanban de cinco columnas (**Backlog, Sprint 1, In Progress, Review, Done**) para organizar el desarrollo mediante una metodología ágil.

### Columna: Sprint 1 (crítico para el MVP jugable)
- HU-01 — Desplazamiento del personaje
- HU-02 — Habilidad de esquiva (Dash)
- HU-03 — Ataque cuerpo a cuerpo
- HU-06 — Detección y persecución básica (IA básica de los zombis)
- HU-10 — Incremento de la dificultad por oleadas (sistema de oleadas)
- HU-11 — Visualización del HUD en combate

### Columna: Backlog (no indispensable para el MVP, se desarrolla en sprints posteriores)
- HU-04 — Cambio de armamento
- HU-05 — Recolección de botiquines
- HU-07 — Diversidad de enemigos (zombis especiales)
- HU-08 — Enfrentamiento contra el jefe final
- HU-09 — Selección de mejoras entre rondas
- HU-12 — Menú Principal
- HU-13 — Pantalla de resultado final

### Columna: In Progress
*(Se moverán aquí las historias que un integrante haya comenzado a desarrollar, para evitar que dos personas trabajen sobre la misma funcionalidad.)*

### Columna: Review
*(Historias ya implementadas, pendientes de revisión por el líder del equipo u otro integrante, verificando que cumplan los criterios de aceptación antes de integrarlas.)*

### Columna: Done
*(Historias completadas y aprobadas, para llevar control del avance por sprint.)*

---

**Resultado:** el equipo obtiene una planificación inicial enfocada en las funcionalidades esenciales del videojuego (movimiento, combate básico, IA de percepción y HUD), dejando para sprints posteriores las características que enriquecen la experiencia (mejoras, variedad de enemigos, jefe final) sin comprometer el alcance ni el tiempo estimado de 20 semanas.
