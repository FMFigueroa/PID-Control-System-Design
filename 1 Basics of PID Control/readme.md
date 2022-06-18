## 1 Basics of PID Control

### Basics of PID Control

Hay cuatro tipos de controladores que pertenecen a la familia de controladores PID:

- controlador proporcional (P)
- controlador proporcional más integral (PI)
- controlador proporcional más derivativo (PD)
- controlador proporcional más integral más derivativo (PID) controlador.

Para comprender las funciones de los controladores, en esta sección analizaremos cada una de las estructuras y los parámetros del controlador PID. De las discusiones, estableceremos algunos conocimientos básicos sobre cómo usar estos controladores en varios aplicaciones.

### Proportional Controller

El controlador más simple es el controlador proporcional. Con este término proporcional, el
la señal de control de retroalimentación u(t) se calcula en proporción al error de retroalimentación e(t) con
la formula,

    u(t) = Kp * e(t)

diagrama de bloques para la configuración de control de retroalimentación de lazo cerrado:

![](./imgs/the%20proportional%20controller.png)

- Kc es la ganancia proporcional.
- el error de realimentación e(t), es la diferencia entre la señal de referencia r(t) y la señal de salida y(t).

  (e(t) = r(t) − y(t)).

- R(s) es la señal de referencia.
- E(s) el error de retroalimentación.
- U(s) es la señal de control.
- Y(s) es la señal de salida.
- G(s) representa la función de transferencia de Laplace.

Todas estan representadas como las transformadas de Laplace respectivamente.

Debido a su simplicidad, el controlador proporcional se usa a menudo en los casos en que hay poca información disponible sobre el sistema y el rendimiento de control requerido en la operación en estado estacionario no es exigente.
Como el controlador solo involucra un parámetro por determinar, es posible elegir Kc sin información detallada sobre el sistema.

Una de las limitaciones de un controlador proporcional simple es que el error de estado estable
del sistema de control de circuito cerrado no se eliminará por completo.
