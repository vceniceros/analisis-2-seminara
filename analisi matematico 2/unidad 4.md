# unidad 4

## regla de la cadena

asi como señalamos que resultan diferenciables en sus respectivos dominios las sumas, productos y cocientes de funciones diferenciables, tambien es posible afirmar que la composicion de funciones diferenciables es diferenciable. esta afirmacion se conoce como la regla de la cadena, y se puede expresar de la siguiente manera:

```math
\text{Si } f: \mathbb{R}^n \to \mathbb{R} \text{ es diferenciable en } (x_0, y_0) \text{ y } g: \mathbb{R}^m \to \mathbb{R}^n \text{ es diferenciable en } (u_0, v_0) \text{ tal que } g(u_0, v_0) = (x_0, y_0), \text{ entonces } h = f \circ g: \mathbb{R}^m \to \mathbb{R} \text{ es diferenciable en } (u_0, v_0) \text{ y } \nabla h(u_0, v_0) = \nabla f(x_0, y_0) \cdot J_g(u_0, v_0)
```

donde $J_g(u_0, v_0)$ es la matriz jacobiana de $g$ en el punto $(u_0, v_0)$, y $\nabla f(x_0, y_0)$ es el gradiente de $f$ en el punto $(x_0, y_0)$. esta regla nos permite calcular la derivada de una funcion compuesta a partir de las derivadas de las funciones que la componen.  

tambien es posible expresar la regla de la cadena de manera mas explicita, indicando que si $f$ es una funcion de varias variables y $g$ es una funcion de varias variables, entonces la derivada de la funcion compuesta $h = f \circ g$ se puede calcular utilizando la regla de la cadena de la siguiente manera:

```math
\frac{\partial h}{\partial u} = \frac{\partial f}{\partial x} \cdot \frac{\partial g_1}{\partial u} + \frac{\partial f}{\partial y} \cdot \frac{\partial g_2}{\partial u}
```

por ultimo la regla de la cadena implica que si g es igual f o h entonces el valor de g en un punto es igual al valor de f o h en ese punto, y por lo tanto la derivada de g en ese punto es igual a la derivada de f o h en ese punto. esto se puede expresar de la siguiente manera:

```math
\text{Si } g = f \text{ o } g = h, \text{ entonces } \nabla g(u_0, v_0) = \nabla f(x_0, y_0) \text{ o } \nabla g(u_0, v_0) = \nabla h(u_0, v_0)
```

## funciones definidas implicitamente

en algunos casos, es posible que una funcion de varias variables no se pueda expresar de manera explicita por ejemplo
```math
e^{xz} - y²x² = 0
```

en este caso, la funcion no se puede expresar de manera explicita como una funcion de x, y o z, pero es posible expresar la funcion de manera implicita utilizando la ecuacion dada, tomando esta funcion de 3 variables como si fuera una funcion de 2 variables, por ejemplo tomando z como una funcion de x e y, es decir, z = f(x, y). entonces la ecuacion dada se puede reescribir de la siguiente manera:

```math
e^{xf(x, y)} - y²x² = 0
```

## teorema de la funcion implicita (cauchy-dinni)

el teorema de la funcion implicita, tambien conocido como el teorema de cauchy-dinni, establece que si una funcion de varias variables es diferenciables cumple que para un punto (x0, y0, z0)

- F es una funcion c¹ en un entorno de (x0, y0, z0)
- F(x0, y0, z0) = 0
- la derivada parcial de F con respecto a z en el punto (x0, y0, z0) es diferente de 0

entonces existe un entorno de (x0, y0) en el que se puede definir una funcion f de x e y tal que f(x0, y0) = z0 y F(x, y, f(x, y)) = 0 para todo (x, y) en ese entorno. ademas, la funcion f es diferenciable en ese entorno y su derivada se puede calcular utilizando la regla de la cadena de la siguiente manera:

```math
\frac{\partial f}{\partial x} = -\frac{\frac{\partial F}{\partial x}}{\frac{\partial F}{\partial z}} \quad \text{y} \quad \frac{\partial f}{\partial y} = -\frac{\frac{\partial F}{\partial y}}{\frac{\partial F}{\partial z}}
```