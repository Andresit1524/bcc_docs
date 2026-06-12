# Registro de cambios (Changelog)

!!! Warning
    Este es un registro de cambios granular, extraido del Git del proyecto y adaptado a un formato legible y general.
    
    Esto se actualiza a mano por lo que podría no corresponder con el historial actual.

---

## Junio del 2026

### Semana del 7 al 14 de junio
- 11 de junio: 
    - Limpieza general y actualización del repositorio
    - Preparación para la versión 0.2

### Semana del 1 al 7 de junio
- 1 de junio:
    - Menú de pausa en batalla
    - Tutorial básico en sustitución a los paneles viejos
    - Música en bucle para el menú y la batalla
    - Etiqueta de versión
    - **Versión 0.1** para su entrega en el SOFA

---

## Mayo de 2026

### Semana del 25 al 31 de mayo
- 29 de mayo: Reorganizaciones sencillas y limpieza
- 26 de mayo: Nueva documentación en GitHub Pages

### Semana del 18 al 24 de mayo
- 24 de mayo: Eliminación de documentación vieja (la de IA)

### Semana del 27 de abril al 3 de mayo
- 01 de mayo: 
    - Mejoras en la interfaz y lógica de los selectores
    - Corrección en el selector de skins para usar los nuevos sprites
    - Cambio en el ícono del juego
    - GameConstants ahora es Constants, sin autoload
    - Integración de nuevas animaciones para los osos

---

## Abril de 2026

### Semana del 20 al 26 de abril
- 24 de abril: 
    - Organización de licencias y tests
    - Eliminacion de los modelos viejos
    - Nueva animación para el oso

### Semana del 06 al 12 de abril
- 11 de abril: 
    - Mejoras en el cálculo de enfrentamientos entre elementos
    - Adición del sprite del oso y de GEMINI.md para uso de IA
- 10 de abril: Conexión con la interfaz de fin de batalla, con colores para el ranking
- 06 de abril: 
    - Adición de documentación técnica adicional
    - Hotfix en el manejo de la lógica de fin de juego (Game Over)
    - Corrección de "cartas fantasma" y gestión de jugadores eliminados
    - Ajustes integrales en el gestor de batalla y estados del juego
    - Reorganización de activos de batalla (dados, jugadores, rocas) en sus respectivas carpetas

---

## Marzo de 2026

### Semana del 23 al 29 de marzo
- 27 de marzo: Adición de nuevos contenidos y actualización de las reglas de juego
- 26 de marzo: 
    - Actualización de la documentación técnica del proyecto
    - Mejoras generales en la interfaz de usuario
    - Implementación del prototipo funcional de lucha de cartas
- 25 de marzo:
    - Adiciones al flujo de la secuencia de batalla
    - Implementación del flujo básico de batalla
    - Mejoras en la lógica del juego y optimización de la responsividad
    - HotFix: Optimización del manejo de los paneles de personajes
    - Creación del mundo de batalla y configuración de personajes
- 24 de marzo:
    - Ajustes menores en los detalles de configuración del proyecto
    - Integración de la rama de documentación
    - Documentación detallada del sistema de batalla
    - Reorganización estructural de la escena de batalla y sus estados
- 23 de marzo:
    - Reordenamiento y adición de la escena de personalización de personajes
    - Ajustes menores en los scripts de autoloads y máquina de estados

### Semana del 16 al 22 de marzo
- 22 de marzo: Implementación de la interfaz de finalización de juego
- 20 de marzo:
    - Ajustes y adiciones en el sistema de shaders (resaltado, silueta y pixelado)
    - Optimizaciones en los scripts de dados y rocas
- 18 de marzo:
    - Mejoras en el comportamiento de las rocas y optimización del sistema de shaders
    - Limpieza de código innecesario y mejoras en el funcionamiento de las rocas
    - Implementación del script de utilidades generales
    - Ajustes en la lógica central de la batalla
    - Ajustes en el funcionamiento de la máquina de estados
- 17 de marzo: 
    - Actualización de la documentación técnica
    - Mejoras estructurales en el sistema de batalla
    - Actualización de la banda sonora y gestión de música

