# unidad 3 continuidad y derivabilidad

## limites (llegamos aqui otra vez maldita sea)

en una, dos o tres variables, el concepto de límite es fundamental para entender el comportamiento de las funciones cerca de ciertos puntos. por ejemplo, el límite de una función f(x) cuando x se acerca a un valor a se denota como:

```math
    \lim_{x \to a} f(x)
``` 

la definicion formal es la siguiente:

```math
\forall \varepsilon > 0,\ \exists\delta = \delta(\varepsilon) > 0\ \text{tal que, si}\ 0 < |x - x_0| < \delta,\ \text{entonces}\ |f(x) - L| < \varepsilon.
```
si lo miras con ganas esto se puede expresar como existen un l (limite) y un epsilon (distancia al limite) tales que 

```math
L -\varepsilon < f(x) < L + \varepsilon
```

es decir que f(x) se encuentra dentro de un intervalo alrededor de L, y que ese intervalo se puede hacer tan pequeño como queramos al elegir un delta suficientemente pequeño. esto significa que a medida que x se acerca a x0, f(x) se acerca a L, lo que es la esencia del concepto de límite. 

en otras palabras y resumidamente, el limite de consiste en ir acotando desde arriba o abajo de la funcion en el punto un intervalo cada vez mas pequeño, y si ese intervalo se puede acotar cada vez mas cerca de un numero L, entonces decimos que el limite de f(x) cuando x se acerca a x0 es L. este concepto es fundamental para entender la continuidad, la derivabilidad y otros aspectos importantes de las funciones en análisis matemático.

concretamente para que una funcion sea continua en un punto x0, es necesario que el límite de la función cuando x se acerca a x0 sea igual al valor de la función en ese punto, es decir:

```math
\lim_{x \to x_0} f(x) = f(x_0)
```
esto significa que la función no tiene saltos, ni agujeros, ni discontinuidades en ese punto, y que el valor de la función en ese punto coincide con el valor al que se acerca la función a medida que x se acerca a x0. esta es una condición esencial para que una función sea continua en un punto dado.

para el caso de campos escalares es decir de varias variables, el concepto de límite se extiende de manera similar. por ejemplo, para una función f(x, y), el límite cuando (x, y) se acerca a un punto (x0, y0) se denota como:

```math
\lim_{(x, y) \to (x_0, y_0)} f(x, y)
``` 
y la definición formal es análoga a la de una variable:

```math
\forall \varepsilon > 0,\ \exists\delta = \delta(\varepsilon) > 0\ \text{tal que, si}\ 0 < \sqrt{(x - x_0)^2 + (y - y_0)^2} < \delta,\ \text{entonces}\ |f(x, y) - L| < \varepsilon.
```
esto significa que a medida que el punto (x, y) se acerca al punto (x0, y0), la función f(x, y) se acerca al valor L, lo que es la esencia del concepto de límite en varias variables. al igual que en el caso de una variable, el concepto de límite es fundamental para entender la continuidad, la derivabilidad y otros aspectos importantes de las funciones de varias variables en análisis matemático.

## que pasa en funciones vectoriales?

en el caso de funciones vectoriales, el concepto de límite se extiende de manera similar. por ejemplo, para una función vectorial r(t) = (x(t), y(t), z(t)), el límite cuando t se acerca a un valor t0 se denota como:

```math
\lim_{t \to t_0} \mathbf{r}(t) = \mathbf{L}
```

donde cada componente de la función vectorial se acerca a un valor específico.


## como calcular el limite de una funcion de una variable

tenemos varias formas de calcular un limite

1. evaluacion directa: si la función es continua en el punto al que se acerca, simplemente evaluamos la función en ese punto para obtener el límite.

```math
\lim_{x \to a} f(x) = f(a)
```

2. cambio de variable: a veces, al hacer un cambio de variable, podemos simplificar la función y calcular el límite de manera más fácil o usar limite conocido:

```math
\lim_{x \to 0} \frac{\sin(x)}{x} = \lim_{u \to 0} \frac{\sin(u)}{u} = 1
```
3. factorización: si la función tiene una forma que se puede factorizar, podemos factorizarla para simplificarla y luego calcular el límite.

