# Registro de cambios (Changelog)
Este changelog recopila los cambios en el juego y en la documentación. Estos últimos se etiquetan con **(Docs)**.

_Los cambios en la documentación registrados aquí solo incluyen páginas nuevas, eliminadas o cambios importantes_. Si necesitas más detalles, consulta el [historial de git de la documentación](https://github.com/Andresit1524/bcc_docs) y el [del juego](https://github.com/Andresit1524/beast_card_clash).

!!! Note "Formato"

    El formato para el changelog y el orden cronológico es el siguiente:

    - Meses, semanas y días: **orden descendente**
    - Tareas dentro del mismo día: **orden ascendente**

---

## Junio del 2026

### Semana del 15 al 21 de junio
- 16 de junio:
    - Rediseño de jugador: script más sencillo, menos funciones innecesarias y externalización de constantes
    - Reorden en el código de `BattleUI` y `PlayerPanel` para simplificar las funciones y usar Unique Node Names
    - Solución del bug que hacia que un jugador ganase en un empate de elemento y valor
- 15 de junio:
    - **(Docs)** Nueva página: [Escena de batalla](./arquitectura/battle_scene.md)
    - Eliminación de la señal innecesaria `BattleStage.players_ready`
    - Simplificación de la lógica de la roca
    - Simplificación de la lógica del dado y su integración con `BattleManager`

### Semana del 7 al 14 de junio
- 14 de junio:
    - Renombre definitivo de `World` hacia `Stage`
    - Interfaz de batalla agrupada
    - Recarga de los archivos del proyecto
- 13 de junio:
    - Mejoras en el manejo de los turnos y la inicialización en batalla
    - **(Docs)** Nueva página: [Máquina de estados de la batalla](./arquitectura/battle_sfm.md)
    - Optimización del referee y la gestión de la batalla
    - Ahora el podium siempre se muestra y es el correcto
    - Corrección del error que hacia que el primer jugador, cuando era el humano en la roca superor, no pudiera moverse apropiadamente
    - La música ahora se pausa al finalizar el juego
    - Señales ahora manuales en el editor, en lugar de por código
- 11 de junio: 
    - Limpieza general y actualización del repositorio
    - Preparación para la versión 0.2
- 9 de junio: **(Docs)** Migración de la documentación de Jekyll a Zensical

### Semana del 1 al 7 de junio
- 1 de junio:
    - Menú de pausa en batalla
    - Tutorial básico en sustitución a los paneles viejos
    - Música en bucle para el menú y la batalla
    - Etiqueta de versión
    - **(Release)** Versión 0.1 para su entrega en el SOFA

---

## Mayo de 2026

### Semana del 25 al 31 de mayo
- 29 de mayo:
    - Cambios de nombre y limpieza en el código
    - Reorganización de la carpeta de batalla
- 26 de mayo: **(Docs)** Nueva base para documentación en GitHub Pages

### Semana del 18 al 24 de mayo
- 24 de mayo: **(Docs)** Eliminación de documentación vieja (la de IA)

### Semana del 27 de abril al 3 de mayo
- 01 de mayo: 
    - Nuevas animaciones para los osos
    - Nuevo ícono del juego
    - `GameConstants` ahora es `Constants`, sin autoload
    - Ajustes nuevos para edición y depuración en VSCode
    - `skin_selector` ahora es un `.tscn` y usa los nuevos sprites en 2D
    - Simplificación del sistema de selección de equipos
    - Mejoras menores en las interfaces

---

## Abril de 2026

### Semana del 20 al 26 de abril
- 24 de abril: 
    - Nueva animación para el oso
    - Eliminacion de los modelos viejos
    - Organización de licencias, tests
    - Adiciones menores en el README y la licencia

### Semana del 06 al 12 de abril
- 11 de abril:
    - Adición de `GEMINI.md` con instrucciones para la IA
    - Optimización en el `Referee`: ahora usamos una matriz de fortaleza en lugar de un `match`
    - El oso ahora usa un sprite
- 10 de abril: Prototipo y mejora del sistema de ranking al final del juego
- 06 de abril: 
    - Reorganización de la carpeta de batalla
    - Prototipo de `BattleData`
    - Efecto visual al morir: desvanecimiento
    - Corrección de las cartas fantasma extra en la baraja
    - Corrección en el manejo de turnos tras un game over
    - **(Docs)** Inicio del `changelog.md`
    - **(Docs)** Feedback de la arquitectura de batalla

---

## Marzo de 2026

### Semana del 23 al 29 de marzo
- 27 de marzo: Nueva regla implementada: las cartas son 9 y se reponen
- 26 de marzo: 
    - Prototipo del `BattleReferee` para manejo de rondas y muerte de jugadores
    - Resaltado del dado y los paneles del jugador al perder vida
    - Movimiento de baraja para ocultar-mostrar
    - **(Docs)** Actualización de la documentación
- 25 de marzo:
    - El mundo de batalla (`World`) ahora es una escena independiente
    - Implementación de instancia y movimiento de los jugadores
    - Lista de elementos ahora es una constante: `ElementsList`
    - Mejora en el manejo de los paneles de personaje
    - Corrección en el shader de contorno: ahora se desactiva si el grosor es cero
    - Mejor manejo y responsividad de las rocas y cartas en batalla
    - Flujo básico de batalla: lanzar dado, elegir carta y rotar el turno
- 24 de marzo:
    - Segmentación en la estructura de la escena de batalla y sus estados
    - **(Docs)** Documentación detallada del sistema de batalla
    - Insignias en el README
    - Actualización en la configuración del proyecto
- 23 de marzo:
    - Ajustes menores en los scripts de autoloads y máquina de estados
    - Reordenamiento de escenas
    - Nueva escena independiente para el personaje-jugador

### Semana del 16 al 22 de marzo
- 22 de marzo: Interfaz de fin de juego en batalla
- 20 de marzo:
    - Optimizaciones en los scripts de dados y rocas
    - Ahora los shaders oscilan su grosor e intensidad
- 18 de marzo:
    - Ícono para la máquina de estados
    - Ahora el `BattleManager` es la máquina de estados de batalla
    - Script de utilidades (`utilities.gd`)
    - Ordenaciones en el código
    - Mejoras en el resaltado de las rocas
    - Ahora las rocas tienen contorno con el shader
- 17 de marzo: 
    - Nueva música original para el juego
    - Prototipo de la máquina de estados de batalla
    - Modo de partida rápida
    - Organización de archivos
    - **(Docs)** Actualización de la documentación técnica

### Semana del 09 al 15 de marzo
- 15 de marzo:
    - Conexión interfaz-juego en batalla
    - Las rocas ahora tienen los íconos de los elementos
    - Docstrings y otras adiciones al código
- 11 de marzo:
    - Inclusión de los íconos de los elementos
    - Corregido el bug que movía bruscamente las cartas
    - Shader para resaltado y contorno de objetos
    - Lógica base para la rocas y los jugadores en batalla
- 09 de marzo: Actualización en el `.gitignore`
- 09 de marzo:
    - Instalación del plugin `VectorDisplay2D`
    - Implementación de movimiento ondulatorio en las cartas
    - Corrección de bugs que hacia los dados siempre clicables

### Semana del 02 al 08 de marzo
- 08 de marzo: 
    - Ajustes en las rocas
    - Corrección del bug que hacia girar las cartas siempre
    - Barra de vida en los paneles de los jugadores
- 03 de marzo:
    - Tabuladores y botón de jugar en el selector de equipos
    - Creación de `BattleManager`
    - Mejoras en el sistema de baraja y cartas
    - Prototipo de la interfaz y dado de batalla
    - **(Docs)** Actualización de la documentación del proyecto

### Semana del 23 de febrero al 01 de marzo
- 01 de marzo:
    - Tabuladores en `DialogueManager`
    - Nuevo elemento 'aire' y adición de todas las cartas
    - Demo de la baraja en batalla

---

## Febrero de 2026

### Semana del 23 de febrero al 01 de marzo
- 26 de febrero: Ajustes en la guía de contribución (`CONTRIBUTING.md`)

### Semana del 09 al 15 de febrero
- 10 de febrero:
    - Rediseño de los créditos y mejoras generales en la UI
    - **(Docs)** Cambio del modelo de IA del sistema de documentación
    - Corrección en la skin del panda
    - Primera versión del selector de personajes y aspectos (skins)
    - Cambio a tabuladores para todo el código

### Semana del 02 al 08 de febrero
- 08 de febrero:
    - Verificación de tipos en los `AutoloadResource`
    - Nuevos autoloads: `PlayerStats` y `GameConstants`
    - Nuevo componente de UI: Barra superior en pantalla
- 07 de febrero:
    - Implementación de los `AutoloadResource`
    - Cambio de fuentes
    - Mejoras visuales en las interfaces
    - Primera versión funcional del selector de personajes
- 06 de febrero: Desinstalación de plugins no utilizados: Git Bash y MarkdownLabel
- 05 de febrero:
    - Integración del plugin para terminal Git Bash
    - Mejora en los prints
    - Nuevas texturas para la rana
    - Botón para ir al tutorial desde el menú de inicio
- 03 de febrero:
    - Limpieza del código y de `MusicManager` 
    - Reorganización del juego hacia `assets` y UIDs
    - Nuevos diálogos
    - Nuevo singleton: `Flags`

---

## Enero de 2026

### Semana del 26 de enero al 01 de febrero
- 30 de enero:
    - Incorporación del modelo del dado y el camaleón
    - Implementación de tipado fuerte y optimizaciones
    - Ajustes para VSCode
    - Creación del `MusicManager`
- 29 de enero: Adición de personajes 3D y materiales para el oso y la rana
- 28 de enero: Importación de modelos 3D y skins para los personajes del juego
- 27 de enero:
    - Nuevo singleton: `SceneManager`
    - Reubicación y mejoras en las interfaces
    - Música para el menú principal del juego
- 26 de enero:
    - **Inicio oficial del proceso de portado del proyecto desde Unity**
    - Primera versión funcional de la interfaz de usuario para inicio, tutorial y créditos

### Semana del 19 al 25 de enero
- 25 de enero:
    - Commit inicial: creación del repositorio y estructura básica
    - Inicialización del proyecto en Godot
    - Actualización de los términos de la licencia del proyecto
    - Instalación de Dialogue Manager y MarkdownLabel
    - Configuración de exportación para builds
    - **(Docs)** Implementación del sistema de generación automática de documentación con IA
