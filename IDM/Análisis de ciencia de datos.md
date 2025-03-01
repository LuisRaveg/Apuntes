[[SQL]]

### Experimentos y muestreo
	Tipos de experimentos:
		Observacional: Se colectan aleatoriamente datos ya existentes, de manera             que la colección no intervenga con la generación de datos mismos.
		Controlado: Se asignan tratamientos diferentes de manera aleatoria a                 diferentes grupos.
	Las muestras deben  de cumplir:
		Realism: Representar la realidad de una población 
		Randomization: Las muestras deben incluir aleatoriedad
		Representation:  Ser representativas de la población
	de lo contrario existirá un sesgo.
	Tipos de muestreo:
		Probabilístico:
			Muestreo aleatorio simple: Cada individuo o elemento se elige                       aleatoriamente.
			Muestreo aleatorio estratificado: Subgrupos o estratos, escogiendo                  posteriormente una muestra al azar
			Muestreo sistemático: Primera parte muestra estará entre 1 y k y se                 elige al azar; a partir de esta unidad se van seleccionando                         sistemáticamente uno de los k individuos siguiendo un orden                         determinado. K = Total Población/tamaño muestra
			Muestreo en etapas múltiples: Consiste en empezar a muestrear por algo              que no constituye el objeto de la investigación (unidades primarias),               y obtener una muestra dentro de cada una de ellas (unidades                        secundarias)
		No probabilístico:
			Conveniencia:El investigador decide qué individuos de la población                  forman parte de la muestra en función de la disponibilidad de los                    mismos
			Discrecional: La selección de los individuos de la muestra es                       realizada por un experto que indica al investigador qué individuos de               la población son los que más pueden contribuir al estudio
			Por cuotas: Si se conocen las características de la población a                     estudiar, se elegirán los individuos respetando siempre ciertas cuotas              por edad, género, zona de residencia, entre otras que habrán sido                   prefijadas
### Muestro aleatorio simple
En el muestreo aleatorio simple, la probabilidad de que se escoga un elemento de la muestra es la misma en toda la población. El número de muestras que se pueden seleccionar de una población finita es :
$$ \begin{pmatrix}   N \\ n \end{pmatrix}$$
Si la muestra es insesgada, entonces el valor esperado del parámetro estimado es igual al valor del parámetro de la población.
	Error estandar para la media:$$ \frac{\sigma}{\sqrt{n  }}$$Error estandar para la media en una poblacion finita
$$\sqrt{ 1-\frac{n}{N} } \frac{\sigma}{\sqrt{ n }}$$
	Estimación para la media: $$ \overline{x} \pm z * \frac{\sigma}{\sqrt{n  }}$$
	Estimación para la proporción: $$ p \pm * \sqrt{\frac{p(1-p)}{n}  }$$
### Muestreo por clusters
Usada si tenemos agrupamientos  naturales relativamente homogéneos, por ejemplo edificos con departamentos.
Sea (A) el número total de edificios, (a) el número de edificios seleccionados, entonces:
	Varianza relacionada a la selección de clusters:
	$$ s_{a} ^2 = \frac{1}{a-1}\sum _{i=1}^{a}(\overline{x_{a}}-\overline {x})^2$$
	Error estandar de la media:
	$$ \sqrt{1-\frac{a}{A}  }\frac {s_{a}}{\sqrt{a  }}$$






### Machine Learning
Todos los enfoques de ML, aprenden un mapeo de entradas vs salidas
$$y =f(\overline{x})$$
$$f \rightarrow \{ w_1 ,\dots,w_{m} \}$$
Problem: To compute  $$\overline {w }$$
Supervised Learning:
	1) Classification (Pattern Recognition)
	$$ x \in \mathbb{R}^n , y \in \mathbb{Z}$$
en el caso más sencillo:
$$y\in \{ 0,1\}$$
$$y=\overline{w}^T \overline{x} +b$$
$$y=w_{1 } x_{1}+w_{2}x_{2}+b$$
$$y=\sum _{i=1}^n w_{1}x_{1}+b$$
con n=2:
$$\overline {x} =\begin{pmatrix}
 x_{1}\\ x_{2}
\end{pmatrix}$$
$$\overline {w} =\begin{pmatrix}
 w_{1}\\ w_{2}
\end{pmatrix}$$
	2) Regression Forecasting
		Si tenemos una representación grafíca de las entradas y salidas, podemos crear varios modelos
		Modelo lineal:
			$$y= w_{1}x_{1}+b$$
		Modelo cuadrático:
		$$y=w_{2}x_{1}^2 +w_{1}x_{1}+b$$
		Hasta grado n

Non Supervised Learning
	3) Clustering
		Si tenemos una representación solamente de las entradas x, tendremos que encontrar patrones.
		$$x\in \mathbb{R}^n$$
			k-means:
			Agrupamos en k grupos dependiendo de sus medias.
			
Descenso del gradiente:
La funcion de costo J(w) esta definida como:
$$f_{w}(x_{i})=wx_{i}+b
$$$$J(w)=\frac{1}{2m} \sum  _{i=1}^n (f_{w}(x_{i})-y_{i})^2$$
