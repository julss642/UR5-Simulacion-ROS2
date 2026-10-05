# UR5-Simulacion-ROS2

Repositorio correspondiente a la actividad de simulación y control del robot colaborativo UR5 mediante URSim, PolyScope y ROS2.

## Contenido

### Programa 1 – Trayectorias de las iniciales

Programa desarrollado en PolyScope para generar las trayectorias correspondientes a las iniciales de los integrantes del grupo:

- L – Leydi Solorza
- S – Leydi Solorza
- A – Alejandro Huertas
- H – Alejandro Huertas

Cada trayectoria cuenta con un Popup previo que identifica la letra que será simulada.

### Programa 2 – External Control

Programa desarrollado para establecer la comunicación entre el UR5 simulado y ROS2 mediante External Control.

La secuencia incluye:

- Activación de la salida digital DO[0].
- Mensaje de aviso mediante Popup.
- Espera de 5 segundos.
- Transferencia del control mediante External Control.
- Ejecución de una trayectoria articular desde ROS2.

### Programa 3 – Pick and Place

Programa correspondiente a la rutina de Pick and Place.

La rutina implementa dos puntos de recogida y sus respectivas trayectorias de transporte y entrega, incluyendo puntos intermedios sobre las posiciones de recogida y destino, así como la activación y desactivación del efector mediante salidas digitales.

Al finalizar las rutinas, el programa espera la señal de una entrada digital para continuar con la ejecución.

## Herramientas utilizadas

- Universal Robots UR5
- URSim
- PolyScope
- ROS2 Humble
- External Control URCap
- Docker
