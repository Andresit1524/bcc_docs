# Escena de batalla
La escena de batalla se compone por el siguiente árbol de nodos. Se han omitido varios nodos para resaltar solo la estructura básica:

```
○ Battle
┣━○ Background      # El fondo (por ahora un color)
┣━○ UILayer/UI      # Toda la interfaz
┃ ┣━○ Battle         # Batalla (baraja, paneles)
┃ ┣━○ Pause          # Pausa
┃ ┗━○ End            # Fin de juego (Ranking)
┣━○ BattleData      # Datos de la batalla actual
┣━○ BattleManager   # Gestor de batalla con sus estados
┃ ┣━○ Start
┃ ┣━○ Turn
┃ ┣━○ Loop
┃ ┣━○ Referee
┃ ┗━○ End
┗━○ Stage           # Mundo 3D
  ┣━○ Platform      # Plataforma del juego
  ┣━○ Dice          # Dado
  ┣━○ Rocks         # Rocas
  ┗━○ Players       # Jugadores
```

*La estructura en archivos y carpetas no se añade porque está sujeta a cambios rápidamente*. La estructura del `BattleManager` se explica con un poco más de detalle [aquí](./battle_sfm.md).

!!! Bug "Un problema de estructura"
    
    Actualmente esta estructura es enredada a nivel de código, especialmente con:

    1. La separación de las responsabilidades en el `BattleManager`
    2. La excesiva abstracción en el `Stage`
    3. La arquitectura de las señales y como se propagan por el árbol

    Queda pendiente simplificar esta estructura, y además prepararla para añadir las nuevas reglas y sistemas que le faltan al juego, esto último en el `BattleManager` y sus hijos.