```math
\lim_{x \to 2} \frac{x^2 - 4}{x - 2} = \lim_{x \to 2} \frac{(x - 2)(x + 2)}{x - 2} = \lim_{x \to 2} (x + 2) = 4
```
4. racionalización: si la función tiene una forma que se puede racionalizar, podemos racionalizarla para simplificarla y luego calcular el límite.

```math
\lim_{x \to 0} \frac{\sqrt{x + 1} -
1}{x} = \lim_{x \to 0} \frac{(\sqrt{x + 1} - 1)(\sqrt{x + 1} + 1)}{x(\sqrt{x + 1} + 1)} = \lim_{x \to 0} \frac{x}{x(\sqrt{x + 1} + 1)} = \lim_{x \to 0} \frac{1}{\sqrt{x + 1} + 1} = \frac{1}{2}
```
5. regla de l'hôpital: si el límite tiene una forma indeterminada como 0/0 o ∞/∞, podemos aplicar la regla de l'hôpital, que establece que el límite de una función en una forma indeterminada se puede calcular tomando la derivada del numerador y del denominador por separado y luego calculando el límite de la nueva función.

```math
\lim_{x \to 0} \frac{\sin(x)}{x} = \lim_{x \to 0} \frac{\cos(x)}{1} = 1
``` 
6. teorema del sandwich: si la función que queremos calcular el límite está acotada por dos funciones que tienen el mismo límite en un punto dado, entonces la función también tiene ese mismo límite en ese punto.

```math
    \text{Si}\ g(x) \leq f(x) \leq h(x)     \text{y}\ \lim_{x \to a} g(x) = \lim_{x \to a} h(x) = L,\ \text{entonces}\ \lim_{x \to a} f(x) = L
``` 
7. infinitesimo por acotado: si la función que queremos calcular el límite se puede expresar como el producto de un infinitesimal y una función acotada, entonces el límite de la función es cero.

```math
\text{Si}\ f(x) = g(x)h(x),\ \text{donde}\ \lim_{x \to a} g(x) = 0\ \text{y}\ h(x)\ \text{es acotada},\ \text{entonces}\ \lim_{x \to a} f(x) = 0
```

### algunos limites conocidos

```math
\lim_{x \to 0} \frac{\sin(x)}{x} = 1
```

```math
\lim_{x \to 0} \frac{1 - \cos(x)}{x^2} = \frac{1}{2}
```

```math
\lim_{x \to 0} \frac{e^x - 1}{x} = 1
```

```math
\lim_{x \to 0} \frac{\ln(1 + x)}{x} = 1
```


## como calcular el limite de una funcion de varias variables

el cálculo de límites de funciones de varias variables puede ser más complejo que el de funciones de una variable, ya que el comportamiento de la función puede variar dependiendo de la dirección desde la cual se acerca al punto en cuestión. sin embargo, existen algunas técnicas y estrategias que pueden ayudar a calcular estos límites:

1. Evaluación directa: si la función es continua en el punto al que se acerca, simplemente evaluamos la función en ese punto para obtener el límite.

```math
\lim_{(x, y) \to (a, b)} f(x, y) = f(a, b)
```

2. Cambio de variable: a veces, al hacer un cambio de variable, podemos simplificar la función y calcular el límite de manera más fácil o usar límites conocidos.

```math
\lim_{(x, y) \to (0, 0)} \frac{\sin(x^2 + y^2)}{x^2 + y^2} = \lim_{r \to 0} \frac{\sin(r^2)}{r^2} = 1
``` 

3. Racionalización: si la función tiene una forma que se puede racionalizar, podemos racionalizarla para simplificarla y luego calcular el límite.

```math
\lim_{(x, y) \to (0, 0)} \frac{\sqrt{x^2 + y^2 + 1} - 1}{x^2 + y^2} = \lim_{(x, y) \to (0, 0)} \frac{(\sqrt{x^2 + y^2 + 1} - 1)(\sqrt{x^2 + y^2 + 1} + 1)}{(x^2 + y^2)(\sqrt{x^2 + y^2 + 1} + 1)} = \lim_{(x, y) \to (0, 0)} \frac{1}{\sqrt{x^2 + y^2 + 1} + 1} = \frac{1}{2}
```

