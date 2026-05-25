# ecuaciones diferenciales ordinarias

la matemiatica es el lenguaje de la ciencia, los cientificos mediantes la experimentacion buscar llegar a representar mediante expresiones matematicas los fenomenos que observan en la naturaleza, y de esta manera poder predecir su comportamiento, un modelo matematico con cierto grado de aproximacion permite por ejemplo poder predecir comportamientos futuos, a su vez un ingeniero puede utilizar un modelo matematico para diseñar un sistema que cumpla con ciertos requisitos, por ejemplo, un ingeniero puede utilizar un modelo matematico para diseñar un puente que pueda soportar una cierta carga.

## definicion

una ecuacion diferencial ordinaria es una ecuacion que relaciona una funcion desconocida con sus derivadas, es decir, es una ecuacion que contiene una funcion desconocida y sus derivadas, y que se utiliza para describir el comportamiento de un sistema dinamico. las ecuaciones diferenciales ordinarias se utilizan en muchas areas de la ciencia y la ingenieria, por ejemplo, en la fisica para describir el movimiento de los cuerpos, en la biologia para describir el crecimiento de las poblaciones, en la economia para describir el comportamiento de los mercados, entre otras.


### definicion formal

se llama ecuacion diferencial ordinaria (EDO) a toda ecuacion que involucre una funcion incognita **de una variable independiente** y sus derivadas incluyendo eventualmente tambien a la variable independiente. es decir, una ecuacion diferencial ordinaria es una ecuacion que relaciona una funcion desconocida con sus derivadas. 
```math

F(x, y, y', y'', \ldots, y^{(n)}) = 0
```

## orden de una ecuacion diferencial ordinaria

se llama orden de la ecuacion diferencial ordinaria al mayor orden de derivacion con que aparezca la funcion incognita y(x) en la ecuacion diferencial: 

```math
F(x, y(x), y'(x), y''(x), \ldots, y^{(n)}(x)) = 0
```

## solucion de una ecuacion diferencial ordinaria

se llama solucion de una ecuacion diferencial ordinaria a toda funcion que al ser sustituida en la ecuacion diferencial satisface la igualdad. es decir, una solucion de una ecuacion diferencial ordinaria es una funcion que al ser sustituida en la ecuacion diferencial satisface la igualdad. por ejemplo, si tenemos la ecuacion diferencial ordinaria:

```math
y' = y
```

## metodos de resolucion de EDOS de primer orden

existen varios metodos para resolver ecuaciones diferenciales ordinarias de primer orden, algunos de los metodos mas comunes son:

1. metodo de separacion de variables: este metodo se utiliza cuando la ecuacion diferencial ordinaria se puede escribir en la forma:

```math
\frac{dy}{dx} = g(x)h(y)
```

ejemplo, tomando la funcion u'+ 3u = 0, podemos escribirla como u' = -3u, y luego separando las variables obtenemos:

```math
\frac{du}{u} = -3 dx
```

2. ecuaciones lineales, para eso expliquemos el conecpto de ecuacion diferencial ordinaria lineal, una ecuacion diferencial ordinaria de primer orden es lineal si se puede escribir en la forma:

```math
p(x)* y'  + q(x)* y = f(x)
``` 
con p(x), q(x) y f(x) funciones continuas en un intervalo I

se llama tambien ecuacion homogenea asociada a la que es de forma p(x)* y'  + q(x)* y = 0, es decir, la ecuacion homogenea asociada a una ecuacion diferencial ordinaria lineal es la ecuacion diferencial ordinaria lineal que se obtiene al igualar a cero el termino independiente f(x). para resolver una ecuacion diferencial ordinaria lineal de primer orden, debemos seguir los siguientes pasos:

1. resolver la ecuacion homogenea asociada, es decir, resolver la ecuacion diferencial ordinaria lineal que se obtiene al igualar a cero el termino independiente f(x).
2. encontrar una solucion particular de la ecuacion diferencial ordinaria lineal, es decir, encontrar una funcion que al ser sustituida en la ecuacion diferencial ordinaria lineal satisfaga la igualdad.
3. la solucion general de la ecuacion diferencial ordinaria lineal es la suma de la solucion general de la ecuacion homogenea asociada y una solucion particular de la ecuacion diferencial ordinaria lineal.

3. ecuaciones diferenciales de tipo homogeneo, una ecuacion diferencial ordinaria de primer orden es homogenea si se puede escribir en la forma:

```math
\frac{dy}{dx} = f\left(\frac{y}{x}\right)
```

## aplicacion de EDOs a familias de curvas

una familia de curvas es un conjunto de curvas que se pueden describir mediante una ecuacion diferencial ordinaria. por ejemplo, la familia de curvas que se pueden describir mediante la ecuacion diferencial ordinaria:

```math
\frac{dy}{dx} = \frac{y}{x}
```

dos familias de curvas son ortogonales si las tangentes a las curvas de una familia son perpendiculares a las tangentes a las curvas de la otra familia. para encontrar la ecuacion diferencial ordinaria que describe la familia de curvas ortogonales a una familia de curvas dada, debemos seguir los siguientes pasos:

1. encontrar la ecuacion diferencial ordinaria que describe la familia de curvas dada, es decir, encontrar la ecuacion diferencial ordinaria que se obtiene al derivar la ecuacion de la curva con respecto a x.
2. encontrar la ecuacion diferencial ordinaria que describe la familia de curvas ortogonales, es decir, encontrar la ecuacion diferencial ordinaria que se obtiene al derivar la ecuacion de la curva con respecto a x y luego multiplicar por -1.

3. resolver la ecuacion diferencial ordinaria que describe la familia de curvas ortogonales, es decir, encontrar la solucion general de la ecuacion diferencial ordinaria que se obtiene al derivar la ecuacion de la curva con respecto a x y luego multiplicar por -1.

## lineas de campo

las lineas de campo son curvas que representan la direccion del campo vectorial en cada punto del espacio. para encontrar las lineas de campo de un campo vectorial, debemos seguir los siguientes pasos:

1. encontrar la ecuacion diferencial ordinaria que describe las lineas de campo, es decir, encontrar la ecuacion diferencial ordinaria que se obtiene al derivar la ecuacion de la curva con respecto a x y luego multiplicar por -1.

2. resolver la ecuacion diferencial ordinaria que describe las lineas de campo, es decir, encontrar la solucion general de la ecuacion diferencial ordinaria que se obtiene al derivar la ecuacion de la curva con respecto a x y luego multiplicar por -1.

