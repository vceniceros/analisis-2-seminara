# unidad 2 (funciones vectoriales, curvas y rectas tangentes)

## funciones vectoriales

las funciones vectoriales son funciones que asignan a cada punto de su dominio un vector en un espacio vectorial. Por ejemplo, una función vectorial de una variable real puede asignar a cada número real un vector en el espacio tridimensional.

```math

\mathbf{r}(t) = \langle x(t), y(t), z(t) \rangle
``` 

estas admiten representacion en r2 y r3, y se pueden usar para describir curvas en el espacio.

## curvas

una curva es una función vectorial que describe una trayectoria en el espacio. por ejemplo, la curva dada por:

```math
\mathbf{r}(t) = \langle \cos(t), \sin(t), t \rangle
``` 
describe una hélice en el espacio tridimensional.

![alt text](imagenes/helice_en_r3.png)

## paremtrizacion de curvas

la parametrización de una curva es la forma en que se describe la curva mediante una función vectorial. por ejemplo, la curva dada por:

```math
\mathbf{r}(t) = \langle t, t^2, t^
3 \rangle
```

describe una curva en el espacio tridimensional, y la función vectorial que la describe es su parametrización.

## rectas tangentes

parte de la base de que para una parametrizacion de una curva X(t) = (x(t), y(t), z(t)) para t ∈ [a,b], se dice regural si para cada punto de (a,b) existe y es no nulo un vector x'(t) = (x'(t), y'(t), z'(t)). entonces, la recta tangente a la curva en el punto X(t0) es la recta que pasa por el punto X(t0) y tiene como dirección el vector x'(t0). la ecuación de la recta tangente se puede escribir como:

```math
\mathbf{L}(s) = \mathbf{X}(t_0) + s \mathbf{X}'(t_0)
``` 
donde s es un parámetro que varía a lo largo de la recta. esta recta tangente representa la dirección en la que la curva se mueve en el punto X(t0).

## plano tangente

el plano tangente a una superficie en un punto dado es el plano que toca la superficie en ese punto y es perpendicular a la normal de la superficie en ese punto. para encontrar el plano tangente a una superficie dada por una función z = f(x, y) en un punto (x0, y0, z0), se puede usar la siguiente fórmula:

```math
z - z_0 = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)
```     

tambien podemos partir de la base de que una recta tangente a una curva en un punto dado es perpendicular a la normal de la curva en ese punto. entonces, para encontrar el plano tangente a una curva dada por una función vectorial r(t) = (x(t), y(t), z(t)) en un punto t0, se puede usar la siguiente fórmula:

```math
\mathbf{n}(t_0) \cdot (\mathbf{r} - \mathbf{r}(t_0)) = 0
``` 

donde n(t0) es el vector normal a la curva en el punto t0, y r es un punto cualquiera en el plano tangente. esta ecuación representa el plano tangente a la curva en el punto t0.

## conjunto de nivel

un conjunto de nivel de una función f(x, y) es el conjunto de puntos (x, y) en el plano que satisfacen la ecuación f(x, y) = c, donde c es una constante. estos conjuntos de nivel representan las curvas de nivel de la función, que son las curvas que conectan los puntos con el mismo valor de la función. por ejemplo, si f(x, y) = x^2 + y^2, entonces el conjunto de nivel para c = 1 sería el círculo dado por la ecuación x^2 + y^2 = 1.