### Semana del 09 al 15 de marzo
- 15 de marzo:
    - Integración de la rama de desarrollo `port-andres` a `main`
    - Implementación de nuevas funcionalidades en la interfaz de batalla
- 11 de marzo:
    - Adición de funciones avanzadas e interfaz para el sistema de batalla
    - Inclusión de nuevos elementos de juego
- 09 de marzo: Actualización de archivos ignorados en el control de versiones (`.gitignore`)
- 09 de marzo:
    - Implementación de movimiento ondulatorio en las cartas y corrección de bugs en los dados
    - Instalación e integración del plugin VectorDisplay2D

### Semana del 02 al 08 de marzo
- 08 de marzo: Aplicación de mejoras menores de estabilidad
- 03 de marzo:
    - Actualización de la documentación del proyecto
    - Desarrollo parcial del sistema de dados e interfaz de batalla
    - Actualización de la demostración del sistema de cartas
    - Mejoras visuales en la interfaz del selector de equipos

### Semana del 23 de febrero al 01 de marzo
- 01 de marzo:
    - Implementación de la demo de visualización de baraja en pantalla
    - Adición de nuevos elementos y diseño de nuevas cartas
    - Actualización del sistema de diálogos (DialogueManager)

---

## Febrero de 2026

### Semana del 23 de febrero al 01 de marzo
- 26 de febrero: Actualización de la guía de contribución (CONTRIBUTING.md)

### Semana del 09 al 15 de febrero
- 10 de febrero:
    - Estandarización del código mediante el cambio a tabuladores
    - Implementación de la primera versión del selector de personajes y aspectos (skins)
    - Corrección de errores visuales en el aspecto del oso panda
    - Actualización del modelo del sistema de documentación
    - Adición de la sección de créditos y mejoras generales en la UI

### Semana del 02 al 08 de febrero
- 08 de febrero:
    - Conversión de la barra superior de créditos y tutorial en escenas reutilizables
    - Creación de autoloads PlayerStats y GameConstants para gestión de datos persistentes
    - Mejora en la validación de tipos para los recursos de los autoloads
- 07 de febrero:
    - Implementación de la primera versión funcional del selector de personajes
    - Mejoras visuales en la interfaz y reestructuración de recursos en autoloads
- 06 de febrero:
    - Limpieza de plugins obsoletos del proyecto
    - Integración de la rama `port-andres`
    - Desinstalación de plugins no utilizados
- 05 de febrero:
    - Actualización de los modelos 3D del proyecto
    - Mejora del sistema de depuración (debug)
    - Integración del plugin para terminal Git Bash
- 03 de febrero:
    - Implementación de sistema de diálogos y singleton para gestión de banderas (Flags)
    - Reestructuración del proyecto: referencias por UID y organización de recursos en carpeta `assets`
    - Ajustes generales y actualización de la documentación

---

## Enero de 2026

### Semana del 26 de enero al 01 de febrero
- 30 de enero:
    - Implementación de tipado fuerte, optimizaciones de rendimiento y creación del MusicManager
    - Incorporación de nuevos modelos 3D al proyecto
- 29 de enero: Adición de personajes 3D y materiales para el oso y la rana
- 28 de enero: Importación de elementos y modelos 3D iniciales
- 27 de enero:
    - Incorporación de música para los menús principales del juego
    - Integración de la rama de desarrollo `port-andres`
    - Mejoras estéticas y funcionales en la interfaz de usuario inicial
- 26 de enero:
    - Primera versión funcional de la interfaz de usuario
    - Inicio oficial del proceso de portado del proyecto
    - Configuración de compatibilidad con Godot 4.6 y personalización del motor

### Semana del 19 al 25 de enero
- 25 de enero:
    - Implementación del sistema de generación automática de documentación
    - Ajustes en la configuración de exportación para builds
    - Instalación y configuración inicial del Dialogue Manager
    - Inicialización de la estructura base del proyecto
    - Actualización de los términos de la licencia del proyecto
    - Commit inicial: creación del repositorio y estructura básica
