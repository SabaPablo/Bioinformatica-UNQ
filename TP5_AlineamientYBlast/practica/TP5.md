# ALINEAMIENTO Y BLAST

## [TRABAJO PRACTICO 5](https://flbulgarelli.github.io/umi/#una-palabra-no-dice-nada-y-al-mismo-tiempo-lo-dice-todo)

#### 👉 PARA PENSAR: ¿Qué tipo de información se puede extraer de la comparación de secuencias? ¿Cómo esperás que se vea en una comparación? 

Al comparar secuencias podemos identificar a quien corresponde o que tan similar es con otras. 


#### 👉 PARA PENSAR: ¿Por qué crees que es mejor evaluar las relaciones evolutivas lejanas comparando proteínas?

Porque las proteinas conservan mejor la mejor la informacion filogenetica a lo largo del tiempo.

#### 👇 RETO I: Intentemos, entonces alinear estas dos palabras, para comprender mejor el problema. Alineá en la tabla interactiva las palabras "BANANA" y "MANZANA".
###### ¡Tomá nota de tus observaciones y de las conclusiones que se desprendan de estas observaciones!
#### ☑ ️ PREGUNTAS DISPARADORAS: ¿Existe una única forma de alinearlas? ¿Es alguno de los posibles alineamientos mejor que otro? Si así fuera ¿Por qué?
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R1-2.png)
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R1-1.png)
Pueden existir varios formas de alinear y dependiendo de cuanto se tenga que modificar para alineralos y cuantos errores podemos encontrar.

#### 👇 RETO II: En la siguiente tabla interactiva  distintos alineamientos para las palabras "ANA" y "ANANA". Verás que en el margen superior derecho aparece un valor de identidad calculado para cada alineamiento que intentes.
###### ¡Tomá nota de los valores de identidad observados y de las conclusiones que se desprendan de estas observaciones!
#### ☑ ️ PREGUNTAS DISPARADORAS: ¿Son todos los valores iguales? ¿Qué consideraciones deberían tenerse en cuenta a la hora de realizar el cálculo? ¿Se te ocurre, distintas formas de calcularlo? ¿Serán todas ellas igualmente válidas en Biología?
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R2-1.png)
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R2-2.png)
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R2-3.png)
![Tabla](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R2-4.png)

En esta prueba no importa donde agregue el gap, la identidad es la misma si no tiene errores. Sin embargo creo que la penalidad no es la misma para dos gap en el inicio o 2 gaps en el final o los gaps entre medio de las letras. La forma de saber si una variante es posible es por medio de evidencia que podemos encontrar en distintos organismos.

#### 👇 RETO III: Probá en  tabla interactiva distintos alineamientos para las palabras "ANA" y "ANANA". Verás que en el margen superior derecho aparece un valor de identidad calculado para cada alineamiento que intentes y un botón para cambiar la penalidad que se le otorga a dicho para el cálculo de identidad.
###### Probá varias combinaciones, tomá nota de los valores de identidad observados y de las conclusiones que se desprendan de estas observaciones.
#### ☑ ️ PREGUNTAS DISPARADORAS: ¿Cómo se relacionan los valores de identidad obtenidos con las penalizaciones que se imponen al gap? ¿Qué implicancias crees que tiene una mayor penalización de gaps? ¿Se te ocurre alguna otra forma de penalización que no haya sido tenido en cuenta en este ejemplo?

![Original](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R3-1.png)

![Cambio en penalidad](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R3-2.png)
![ConErrores](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R3-3.png)
![ConErrores](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R3-4.png)
![ConErrores y gaps](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/R3-5.png)

Dependiendo la penalidad de los gaps puedo ver que un error es menos costos. Sacando del medio los errores, puedo pensar que dependiendo el coste de los gaps la identidad entre dos secuencias puede ser mayor o peor. Una forma que vimos de penalizar es ver caso por caso y buscar evidencia en la naturaleza, donde la penalidad se calcule con que tan probable sea que exista ese gap en la naturaleza.

#### 👉 PARA PENSAR: Entonces, pensando en un alineamiento de ácidos nucleicos ¿Cuáles te parece que son las implicancias de abrir un gap en el alineamiento? ¿Qué implicaría la inserción o deleción de una región de más de un residuo?
Un gap implica un costo que implica la identidad o no entre dos secuencias, pero a su vez pueden ayudar a dichas secuencias a continuacion del gap sen mas identicas. 

