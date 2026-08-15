# Registro de desarrollo (Changelog)
Este changelog recopila los cambios en el desarrollo del juego y en la documentación. Estos últimos se etiquetan con **(Docs)**. _Los cambios en la documentación registrados aquí solo incluyen páginas nuevas, eliminadas o cambios importantes_. Si necesitas más detalles, consulta el [historial de git de la documentación](https://github.com/Andresit1524/bcc_docs) y el [del juego](https://github.com/Andresit1524/beast_card_clash).

!!! Note "Formato"

    El formato para el changelog y el orden cronológico es el siguiente:

    - Meses, semanas y días: **orden descendente**
    - Tareas dentro del mismo día: **orden ascendente**

## Versiones anteriores

- [Versión `0.1`](v0.1.md)

---

## Agosto de 2026

### Semana del 10 al 16 de agosto
- 15 de agosto: **(Docs)** Changelog dividido por versiones

## Junio del 2026

### Semana del 15 al 21 de junio
- 19 de junio:
    - Sustitución de `AutoloadResource` con autoloads independientes y con verificación de tipos
    - Actualización a Godot 4.7
    - Rediseño de señales en batalla por medio de un bus en la raíz de la escena. **¡Proceso de refactorización de batalla completo!**
    - **(Docs)** Nueva página: [Señales de la escena de batalla](../arquitectura/battle_signals.md)
- 18 de junio:
    - Conversión de `TeamsList` y `ElementsList` a `TeamIcons` y `ElementIcons`, ahora estáticos y precargados
    - `card/card_sprites/` renombrado a `card/sprites/`
    - Eliminación de `BattleData.Snapshot` a favor de diccionarios
- 17 de junio:
    - Constantes de `BattleData` movidas a `Constants`
    - Eliminación de `Utilities` y `Card.set_properties`
    - Tipado estático en todas las funciones y lambdas faltantes por ello
- 16 de junio:
    - Rediseño de jugador: script más sencillo, menos funciones innecesarias y externalización de constantes
    - Reorden en el código de `BattleUI` y `PlayerPanel` para simplificar las funciones y usar Unique Node Names
    - Solución del bug que hacia que un jugador ganase en un empate de elemento y valor
- 15 de junio:
    - **(Docs)** Nueva página: [Escena de batalla](../arquitectura/battle_scene.md)
    - Eliminación de la señal innecesaria `BattleStage.players_ready`
    - Simplificación de la lógica de la roca
    - Simplificación de la lógica del dado y su integración con `BattleManager`

### Semana del 7 al 14 de junio
- 14 de junio:
    - Renombre definitivo de `World` hacia `Stage`
    - Interfaz de batalla agrupada
    - Recarga de los archivos del proyecto
- 13 de junio:
    - **Inicio del proceso de refactorización de la batalla**
    - Mejoras en el manejo de los turnos y la inicialización en batalla
    - **(Docs)** Nueva página: [Máquina de estados de la batalla](../arquitectura/battle_sfm.md)
    - Optimización del referee y la gestión de la batalla
    - Ahora el podium siempre se muestra y es el correcto
    - Corrección del error que hacia que el primer jugador, cuando era el humano en la roca superor, no pudiera moverse apropiadamente
    - La música ahora se pausa al finalizar el juego
    - Señales ahora manuales en el editor, en lugar de por código
- 11 de junio: 
    - Limpieza general y actualización del repositorio
    - Preparación para la versión 0.2
- 9 de junio: **(Docs)** Migración de la documentación de Jekyll a Zensical
