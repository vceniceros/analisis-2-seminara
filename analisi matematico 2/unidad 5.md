# unidad 5

## polinomios de taylor

supongamos que tenemos una funcion de varias variables f: R^n -> R, y queremos aproximar el valor de la funcion en un punto cercano a un punto dado (x0, y0, z0). para hacer esto, podemos utilizar el polinomio de taylor de la funcion en el punto (x0, y0, z0), que se puede expresar de la siguiente manera:

```math
P_k(x, y, z) = f(x_0, y_0, z_0) + \nabla f(x_0, y_0, z_0) \cdot \begin{pmatrix} x - x_0 \\ y - y_0 \\ z - z_0 \end{pmatrix} + \frac{1}{2} \begin{pmatrix} x - x_0 \\ y - y_0 \\ z - z_0 \end{pmatrix}^T H_f(x_0, y_0, z_0) \begin{pmatrix} x - x_0 \\ y - y_0 \\ z - z_0 \end{pmatrix} + \ldots + \frac{1}{k!} D^k f(x_0, y_0, z_0) \cdot \begin{pmatrix} x - x_0 \\ y - y_0 \\ z - z_0 \end{pmatrix}^k
```

esto nos puede servir para aproximar el valor de la funcion en un punto cercano a (x0, y0, z0) utilizando los valores de la funcion y sus derivadas en el punto (x0, y0, z0). ademas, el polinomio de taylor nos permite analizar el comportamiento de la funcion cerca del punto (x0, y0, z0), por ejemplo, podemos determinar si el punto es un maximo, un minimo o un punto de silla utilizando el polinomio de taylor de segundo orden.

tambien es posible expresar el polinomio de taylor de una funcion de varias variables utilizando la notacion de sumas, de la siguiente manera:

```math
P_k(x, y, z) = \sum_{|\alpha| \leq k} \frac{D^\alpha f(x_0, y_0, z_0)}{\alpha!} \cdot (x - x_0)^{\alpha_1} \cdot (y - y_0)^{\alpha_2} \cdot (z - z_0)^{\alpha_3}
```     

el polinomio de taylor nos rive para aproximar valores de la funcion en puntos cercanos a (x0, y0, z0), pero tambien nos permite analizar el comportamiento de la funcion cerca de ese punto, por ejemplo, podemos determinar si el punto es un maximo, un minimo o un punto de silla utilizando el polinomio de taylor de segundo orden. para esto, debemos calcular el hessiano de la funcion en el punto (x0, y0, z0) y analizar su signo. si el hessiano es positivo definido, entonces el punto es un minimo local; si el hessiano es negativo definido, entonces el punto es un maximo local; y si el hessiano es indefinido, entonces el punto es un punto de silla. 

## extremos en campos escalares 

un extremo local de una funcion de varias variables es un punto donde la funcion alcanza un valor maximo o minimo en un entorno cercano. para determinar si un punto es un extremo local, podemos utilizar el polinomio de taylor de segundo orden de la funcion en ese punto.

si el hessiano de la funcion en el punto es positivo definido, entonces el punto es un minimo local; si el hessiano es negativo definido, entonces el punto es un maximo local; y si el hessiano es indefinido, entonces el punto es un punto de silla.

para encontrar los extremos locales de una funcion de varias variables, debemos seguir los siguientes pasos:

1. calcular las derivadas parciales de la funcion y encontrar los puntos criticos, es decir, los puntos donde las derivadas parciales son iguales a cero.

2. calcular el hessiano de la funcion en cada punto critico y analizar su signo para determinar si el punto es un maximo local, un minimo local o un punto de silla.

es importante tener en cuenta que un punto critico puede no ser un extremo local, por lo que es necesario analizar el hessiano para determinar la naturaleza del punto critico. ademas, es posible que una funcion no tenga extremos locales, o que tenga varios extremos locales, dependiendo de su comportamiento.

## hessiano

el hessiano de una funcion de varias variables es una matriz cuadrada que contiene las segundas derivadas parciales de la funcion. el hessiano se utiliza para analizar el comportamiento de la funcion cerca de un punto critico, y para determinar si el punto critico es un maximo local, un minimo local o un punto de silla.

para calcular el hessiano de una funcion de varias variables, debemos seguir los siguientes pasos:

1. calcular las derivadas parciales de la funcion con respecto a cada variable.

2. calcular las segundas derivadas parciales de la funcion con respecto a cada par de variables.

3. organizar las segundas derivadas parciales en una matriz cuadrada, donde la entrada (i, j) corresponde a la segunda derivada parcial de la funcion con respecto a las variables i y j.

## teorema de schwarz

el teorema de schwarz establece que si una funcion de varias variables tiene segundas derivadas parciales continuas, entonces las segundas derivadas parciales son iguales, es decir, la segunda derivada parcial de la funcion con respecto a las variables i y j es igual a la segunda derivada parcial de la funcion con respecto a las variables j y i.

casos:

si el determinante de la matriz hessiana es mayor que cero y la segunda derivada parcial con respecto a la primera variable es mayor que cero, entonces el punto critico es un minimo local.

si el determinante de la matriz hessiana es mayor que cero y la segunda derivada parcial con respecto a la primera variable es menor que cero, entonces el punto critico es un maximo local.

si el determinante de la matriz hessiana es menor que cero, entonces el punto critico es un punto de silla.

