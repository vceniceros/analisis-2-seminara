# unidad 7

## integrales curvilineas

asi como ya tenemos definido el concepto de curva y las distintas maneras de representarlas, tambien sabemos como evaluar su continuidad y que para cada punto existe un vector tangente a la curva. ahora vamos a aprender medir el largo de una curva, y para eso vamos a utilizar el concepto de integral curvilinea. 

### longitud de una curva

la longitud de una curva se puede calcular utilizando la integral curvilinea de la norma del vector tangente a la curva. es decir, si tenemos una curva parametrizada por una funcion vectorial r(t) = (x(t), y(t), z(t)), entonces la longitud de la curva se puede calcular utilizando la siguiente formula:

```math
L = \int_a^b \|r'(t)\| dt
```

- sabemos que el vector tangente a la curva en un punto t es r'(t) = (x'(t), y'(t), z'(t)), puede pensarse copmo la velocidad con que se mueve una particula sobre la curva a medida que t (podria representar el tiempo) recorre el intervalo [a, b]. 

- en un lapso infinitesimal de tiempo dt, la particula se mueve una distancia infinitesimal, ds = r'(t) dt, cuya longitud es ds = \|r'(t)\| dt. 

- so queremos evaluar la longitud de la trayectoria que recorrio la particula en el intervalo de tiempo [a, b], debemos sumar todas las distancias infinitesimales que recorrió la particula en cada instante de tiempo, lo cual se puede expresar utilizando la integral curvilinea de la norma del vector tangente a la curva, es decir, 
```math 
L = \int_a^b \|r'(t)\| dt.
```

### invariancia de la integral curvilinea respecto a la parametrizacion

tanto la longitud como la masa como las cordenadads del centro de masa y otras magnitudes escalares de la fisica responden a integrales de la siguiente forma:

```math
\int_a^b f(r(t)) \|r'(t)\| dt
```
### teorema 

el valor de la integral curvilinea de una funcion f a lo largo de una curva parametrizada no depende de la parametrizacion de la curva, salvo eventualmente en su signo si la parametrizacion es tal que recorre la curva en sentido contrario. es decir, si tenemos una curva parametrizada por una funcion vectorial r(t) = (x(t), y(t), z(t)), y otra parametrizacion de la misma curva dada por una funcion vectorial s(u) = (x(u), y(u), z(u)), entonces se cumple que:

```math
\int_a^b f(r(t)) \|r'(t)\| dt = \int_c^d f(s(u)) \|s'(u)\| du
``` 

## campos conservativos

un campo vectorial F es conservativo si existe una funcion escalar f tal que F es igual al gradiente de f, es decir, F = \nabla f. en este caso, la funcion f se llama potencial del campo vectorial F.
