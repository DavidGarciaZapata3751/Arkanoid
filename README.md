# Arkanoid Game - Jack Language Implementation

![Arkanoid](https://img.shields.io/badge/Language-Jack-blue)
![Platform](https://img.shields.io/badge/Platform-Nand2Tetris-green)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 📝 Descripción

Implementación del clásico juego Arkanoid en lenguaje Jack para la plataforma Nand2Tetris. El jugador controla una paleta que debe rebotar una bola para destruir todos los ladrillos en la pantalla, mientras evita que bombas caigan sobre la paleta.

## 👥 Integrantes del Grupo

- **David García**
- **Mariana Carrasquilla**
- **Valentina Zapata**

## 🎮 Características del Juego

### Mecánicas Principales
- **Paleta móvil**: Controlada por el jugador con las flechas izquierda/derecha
- **Bola rebotante**: Destruye ladrillos al impactarlos
- **Ladrillos**: 40 ladrillos distribuidos en 5 filas × 8 columnas
- **Bombas**: Caen desde los ladrillos destruidos
- **Sistema de vidas**: 3 vidas iniciales
- **Puntuación**: 10 puntos por cada ladrillo destruido
- **Dificultad progresiva**: La paleta se reduce con cada rebote de la bola

### Controles
- **Flecha Izquierda (←)**: Mover paleta a la izquierda
- **Flecha Derecha (→)**: Mover paleta a la derecha
- **Q**: Salir del juego

### Condiciones de Victoria/Derrota
- **Victoria**: Destruir todos los 40 ladrillos
- **Derrota**: Perder las 3 vidas (bola cae o bomba impacta la paleta)

## 📁 Estructura del Proyecto

```
Arkanoid/
│
├── ArkanoidGame.jack    # Lógica principal del juego y loop de ejecución
├── Main.jack            # Punto de entrada del programa
├── Paddle.jack          # Clase de la paleta controlada por el jugador
├── Ball.jack            # Clase de la bola rebotante
├── Brick.jack           # Clase de los ladrillos destruibles
├── Bomb.jack            # Clase de las bombas que caen
└── README.md            # Este archivo
```

## 🚀 Cómo Compilar y Ejecutar

### Usando la Interfaz Gráfica de Nand2Tetris online IDE

1. **Abre el JackCompiler:**
   - desde el IDE de nand2tetris ir a la sección de Jack compiler.

2. **Compila el proyecto:**
   - Haz clic en la carpeta que aparece al lado de **"Source"**
   - Busca entre tu directorio la carpeta `Arkanoid` y seleccionala.
   - Da click en `Compile`, el compilador generará automáticamente los archivos `.vm`.

3. **Ejecuta el VMEmulator:**
   - luego de compilar, dar click en el botón de al lado que dice `Run`, esto abrirá la interfaz del VMEmulator.
   - Configura la velocidad de ejecución a "Fast" para mejor experiencia.
   - Haz clic en **Run**.


## 📊 Características Técnicas

### Arquitectura del Código

- **Programación Orientada a Objetos**: Cada elemento del juego es una clase independiente
- **Gestión de memoria**: Uso eficiente de arrays y objetos
- **Detección de colisiones**: AABB (Axis-Aligned Bounding Box) para bombas y bola
- **Física simple**: Sistema de rebote con inversión de velocidad

### Limitaciones de la Plataforma

- Pantalla: 512×256 píxeles (blanco y negro)
- Sin soporte para sprites o gráficos avanzados
- Velocidad limitada por el VMEmulator

## 📚 Documentación Adicional

Cada archivo `.jack` contiene comentarios extensos que explican:
- Propósito de cada clase y método
- Algoritmos de detección de colisión
- Flujo de ejecución del juego
- Gestión de memoria y recursos

### Conceptos Aplicados
- Diseño de lenguajes de programación
- Compiladores y máquinas virtuales
- Arquitectura de computadoras
- Gestión de memoria
- Programación orientada a objetos

## 📜 Licencia

Este proyecto es de código abierto y fue desarrollado con fines educativos como parte del curso de Organización de Computadores de la universidad EAFIT.

## 📽️ Video explicativo

link: https://youtu.be/muJYAxBfVxc?si=5W5QPhk5oz-nwauq
