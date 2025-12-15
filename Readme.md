# Examen de Depuración en PyCharm

---

## **Instrucciones:**

1. Realiza un fork de este repositorio y clónalo.
1. Las respuestas a las preguntas realízalas en este Readme
2. Cada pregunta vale un punto

### Apartado 1

- Coloca un punto de interrupción **normal** en la línea donde se inicializa la lista de la serie: `serie = [0, 1]`. 
- Inicia el modo *Debug*.

**Pregunta**

1. Si la función es llamada con `n=10`, ¿cuál es el valor de la variable `n` que se visualiza en la ventana de variables del debugger justo antes de que se ejecute la línea `serie = [0, 1]`?

El valor de la variable n justo antes de ejecutar la línea serie = [0, 1] es:
n = 10

![Captura de pantalla1.png](Captura%20de%20pantalla1.png)
---

### Apartado 2

-  Asegúrate de que la llamada a la función es `print(funcion_bucle(10))`.
-  Inicia el modo *Debug* y avanza hasta que la ejecución se detenga en la línea `siguiente_numero = calcular_siguiente(serie)`.
-  Utiliza la opción de depuración adecuada para **entrar dentro** de la función `calcular_siguiente`.

**Preguntas**

1. Justo cuando el debugger se detiene dentro de la función `calcular_siguiente` por **primera vez**, ¿cuál es el valor que tiene la variable local `aux` *después* de que se ejecute la línea `aux = serie[-1] + serie[-2]`?
**(Indica el valor numérico exacto de la variable `aux` en ese momento y el nombre de la herramienta de *debugging* que utilizaste para entrar en la función).**
2. Si estuvieras dentro de la función `calcular_siguiente` y quisieras salir rápidamente sin ejecutar el resto de las líneas, volviendo al punto de llamada en `funcion_bucle`, ¿qué función del debugger deberías usar?
3. ¿Qué diferencia fundamental existe entre usar *Step Over* y *Step Into* en la línea `siguiente_numero = calcular_siguiente(serie)`?


1. El valor de aux la primera vez que se entra en calcular_siguiente es:
aux = 1
Herramienta: Step Into.
2. Para salir rápidamente de la función calcular_siguiente y volver al punto de llamada se utiliza:
Step Out
3. Diferencia entre Step Over y Step Into:

Step Over: ejecuta la línea completa sin entrar en funciones.

Step Into: entra dentro de la función llamada para depurarla paso a paso.


---

### Apartado 3

-  Cambia la llamada a la función para que el número de elementos sea mayor: `print(funcion_bucle(1000))`.
-  Establece un **Breakpoint Condicional** para que la ejecución se detenga solo cuando `siguiente_numero` sea **mayor que 20000**.

**Pregunta**

1. Cuando el *Breakpoint Condicional* se activa por **primera vez** (la primera vez que `siguiente_numero` es mayor que 20000), ¿qué longitud tiene `serie`?

La primera vez que siguiente_numero es mayor que 20000, la longitud de serie es:
24
![captura de pantalla3.png](captura%20de%20pantalla3.png)


---
