# Escena de batalla
La escena de batalla se compone por todos los elementos de la carpeta `assets/battle/`. Se han omitido varios nodos para resaltar solo la estructura básica:

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

*La estructura en archivos y carpetas no se añade porque está sujeta a cambios rápidamente*, sin embargo es similar a la división propuesta en el árbol de nodos:

1. Estados de batalla
2. Interfaz
3. Escenario de batalla

La estructura del `BattleManager` y sus estados se explica con un poco más de detalle [aquí](./battle_sfm.md).
