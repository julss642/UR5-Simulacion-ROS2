# Programa 3 – Pick and Place

Rutina de Pick and Place desarrollada para el robot UR5 en el entorno de simulación URSim y PolyScope.

## Descripción

El programa realiza la recogida y entrega de dos piezas simuladas mediante dos puntos de recogida diferentes.

La secuencia incluye:

- Dos posiciones de recogida: `recogida_a` y `recogida_b`.
- Activación de `DO[0]` para representar el agarre.
- Puntos intermedios sobre las posiciones de recogida y entrega.
- Transporte de cada pieza hasta su respectivo destino.
- Desactivación de `DO[0]` para representar la liberación.
- Espera de confirmación mediante `digital_in[0]` para continuar con un nuevo ciclo.

## Entorno

- Robot: Universal Robots UR5 CB3.
- Simulador: URSim.
- Interfaz de programación: PolyScope.

## Secuencia

```text
Recogida A → Transporte → Entrega A
                    ↓
Recogida B → Transporte → Entrega B
                    ↓
       Espera de confirmación
