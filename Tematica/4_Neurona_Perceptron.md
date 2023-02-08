# Neurona o Perceptron

## Esquema de una Neurona Artificial

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_Sumatoria.jpg)

El resultado de la suma ponderada es -ya lo sabemos- la suma de cada valor de entrada, xi, por el peso del enlace asociado, wi, más el bias. Llamemos a este resultado "z":

z = w1.x1 + w2.x2 + w3.x3 + w4.x4 + b

Ahora bien, si consideramos el conjunto de valores de entrada a la neurona (xi) un vector:

x = (x1, x2, ..., xn)

...y el conjunto de pesos otro vector:

w = (w1, w2, ..., wn)

...llegamos a la conclusión de que la suma ponderada comentada puede también expresarse como el producto escalar del vector compuesto por los pesos y el vector compuesto por los valores de entrada (más el bias):

z = w•x + b

Tal vez si alguno ya conoce este tipo de situación, dará cuenta que nos encontramos frente a un modelo de regresión lineal.

Por lo cual el bias (b) funciona tal cual como en dicha función antes mencionada, para realizar desplazamientos y dar una mayor flexibilidad al modelo.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_Bias.png)

...lo que nos permite expresar algebraicamente el comportamiento de la neurona, por lo tanto, de la siguiente forma:

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_Umbral.jpg)

Ahora, para explicar a mayor detalle, lo que sucederá que la función que es nuestra neurona, procesará las entradas asignado un valores de peso hasta hallar aquellos que logren satisfacer el comportamiento del umbral antes señalado en la imagen de arriba.

Entonces para visualizar esto, podemos pensar en los valores de logica prosicional como And y Or

Siendo uno el valor de verdadero y cero el valor de falso.

### Lógica Proposicional And

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/logica-And.png)

En este primer caso usará valores de prueba tal que no logrará cumplir con las condiciones de la lógica proposicional.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_And_0.png)

Luego para este segundo caso que veremos vuelve a probar valores que han logrado satisfacer la respuesta, llegando a un buena conclusión.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_And_1.png)

### Lógica Proposicional Or

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/logica-Or.png)

Aquí haremos tal cual el caso anterior hasta encontrar la solución correcta a nuestro caso.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_Or.png)

En este momento vamos a visulaizar estos dos conceptos en su forma de compuerta lógica con ayuda de una gráfica y una recta.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_Compueerta_Logica_Y_O.png)

Donde la línea representa a nuestra neurona con la capacidad de resolver el caso.

### Limitación del Caso XOR

Aqui existe una limitación el cual es el caso XOR

Teniendo en cuenta que usamos una líneal representando a la regresión lineal, una función lineal, se nos presenta el siguiente caso.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_XOR_0.png)

En el cual trataremos de hallar solución para este problema con la regresión lineal.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_XOR_1.png)

Podemos observar de tal manera que no podremos trazar una línea que logré resolver el caso.

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_XOR_1.png)

Entonces uno se ve en la obligación de trazar dos líneas para poder resolver la situación que tenemos enfrente.

Esto que estamos observando como dos rectas en redes neuronales se vería de la siguiente forma:

![image](https://github.com/angelcaceres7450/Fundamentos-de-Redes-Neuronales-con-Python-y-Keras/blob/main/Imagen/Neurona_XOR_1.png)

Aquí ya no se presenta una única neurona, sino es necesaria el uso de dos para poder encontrar la solución al problema, en tal caso, esta limitación de la neurona, es la introducción para una red neuronal, un conjunto de nueronas el cual trabaja para resolver operaciones cada vez más complejas.