4. Regla de l'Hôpital: si el límite tiene una forma indeterminada como 0/0 o ∞/∞, podemos aplicar la regla de l'Hôpital, que establece que el límite de una función en una forma indeterminada se puede calcular tomando la derivada parcial del numerador y del denominador por separado y luego calculando el límite de la nueva función.

```math
\lim_{(x, y) \to (0, 0)} \frac{\sin(x^2 + y^2)}{x^2 + y^2} = \lim_{(x, y) \to (0, 0)} \frac{2x\cos(x^2 + y^2) + 2y\cos(x^2 + y^2)}{2x + 2y} = \lim_{(x, y) \to (0, 0)} \frac{2(x + y)\cos(x^2 + y^2)}{2(x + y)} = \lim_{(x, y) \to (0, 0)} \cos(x^2 + y^2) = 1
```     

5. Teorema del sándwich: si la función que queremos calcular el límite está acotada por dos funciones que tienen el mismo límite en un punto dado, entonces la función también tiene ese mismo límite en ese punto.

```math
\text{Si}\ g(x, y) \leq f(x, y) \leq h(x, y)     \text{y}\ \lim_{(x, y) \to (a, b)} g(x, y) = \lim_{(x, y) \to (a, b)} h(x, y) = L,\ \text{entonces}\ \lim_{(x, y) \to (a, b)} f(x, y) = L
```

6. Infinitesimal por acotado: si la función que queremos calcular el límite se puede expresar como el producto de un infinitesimal y una función acotada, entonces el límite de la función es cero.

```math
\text{Si}\ f(x, y) = g(x, y)h(x, y),\ \text{donde}\ \lim_{(x, y) \to (a, b)} g(x, y) = 0\ \text{y}\ h(x, y)\ \text{es acotada},\ \text{entonces}\ \lim_{(x, y) \to (a, b)} f(x, y) = 0
```

por ultimo si todo falla la mejor opcion, es demostrar que el limite no existe, para eso se pueden usar diferentes caminos de aproximacion al punto en cuestion, y si el limite es diferente dependiendo del camino de aproximacion, entonces el limite no existe.

```math
\text{Si}\ \lim_{(x, y) \to (a, b)} f(x, y) \neq \lim_{(x, y) \to (a, b)} f(x, y),\ \text{entonces}\ \lim_{(x, y) \to (a, b)} f(x, y) \text{no existe}
```

las mas comunes son aproximacion por lineas rectas, es decir, aproximar al punto (a, b) por diferentes lineas rectas que pasen por ese punto, y si el limite es diferente dependiendo de la linea recta de aproximacion, entonces el limite no existe.

```math
\text{Si}\ \lim_{t \to 0} f(a + t, b + mt) \neq \lim_{t \to 0} f(a + t, b + nt),\ \text{para}\ m \neq n,\ \text{entonces}\ \lim_{(x, y) \to (a, b)} f(x, y) \text{no existe}
```

tambien se puede aproximar al punto (a, b) por curvas, es decir, aproximar al punto (a, b) por diferentes curvas que pasen por ese punto, y si el limite es diferente dependiendo de la curva de aproximacion, entonces el limite no existe.

```math
\text{Si}\ \lim_{t \to 0} f(a + t^2, b + t^3) \neq \lim_{t \to 0} f(a + t^3, b + t^2),\ \text{entonces}\ \lim_{(x, y) \to (a, b)} f(x, y) \text{no existe}
``` 

## campo escalar continuo

un campo escalar es una función que asigna un valor escalar a cada punto en el espacio. por ejemplo, la temperatura en una habitación puede ser representada como un campo escalar, donde cada punto en la habitación tiene un valor de temperatura asociado. un campo escalar es continuo si para cada punto en el espacio, el límite del campo escalar cuando se acerca a ese punto es igual al valor del campo escalar en ese punto. esto significa que no hay saltos ni discontinuidades en el campo escalar, y que el valor del campo escalar en un punto dado coincide con el valor al que se acerca el campo escalar a medida que nos acercamos a ese punto.

## otras propiedades de la continuidad

- la suma de dos campos escalares continuos es un campo escalar continuo.

- el producto de un campo escalar continuo por una constante es un campo escalar continuo.

- el producto de dos campos escalares continuos es un campo escalar continuo.

