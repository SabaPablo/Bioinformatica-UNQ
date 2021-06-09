# LA VIDA EN TRES DIMENSIONES

## TRABAJO PRACTICO 2



#### - ¿En qué células encontramos hemoglobina?
La hemoglobina la podemos encontrar en las celulas de la sangre.
#### - ¿Para qué es utilizado este oxígeno a nivel celular?
Las celulas utilizan el oxígeno para oxidar determinados compuestos organicos y asi obtener energia aprovechable para la célula.
#### - ¿Cómo crees que es transportada esta molécula de O<sub>2</sub> por la hemoglobina?
La molecula de O<sub>2</sub> es transportada por la hemoglobina en una pequeña endija donde cae dicha molecula y es atrapada y llevada hasta una celula.
[Protein Data Bank o PDB](https://www.rcsb.org/)
## Protein Data Bank  (https://www.rcsb.org/)

#### - ¿Qué información nos provee esta página?
En esta pagina provee el acceso a las bases de datos donde se encuentran todas las estructuras de macromoléculas biológicas obtenidas hasta el momento.
#### - ¿Cómo se determinó la estructura de esta proteína?
La estructura de la proteina se determina a travez de un metodo llamado cristalizacion a la que se somete dicha proteina, donde luego se la bombardea con rayos la cual algunas rebotan para darnos la forma tridimensional de la misma
#### - A la izquierda vemos una representación de la estructura de ubiquitina. ¿Qué significan las cintas, las flechas y las regiones angostas?

las estructuras hélice α se representan con cintas, las hebras β se representan con flechas amplias y los loops son representados con regiones angostas.

#### - ¿Representa esa imagen a la realidad del sistema biológico?

Representan la forma en un momento preciso de una proteina

#### - La estructura 2W6V fue “refinada a una resolución de 1.8 Angstroms”.
#### Éste es el error asociado al experimento: mientras mayor es la resolución, menor es la certeza al determinar la posición de cada átomo.

Para lograr su imagen y posición se la somete a lo que se denomina cristalización lo que hace reducir su movimiento para luego bombardearla con rayos. Lo que nos da a entender que solo modela un momento exacto de la proteína y no en su condición real.

#### ¿Cuál es la utilidad y los condicionamientos de usar un modelo científico que sabemos inexacto?

Si bien sabemos es inexacto, podemos determinar algunas de las formas que adquiere y toma esa proteina, la cual nos permite en forma computacional saber que tan probable es que una droga haga efecto sobre ella o pueda ser quien la transporta.

#### Exploremos la pestaña de visualización tridimensional (3D View). Con el mouse podemos rotar, acercar y desplazar a la molécula. El menú de la derecha nos permite cambiar el modo de representación.
#### ¿Qué diferencias y similitudes notamos respecto de la representación inicial?
####En el menú de la derecha hay opciones de distintos tipos de representación y
formas de colorear la estructura tridimensional. ¿Para qué podría ser útil
visualizar lo mismo de distintas maneras?

Una nos da un aspecto fisico que toma la proteina y el otro muestra mas en detalle porque va tomando una forma o otra.

#### ¿Qué información esperaría encontrar como resultado un experimento destinado a determinar la estructura terciaria de una molécula biológica?

Esperaria encontrar la posicion en el espacion de los componentes de dicha molecula.

#### Podemos explorar el contenido del archivo que acabamos de descargar si lo observamos con un editor de texto. Haciendo clic con el botón derecho del mouse sobre el archivo descargado, usemos la opción Abrir con y seleccionemos el Bloc de Notas u otro editor de texto. ¿En qué consiste un archivo PDB?

Un archivo pdb revela informacion relacionada a la proteina a estudiar. Tiene, nombre de proteina, de que organismo se tomo la muestra, informacion del paper por el cual se hizo el estudio, datos del o les autores. Como esta conformada la estructura primaria. Y datos de la posicion de cada uno de los atomos que conforman a la proteina.

#### Desplacémonos por el archivo hasta encontrar las líneas que comienzan con la palabra ATOM. ¿Qué tipo de información brinda esta sección?

```
ATOM      1  N    VAL	 A    1      18.512  29.178  42.972  1.00 33.06           N  
ATOM      2  CA  AVAL  A     1      19.432  30.114  42.266  0.50 32.94           C  
ATOM      3  CA  BVAL  A    1      19.422  30.061  42.195  0.50 32.89           C  
ATOM      4  C    VAL    A     1      20.844  29.541  42.277  1.00 32.59           C  
ATOM      5  O    VAL    A     1      21.187  28.799  43.185  1.00 33.23           O  
ATOM      6  CB  AVAL  A     1      19.446  31.510  42.960  0.50 33.24           C  
ATOM      7  CB  BVAL  A     1      19.374  31.551  42.672  0.50 33.23           C 
```
Las lineas que empiezan con la palabra ATOM nos indican los atomos que conforman esa proteina, las numera, dice que elemento son, a que aminoacido corresponde, luego da las coordenas en el espacio ('x', 'y', 'z').
Los últimos tres campos que se muestran son la ocupación, el factor de temperatura (B-factor) y el símbolo del elemento.

#### ¿Podríamos extraer de este archivo información sobre la estructura primaria de la proteína en cuestión? ¿Cómo se presenta dicha información y qué significa la representación? Desde el punto de vista computacional:¿de qué tipo de dato se trata esta información?

Si, la estructura primaria esta representada con la palabra inicial SEQRES

Por ejemplo para 1UBQ:
```
SEQRES   1 A   76  MET GLN ILE PHE VAL LYS THR LEU THR GLY LYS THR ILE          
SEQRES   2 A   76  THR LEU GLU VAL GLU PRO SER ASP THR ILE GLU ASN VAL          
SEQRES   3 A   76  LYS ALA LYS ILE GLN ASP LYS GLU GLY ILE PRO PRO ASP          
SEQRES   4 A   76  GLN GLN ARG LEU ILE PHE ALA GLY LYS GLN LEU GLU ASP          
SEQRES   5 A   76  GLY ARG THR LEU SER ASP TYR ASN ILE GLN LYS GLU SER          
SEQRES   6 A   76  THR LEU HIS LEU VAL LEU ARG LEU ARG GLY GLY  
```

### En el sitio web www.uniprot.org usá el código LPXA_ECOLI para:
#### 1. Identificá el tipo de proteína
Es una enzima, una acil-transferasa. La  Acil- [proteína transportadora de acilo] - UDP-N-acetilglucosamina O-aciltransferasa

#### 2. ¿Qué tipo de proteína es? ¿Es una enzima? ¿Cuál es su actividad?
Es una enzima. Su actividad esta relacionada con la biosíntesis de el "lipido A"
#### 3. Identificá a que organismo pertenece la proteína
La proteina pertenece a una bacteria llamada ***Escherichia coli***
#### 4. Analizá los “GO terms”, caracterizá el proceso biológico en el que se encuentra involucrada esta proteína y el lugar donde la LPXA_ECOLI lleva a cabo su rol biológico.
Esta localizada en el citoplasma. Esta proteina esta involucrada en paso 1 de la sub-ruta de sintesis del lipido A.
### Usando la sección de “Cross References”:
#### 5. Obtené la región codificante
[Codigo FASTA región codificante](www.gasdf)
#### 6. ¿Está cristalizada la proteína? ¿Qué código PDB tiene?
Si, esta cristalizada y el codigo PD es [1LXA](https://www.rcsb.org/structure/1LXA)
