# 🏃‍♂️ Gold Rush City

![Engine](https://img.shields.io/badge/Engine-Unreal%20Engine%205-black)
![Genre](https://img.shields.io/badge/Genre-Endless%20Runner-orange)
![Platform](https://img.shields.io/badge/Platform-Windows%20(PC)-blue)
![Input](https://img.shields.io/badge/Input-Keyboard%20%7C%20Gamepad-green)
![Status](https://img.shields.io/badge/Status-Prototype%20Demo-yellow)

**Gold Rush City** es un prototipo de "Infinite Runner" de alta velocidad desarrollado en Unreal Engine 5. El proyecto demuestra la implementación de mecánicas de generación procedural de niveles, optimización de recursos en tiempo real y lógica de juego a través de Visual Scripting (Blueprints).

![Gameplay Level](screenshots/GoldRushCity_level.jpg)

---

## 🚀 Características Técnicas

### 1. Generación Procedural (Level Streaming)
El juego no utiliza un mapa estático infinito. En su lugar, implementa un sistema de **spawning dinámico** de "tiles" (tramos de nivel) que se generan frente al jugador y se destruyen al quedar atrás.
* **Beneficio:** Mantiene el uso de memoria RAM estable y bajo, permitiendo que el juego corra indefinidamente sin caídas de rendimiento.

### 2. Lógica en Blueprints
Toda la jugabilidad fue programada utilizando el sistema de nodos de UE5.
* **Player Controller:** Manejo de Inputs híbridos (Teclado/Mando), física de salto, dash y mecánicas de ataque (Slash).
* **Game Loop:** Gestión de estados de juego (Menú -> Run -> Game Over -> Restart).
* **Score System:** Cálculo de puntaje basado en distancia y recolección de items.

![Blueprints Logic](screenshots/GoldRushCity_bp.jpg)

### 3. Interfaz de Usuario (UMG)
Implementación de Widgets para el HUD y menús interactivos.
* Menú Principal con navegación.
* HUD en tiempo real (Puntaje/Distancia).

![Main Menu](screenshots/GoldRushCity_menu.jpg)

---

## 🎮 Controles

El juego soporta tanto teclado clásico como Gamepad (PlayStation/Xbox/Genérico).

| Acción | Teclado ⌨️ | Gamepad 🎮 |
| :--- | :--- | :--- |
| **Moverse (Carriles)** | Flechas Izquierda / Derecha | D-Pad o Stick Izquierdo |
| **Saltar** | Barra Espaciadora | Botón X (o equivalente) |
| **Atacar (Slash)** | Ctrl Izquierdo | Gatillo R2 (RT) |

---

## 🕹️ Cómo jugar con Mando (Steam Input)

Para garantizar la compatibilidad con tu control (PS4, PS5, Xbox, etc.), se recomienda ejecutar el juego a través de **Steam**:

1.  Abre Steam en tu PC.
2.  Ve al menú **"Juegos"** -> **"Añadir un producto que no es de Steam a mi biblioteca..."**.
3.  Busca y selecciona el archivo `GoldRushCity.exe` que descargaste.
4.  Inicia el juego desde tu biblioteca de Steam.

*Esto activará **Steam Input**, permitiendo que el juego reconozca los inputs de tu mando correctamente.*

---

## 📥 Descarga e Instalación

Este proyecto ha sido empaquetado como un ejecutable standalone para Windows.

1.  Ve a la sección de **[Releases](../../releases)** de este repositorio.
2.  Descarga el archivo `.zip` de la última versión (v1.0).
3.  Descomprime el archivo.
4.  Ejecuta `GoldRushCity.exe`.

*(Nota: Al ser un ejecutable no firmado, Windows podría pedir confirmación para ejecutarlo. Es seguro).*

---

> **Autor:** Raúl Héctor Cámara Carreón
>

