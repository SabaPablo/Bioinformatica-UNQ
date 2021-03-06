# ¿EN QU'E SE PARECEN UNA GALLINA Y UNA MOSCA?

## TRABAJO PRACTICO 4


| Secuencia        | Nombre taxonómico        | Nombre común         | 
| :---------------:|:------------------------:|:--------------------:|
| NP_061820.1      | Homo sapiens             | Humano               |
| NP_001072946.1   | Gallus gallus            | Gallo asiático       |
| NP_001065289.1   | Pan troglodytes          | Chimpancé            |
| NP_001157486.1   | Equus caballus           | Caballo              |
| NP_001183974.1   | Canis lupus familiaris   | Perro                |
| AEP27192.1 	   | Gorilla gorilla          | Gorila occidental    |
| XP_024245566.1   | Oncorhynchus tshawytscha | Salmón real          |
| NP_001086101.1   | Xenopus laevis           | Rana de uñas africana|
| NP_477164.1      | Drosophila melanogaster  | Moscas de la fruta   |


```fasta
>NP_061820.1 cytochrome c [Homo sapiens]
MGDVEKGKKIFIMKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGYSYTAANKNKGIIWGEDTLMEYLE
NPKKYIPGTKMIFVGIKKKEERADLIAYLKKATNE
>NP_001072946.1 cytochrome c [Gallus gallus]
MGDIEKGKKIFVQKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAEGFSYTDANKNKGITWGEDTLMEYLE
NPKKYIPGTKMIFAGIKKKSERVDLIAYLKDATSK
>NP_001065289.1 cytochrome c [Pan troglodytes]
MGDVEKGKKIFIMKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGYSYTAANKNKGIIWGEDTLMEYLE
NPKKYIPGTKMIFVGIKKKEERADLIAYLKKATNE
>NP_001157486.1 cytochrome c [Equus caballus]
MGDVEKGKKIFVQKCAQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGFSYTDANKNKGITWKEETLMEYLE
NPKKYIPGTKMIFAGIKKKTEREDLIAYLKKATNE
>NP_001183974.1 cytochrome c [Canis lupus familiaris]
MGDVEKGKKIFVQKCAQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGFSYTDANKNKGITWGEETLMEYLE
NPKKYIPGTKMIFAGIKKTGERADLIAYLKKATKE
>AEP27192.1 cytochrome c [Gorilla gorilla]
MGDVEKGKKIFIMKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGYSYTAANKNKGIIWGEDTLMEYLE
NPKKYIPGTKMIFVGIKKKEERADLIAYLKKATNE
>XP_024245566.1 cytochrome c [Oncorhynchus tshawytscha]
MGDIEKGKKAFVQKCAQCHTVENGGKHKVGPNLWGLFGRKTGQAEGFSYTDANKAKGIVWDTDTLMTYLE
NPKKYIPGTKMIFAGIKKKGERADLIAYLKSATS
>NP_001086101.1 cytochrome c, testis-specific [Xenopus laevis]
MGDVEKGKKVFVQKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAEGFSYTDANKNKGIVWDEDTLMVYLE
NPKKYIPGTKMIFAGIKKKGERQDLIAYLKQSTSS
>NP_477164.1 cytochrome c distal, isoform A [Drosophila melanogaster]
MGSGDAENGKKIFVQKCAQCHTYEVGGKHKVGPNLGGVVGRKCGTAAGYKYTDANIKKGVTWTEGNLDEY
LKDPKKYIPGTKMVFAGLKKAEERADLIAFLKSNK

```

##### 1. ¿Cuán sencillo será alinear dos o más secuencias a mano? ¿Cuánto influirán el número de secuencias a alinear, su longitud, y la similitud entre ellas?

  En realidad no es tan sensillo de ver el alineamiento, se pueden ver que hay alguna similitud entre ellas. 

##### 2. ¿Son parecidos los citocromos c de humano y gallo? 

  A simple vista cuesta ver que tan parecidos son los citocromos c del humano y del gallo, con Clustal Omega es mucho mas facil visualizar sus similitudes y diferencias, donde muestra de 105 aminoacidos 13 diferencias entre ellos. Si bien no tengo un criterio para saber si con 13 dismatch es muy o poco, considero que es bastante similar.

##### 3. ¿Qué teorías subyacen a este análisis? ¿Cómo nos ayuda la evolución a explicar sus similitudes y diferencias?

  Las teorias que se hacen mas solidas al ver estos análisis es que existe una similitud entre ambas especies, se podria creer que tienen un ancestro en comun. 

  Con estos analisis podriamos entender mejor un poco la historia de la vida. Podemos ver que a nivel molecular tenemos mas parentescos con una especie que con otra.

![cotocromoC Homo - galius](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP4_EnQueSePareceUnaVacaYUnaGallina/practica/extra/homo_gallo_secuence_alignment.png)

##### 4. Podemos elegir verlo en colores (Show Color). ¿Qué indican los colores? ¿Qué indican el guión (-), los dos puntos (:) y el asterisco (*)?

  Segun la documentación podemos encontrar: 

|Residue  |	Colour |	Property |
|:-------:|:-------:|:-------:|
|AVFPMILW | RED |	Small (small+ hydrophobic (incl.aromatic -Y))|
|DE	      | BLUE |	Acidic |
|RK |	MAGENTA |	Basic - H |
|STYHCNGQ	| GREEN |	Hydroxyl + sulfhydryl + amine + G |
|Others |	Grey |	Unusual amino/imino acids etc |

  Los colores agrupan a los aminoacidos segun sus propiedades quimicas

  (-) Indica un gap en esa posición.

  (:) Indica la conservación entre grupos de propiedasdes muy similares.

  (*) Indica posiciones que tienen un solo residuo completamente conservado.

  (.) Indica conservación entre grupos de propiedades débilmente similares.

##### 5. A simple vista, ¿se conserva la secuencia del citocromo c en los organismos?

![multiple secuence alignment](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP4_EnQueSePareceUnaVacaYUnaGallina/practica/extra/multple_secuence_alignment_color.png)


  A simple vista se puede ver que si. Si bien se ven en algunos casos mas diferencias que en otros, podemos observar que se conserva en gran parte la secuenca del citocormo c.
  
##### 6. ¿Creeríamos que todos los organismos se asemejan por igual al resto, o se pueden identificar grupos de mayor similitud? Si es así, ¿tienen sentido?

  Se puede llegar a creer que mayor conservacion sus secuencias, mas cercano su parentezco. Al agruparlos deberiamos tener una idea de que tan cercana es una especie de otras.

##### 7. ¿Qué evidencias nos aportaría este análisis, a la luz de la evolución?

  Podemos identificar que a nivel de proteinas tenemos muchos mas parentezcos en especies que creeriamos ser de especies totalmente diferente, la evidencia nos aporta una trayectoria evolutiva en la cual nos hace mas cercanos a unas especies que a otras.

##### 8. A juzgar por los organismos participantes, ¿cuáles creería que deberían estar más agrupados en el árbol filogenético?

  Yo creeria que en general estarian separados por mamiferos, peces, anfibios, reptiles. 
    
##### 9. Observemos el árbol filogenético. ¿Concuerda con lo esperado? ¿De qué organismos son los citocromos c más parecidos? ¿Cómo se explica?

![true](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP4_EnQueSePareceUnaVacaYUnaGallina/practica/extra/tree.png)

En lineas generales si. La "Xenopus laevis" me desconcierta un poco. 