#### 👇 RETO IV: Probá en la tabla interactiva distintos alineamientos para las secuencias nucleotídicas. Podrás ver las traducciones para cada secuencia.
Probá varias combinaciones, tomá nota de las observaciones y de las conclusiones que se desprendan de estas.
 
👉 PARA PENSAR: ¿Dá lo mismo si el gap que introducís cae en la primera, segunda o tercer posición del codón? ¿Cómo ponderarías las observaciones de este ejercicio para evaluar el parecido entre dos secuencias?


👇 RETO V: Estuvimos viendo que el alineamiento de secuencias no es trivial y requiere contemplar los múltiples caminos posibles, teniendo en cuenta al mismo tiempo la información biológica que restringe ese universo de posibilidades. 
 
¡Es momento de llevar entonces estos conceptos a lo concreto! 
 
Te proponemos pensar los pasos a seguir en un alineamiento de dos secuencias cortas, teniendo en cuenta una matriz genérica de scoring (puntuación) que contemple las complejidades que estuvimos viendo, es decir que penalice de distinto modo una inserción o deleción, una discordancia (mismatch) o una coincidencia (match). Escribilos o esquematizalos en un diagrama de flujo.
 
👉 PARA PENSAR: ¿En qué consiste la programación dinámica? ¿Por qué crees que es útil en este caso? 


👇 RETO VI: Utilizando la herramienta interactiva  desarrollada por el Grupo de Bioinformática de Freiburg probá distintos Gap penalties para el ejemplo propuesto y observá lo que ocurre.
 
Interpretando la recursión, explicá con tus palabras de dónde salen los valores de la matriz  que se construye. ¡Esquematiza tus conclusiones!

👉 PARA PENSAR: ¿En qué casos serán de utilidad uno u otro tipo de alineamientos? ¿Qué limitaciones tendrá cada uno?

👉 PARA PENSAR: Ingresá al servidor del NCBI y mirá los distintos programas derivados del BLAST que se ofrecen ¿Para qué sirve cada uno? ¿En qué casos usarías cada uno?   

👇 RETO VII: calculá el E-value y porcentaje de identidad utilizando el programa BLAST de la siguiente secuencia input usando 5000 hits, un e-value de 100 y tomando aquellos hits con un mínimo de 70% cobertura. Observe y discuta el comportamiento de : E-value vs. % id, Score vs % id,  Score vs E-value

VVGGLGGYMLGSAMSRPIIHFGSDYEDRYYRENMHRYPNQVYYRPMDEYSNQNNFVHDCVNITIKQHTVTTTTKGENFTETDVKMMERVVEQMCITQYERESQAYYQRGSSMVLFSSPPVILLISFLIFLIVG

👇 RETO VIII: Realizá nuevas búsquedas usando la mitad de la secuencia problema y para un cuarto de la secuencia original. Compará los gráficos obtenidos. ¿Qué conclusiones puede sacas?


👇 RETO IX: Utilizando BLAST utilice búsquedas de similitud secuencial para identificar a la siguiente proteína:

MIDKSAFVHPTAIVEEGASIGANAHIGPFCIVGPHVEIGEGTVLKSHVVVNGHTKIGRDNEIYQFASIGEVNQDLKYAGEPTRVEIGDRNRIRESVTIHRGTVQGGGLTKVGSDNLLMINAHIAHDCTVGNRCILANNATLAGHVSVDDFAIIGGMTAVHQFCIIGAHVMVGGCSGVAQDVPPYVIAQGNHATPFGVNIEGLKRRGFSREAITAIRNAYKLIYRSGKTLDEVKPEIAELAETYPEVKAFTDFFARSTRGLIR



👉 PARA PENSAR: ¿Cuál es la función de la proteína? ¿A qué grupo taxonómico pertenece? A un nivel de significancia estadística adecuado ¿cuántas secuencias similares se encuentran? 

👇 RETO X:  Realizá una nueva corrida del BLASTp, utilizando la misma secuencia , pero ahora contra la base de datos PDB.  ¿Se obtienen los mismo resultados? ¿Qué tipo de resultados(hits) se recuperan? ¿Cuándo nos podría ser útil este modo de corrida?

