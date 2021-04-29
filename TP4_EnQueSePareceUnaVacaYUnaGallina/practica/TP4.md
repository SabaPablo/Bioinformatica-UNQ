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
##### 6. ¿Creeríamos que todos los organismos se asemejan por igual al resto, o se pueden identificar grupos de mayor similitud? Si es así, ¿tienen sentido?
##### 7. ¿Qué evidencias nos aportaría este análisis, a la luz de la evolución?
##### 8. A juzgar por los organismos participantes, ¿cuáles creería que deberían estar más agrupados en el árbol filogenético?
##### 9. Observemos el árbol filogenético. ¿Concuerda con lo esperado? ¿De qué organismos son los citocromos c más parecidos? ¿Cómo se explica?