- el cociente de dos campos escalares continuos es un campo escalar continuo, siempre y cuando el denominador no sea cero.

### funciones tipicamente continuas (en su dominio)

- polinomios: los polinomios son funciones continuas en todo el espacio, ya que no tienen puntos de discontinuidad.
- funciones trigonometricas: las funciones trigonométricas como el seno, coseno y tangente son continuas en todo su dominio, que es el conjunto de los números reales.
- funciones racionales: las funciones racionales, que son cocientes de polinomios, son continuas en su dominio, que es el conjunto de los números reales excepto los puntos donde el denominador es cero.
- logaritmos: las funciones logarítmicas son continuas en su dominio, que es el conjunto de los números reales positivos.
- funciones exponenciales: las funciones exponenciales son continuas en todo su dominio, que es el conjunto de los números reales.
- funciones radicales: las funciones radicales, como la raíz cuadrada, son continuas en su dominio, que es el conjunto de los números reales no negativos.

asi como las composiciones de funciones continuas son continuas, es decir, si f y g son funciones continuas, entonces la función compuesta f(g(x)) también es continua en su dominio.


## derivadas de campos escalares

entendemos que funciones de una variable, la derivada de una función f(x) en un punto x0 se define como el límite:

```math
f'(x_0) = \lim_{h \to 0} \frac{f(x_0 + h) - f(x_0)}{h}
```

que quiere decir que la derivada de una función en un punto dado representa la tasa de cambio instantánea de la función en ese punto, o la pendiente de la tangente a la curva de la función en ese punto. esta definición se puede extender a funciones de varias variables, donde la derivada se define como el límite del cociente incremental en cada dirección, que existas ese numero indica que la función es diferenciable en ese punto, representa la pendiente de la tangente a la superficie de la función en ese punto.

en el caso de funciones de varias variables, vamos a tener varias derivadas parciales, una para cada variable, que se denotan como:

```math
\frac{\partial f}{\partial x}, \quad \frac{\partial f}{\partial y}, \quad \frac{\partial f}{\partial z}
``` 

aca es donde entran las derivadas direccionales

## derivada direccional

el asunto en mas de una variable es que podemos "movernos" en diferentes direcciones, cada una de estas direcciones es representable por un versor v, y la derivada direccional de una función f en la dirección de un versor v se define como el límite:

```math
D_v f((x_0, y_0)) = \lim_{h \to 0} \frac{f(x_0 + hv_x, y_0 + hv_y) - f(x_0, y_0)}{h}
```

si este limite existe y es finito, entonces decimos que la función f es diferenciable en el punto (x0, y0) y que la derivada direccional de f en la dirección de v en el punto (x0, y0) es igual a ese límite. esta derivada direccional representa la tasa de cambio de la función f en la dirección del versor v en el punto (x0, y0), y es una medida de cómo cambia la función a medida que nos movemos en esa dirección específica.

## derivadas parciales

las derivadas parciales de una función de varias variables se definen como las derivadas direccionales en las direcciones de los ejes coordenados. por ejemplo, la derivada parcial de una función f(x, y) con respecto a x se define como:

```math
\frac{\partial f}{\partial x}(x_0, y_0) = \lim_{h \to 0} \frac{f(x_0 + h, y_0) - f(x_0, y_0)}{h}
```

## derivadas de orden superior

las derivadas de orden superior de una función de varias variables se definen como las derivadas parciales de las derivadas parciales. por ejemplo, la segunda derivada parcial de una función f(x, y) con respecto a x se define como:

```math
\frac{\partial^2 f}{\partial x^2}(x_0, y_0) = \lim_{h \to 0} \frac{\frac{\partial f}{\partial x}(x_0 + h, y_0) - \frac{\partial f}{\partial x}(x_0, y_0)}{h}
```

de mas esta decir que no es necesario calcular todas las derivadas por definicion, ya que si la función es suficientemente suave, entonces las derivadas parciales de orden superior pueden ser calculadas a partir de las derivadas parciales de orden inferior utilizando las reglas de derivación.



## teorema de Schwarz

el teorema de Schwarz establece que si una función f(x, y) tiene derivadas parciales de segundo orden continuas en un punto dado, entonces las derivadas parciales mixtas de segundo orden son iguales en ese punto. es decir, si f tiene derivadas parciales de segundo orden continuas en un punto (x0, y0), entonces:

