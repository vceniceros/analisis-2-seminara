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

