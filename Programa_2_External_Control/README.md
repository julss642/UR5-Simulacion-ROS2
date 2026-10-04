# Programa 2 – External Control

Programa desarrollado en PolyScope para establecer la comunicación entre el UR5 simulado y ROS2 mediante External Control.

## Secuencia del programa

- Activación de la salida digital DO[0].
- Popup de aviso al usuario.
- Espera de 5 segundos.
- Activación de External Control.

Posteriormente, desde ROS2 se establece la comunicación con el robot y se ejecuta una trayectoria articular mediante el controlador `scaled_joint_trajectory_controller`.