```math
\frac{\partial^2 f}{\partial x \partial y}(x_0, y_0) = \frac{\partial^2 f}{\partial y \partial x}(x_0, y_0)
```

## derivadas maximas, minimas y nulas de un campo escalar


sabemos que las derivadas parciales de una función de varias variables representan la tasa de cambio (velocidad de crecimiento o decrecimiento) de la función en cada dirección. entonces, si queremos encontrar los puntos donde la función alcanza un máximo, mínimo o punto de inflexión, debemos buscar los puntos donde las derivadas parciales, por ejemeplo sabemos que la direccion maxima puede obtenerse a partir del gradiente, que es un vector que contiene las derivadas parciales de la función en cada dirección. el gradiente de una función f(x, y) se denota como:

```math
\nabla f(x, y) = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right)
```


sabemos entonces que si un campo es diferenciable en un punto entonces se puede calcular la derivada direccional en la direccion de cualquier versor v, y esa derivada direccional se puede calcular como el producto escalar entre el gradiente de la funcion y el versor v:

```math
D_v f((x_0, y_0)) = \nabla f(x_0, y_0) \cdot \mathbf{v}
``` 

del producto escalar sabemos que el valor máximo se obtiene cuando los dos vectores son paralelos, es decir, cuando el versor v apunta en la misma dirección que el gradiente de la función, quedando entonces:

```math
D_v f((x_0, y_0)) = |\nabla f(x_0, y_0)| \cdot |\mathbf{v}| \cdot \cos(0) = |\nabla f(x_0, y_0)|
```

entonces basandonos en los angulos sabesmos que si

- cos(0) = 1, entonces la derivada direccional es máxima y la función crece más rápidamente en esa dirección.

- cos(π) = -1, entonces la derivada direccional es mínima y la función decrece más rápidamente en esa dirección.

- cos(π/2) = 0, entonces la derivada direccional es nula y la función no cambia en esa dirección.

por lo tanto entonces la derivada direccionala maxima se obtiene en la dirección del gradiente de la función, la derivada direccional mínima se obtiene en la dirección opuesta al gradiente de la función, y la derivada direccional nula se obtiene en cualquier dirección perpendicular al gradiente de la función. 

```math
\text{Dirección de crecimiento máximo:}\ \mathbf{v} = \frac{\nabla f(x_0, y_0)}{|\nabla f(x_0, y_0)|}

```

```math

\text{Dirección de crecimiento mínimo:}\ \mathbf{v} = -\frac{\nabla f(x_0, y_0)}{|\nabla f(x_0, y_0)|}

```

```math 

\text{Dirección de crecimiento nulo:}\ \mathbf{v} \cdot \nabla f(x_0, y_0) = 0
```

## superficies parametrizadas

podemos enteder una superficie parametrizada como una función vectorial que asigna un vector a cada punto en un dominio dado. por ejemplo, una superficie parametrizada en tres dimensiones se puede representar como:

```math
\mathbf{X}(t) = (x(t), y(t), z(t))
```

la parametrizacion de una superficie nos permite describir la superficie de manera más flexible y general, se dice entonces que la misma es regular en un punto dado si el vector tangente a la superficie en ese punto no es nulo, es decir, si el vector tangente a la superficie en ese punto tiene una magnitud diferente de cero. esto significa que la superficie no tiene puntos de singularidad o puntos donde la superficie se "pliega" sobre sí misma, lo que permite que la superficie tenga una estructura suave y bien definida en ese punto.

```math
\text{Una superficie parametrizada es regular en un punto } t_0 \text{ si } \mathbf{X}'(t_0) \neq \mathbf{0}
```

de este modo una funcion vectorial de dos parametros, es decir, una funcion de la forma:

```math
\mathbf{X}(u, v) = (x(u, v), y(u, v), z(u, v))
```
representa una superficie parametrizada en tres dimensiones, donde cada punto en la superficie se describe mediante dos parámetros u y v. la regularidad de esta superficie se determina por la condición de que los vectores tangentes a la superficie, que se obtienen al tomar las derivadas parciales de la función vectorial con respecto a los parámetros u y v, no sean nulos. es decir, la superficie es regular en un punto dado si los vectores tangentes a la superficie en ese punto tienen una magnitud diferente de cero.

