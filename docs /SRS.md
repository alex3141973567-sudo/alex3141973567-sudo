# Especificación de Requisitos de Software (SRS)

**Proyecto:** Sanar tu mundo
**Versión:** 1.0
**Fecha:** 13/11/2026
**Equipo:** Alejandro Elías Moreno, Geogan Alexander Velázquez García

---

## 1. Introducción

### 1.1 Propósito
Este documento define los requisitos de software del proyecto Sanar tu mundo.
Sirve como acuerdo común para el equipo de desarrollo y como base para
planear, construir y probar el sistema. Está dirigido a los integrantes del
equipo y a la maestra que evalúa el proyecto.

### 1.2 Alcance
Sanar tu mundo es un videojuego en el que el jugador explora un mundo con
distintos biomas, flora y fauna, sigue una historia lineal y puede jugar con
otras personas en modo multijugador. Incluye música ambiental. En esta
versión no se contemplan compras dentro del juego ni versión para celular.

### 1.3 Glosario
| Término | Definición |
|---|---|
| SRS | Especificación de Requisitos de Software |
| RF | Requisito funcional: lo que el sistema debe hacer |
| RNF | Requisito no funcional: cómo debe comportarse el sistema |
| Bioma | Zona del mundo con clima, terreno y paisaje propios |
| Flora y fauna | Plantas y animales presentes en cada bioma |
| Textura | Imagen que se aplica a los objetos del juego para darles apariencia |
| Multijugador | Modo en el que varios jugadores comparten la misma partida |
| Jugabilidad | Controles y mecánicas con las que el jugador interactúa con el juego |

### 1.4 Referencias
- IEEE Std 830-1998. Recommended Practice for Software Requirements Specifications.
- docs/investigacion-srs.md

---

## 2. Descripción general

### 2.1 Usuarios
| Usuario | Descripción |
|---|---|
| Jugador | Persona que juega en PC; no necesita conocimientos técnicos |
| Equipo desarrollador | Integrantes que mantienen y amplían el juego |

### 2.2 Restricciones
- El proyecto se desarrolla durante el semestre actual con un equipo de estudiantes.
- El juego debe funcionar en una computadora con Windows de gama media.
- El código y la documentación se gestionan en GitHub.

### 2.3 Supuestos y dependencias
- Cada jugador cuenta con una computadora que cumple los requisitos mínimos.
- El modo multijugador requiere conexión a internet estable.
- Los recursos gráficos y de audio se crean por el equipo o tienen licencia libre.

---

## 3. Requisitos específicos

### 3.1 Requisitos funcionales

**RF-01 — Flora y Fauna**
- **Descripción:** El juego debe incluir al menos 3 tipos de plantas y 3 tipos de animales distribuidos en los biomas.
- **Prioridad:** Alta
- **Criterio de aceptación:** Al recorrer el mundo el jugador encuentra al menos 3 plantas y 3 animales distintos, cada uno con su textura propia.

**RF-02 — Historia lineal**
- **Descripción:** El juego debe presentar una historia con inicio, desarrollo y final que avanza en orden mediante objetivos.
- **Prioridad:** Alta
- **Criterio de aceptación:** El jugador puede completar todos los objetivos en orden y al terminar el último se muestra la pantalla final.

**RF-03 — Jugabilidad**
- **Descripción:** El jugador debe poder moverse, interactuar con objetos y realizar las acciones principales con teclado y mouse.
- **Prioridad:** Alta
- **Criterio de aceptación:** Con teclado y mouse el jugador camina, salta e interactúa con objetos, y cada acción responde en menos de 1 segundo.

**RF-04 — Música**
- **Descripción:** El juego debe reproducir música ambiental distinta en cada bioma, con control de volumen.
- **Prioridad:** Media
- **Criterio de aceptación:** Al entrar a otro bioma cambia la pista, y desde Opciones el jugador puede subir, bajar o silenciar el volumen.

**RF-05 — Multiplayer**
- **Descripción:** El juego debe permitir que al menos 2 jugadores compartan la misma partida.
- **Prioridad:** Media
- **Criterio de aceptación:** Dos jugadores se conectan a la misma partida y cada uno ve al otro moverse en tiempo real.

### 3.2 Requisitos no funcionales

**RNF-01 — Rendimiento**
- **Descripción:** El juego debe mantener una fluidez aceptable durante la partida.
- **Prioridad:** Alta
- **Criterio de aceptación:** En una computadora de gama media el juego mantiene al menos 30 cuadros por segundo durante 10 minutos de juego.

**RNF-02 — Usabilidad**
- **Descripción:** Un jugador nuevo debe poder empezar a jugar sin leer instrucciones externas.
- **Prioridad:** Media
- **Criterio de aceptación:** 4 de 5 personas de prueba inician una partida y completan el primer objetivo sin ayuda en menos de 5 minutos.

**RNF-03 — Mantenibilidad**
- **Descripción:** El proyecto debe estar organizado para que cualquier integrante pueda continuar el trabajo de otro.
- **Prioridad:** Media
- **Criterio de aceptación:** Un integrante nuevo clona el repositorio y ejecuta el proyecto siguiendo solo el README, sin pedir ayuda.

### 3.3 Checklist de calidad
Cada requisito se revisó contra estos criterios: correcto, no ambiguo, completo,
consistente, factible y verificable.