```math
\text{Una superficie parametrizada es regular en un punto } (u_0, v_0) \text{ si } \mathbf{X}_u(u_0, v_0) \times \mathbf{X}_v(u_0, v_0) \neq \mathbf{0}
```

### plano tangente a una superficie parametrizada

el plano tangente a una superficie parametrizada en un punto dado se define como el plano que es tangente a la superficie en ese punto. para encontrar el plano tangente a una superficie parametrizada, primero debemos calcular los vectores tangentes a la superficie en ese punto, que se obtienen al tomar las derivadas parciales de la función vectorial con respecto a los parámetros u y v. luego, el plano tangente se puede describir utilizando estos vectores tangentes y el punto de tangencia.

si la superficie parametrizada se describe mediante la función vectorial:

```math
\mathbf{X}(u, v) = (x(u, v), y(u, v), z(u, v))
```

entonces los vectores tangentes a la superficie en un punto dado (u0, v0) se pueden calcular como:

```math
\mathbf{X}_u(u_0, v_0) = \left( \frac{\partial x}{\partial u}(u_0, v_0), \frac{\partial y}{\partial u}(u_0, v_0), \frac{\partial z}{\partial u}(u_0, v_0) \right)
``` 

```math
\mathbf{X}_v(u_0, v_0) = \left( \frac{\partial x}{\partial v}(u_0, v_0), \frac{\partial y}{\partial v}(u_0, v_0), \frac{\partial z}{\partial v}(u_0, v_0) \right)
```

luego, el plano tangente a la superficie en el punto (u0, v0) se puede describir utilizando estos vectores tangentes y el punto de tangencia, que se obtiene al evaluar la función vectorial en ese punto:

```math
\mathbf{X}(u_0, v_0) = (x(u_0, v_0), y(u_0, v_0), z(u_0, v_0))
``` 
entonces, el plano tangente a la superficie en el punto (u0, v0) se puede describir utilizando la ecuación del plano:

```math
\mathbf{n} \cdot (\mathbf{r} - \mathbf{X}(u_0, v_0)) = 0
``` 

### rectas tangentes a una superficie parametrizada

las rectas tangentes a una superficie parametrizada en un punto dado se definen como las líneas que son tangentes a la superficie en ese punto. para encontrar las rectas tangentes a una superficie parametrizada, primero debemos calcular los vectores tangentes a la superficie en ese punto, que se obtienen al tomar las derivadas parciales de la función vectorial con respecto a los parámetros u y v. luego, las rectas tangentes se pueden describir utilizando estos vectores tangentes y el punto de tangencia.

si la superficie parametrizada se describe mediante la función vectorial:

```math
\mathbf{X}(u, v) = (x(u, v), y(u, v), z(u, v))
```
entonces los vectores tangentes a la superficie en un punto dado (u0, v0) se pueden calcular como:

```math
\mathbf{X}_u(u_0, v_0) = \left( \frac{\partial x}{\partial u}(u_0, v_0), \frac{\partial y}{\partial u}(u_0, v_0), \frac{\partial z}{\partial u}(u_0, v_0) \right)
```
```math
\mathbf{X}_v(u_0, v_0) = \left( \frac{\partial x}{\partial v}(u_0, v_0), \frac{\partial y}{\partial v}(u_0, v_0), \frac{\partial z}{\partial v}(u_0, v_0) \right)
```
luego, las rectas tangentes a la superficie en el punto (u0, v0) se pueden describir utilizando estos vectores tangentes y el punto de tangencia, que se obtiene al evaluar la función vectorial en ese punto:

```math
\mathbf{X}(u_0, v_0) = (x(u_0, v_0), y(u_0, v_0), z(u_0, v_0))
```

entonces, las rectas tangentes a la superficie en el punto (u0, v0) se pueden describir utilizando la ecuación de la recta:

```math
\mathbf{r}(t) = \mathbf{X}(u_0, v_0) + t \mathbf{X}_u(u_0, v_0)
```
```math
\mathbf{r}(t) = \mathbf{X}(u_0, v_0) + t \mathbf{X}_v(u_0, v_0)
```

