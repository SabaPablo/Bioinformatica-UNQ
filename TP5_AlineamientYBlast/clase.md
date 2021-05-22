#### Evolución molecular

La **biodiversidad** es gracias a las mutaciones.
Los **genes** van generando mutaciones.

Dos secuencias son **homólogas** cuando tienen un **ancestro en común**.
Si dos secuencias no son **homólogas** no tiene sentido que las compare!
Dos secuencias deben mostrar almenos un 40% de identidad para considerarse que tienen un **ancenstro en común**.

Las secuencias homólogas pueden ser ortólogas o parálogas:
- **Ortólogos**: Genes que comparten el último ancestro común y cuya divergencia se debe a la especiación.
- **Parálogos**: Genes que debido a una duplicación, ya no comparten el último ancestro. Frecuentemente tienen funciones distintas. Copias que tiene la posibilidad de evolucionar.

![Genes Orto Para](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/homology_en1.png)

#### Alineamiento de secuencias

El alineamiento secuecial es un procedimiento por el cual podemos comparar 2 
no siempre es el que me da mejor score sino los que me representan mejor la naturaleza, para ello vamos a penalizar el uso de gaps de diferente forma

existen matrices de sustitución que sirve para simular los cambios en secuencias de proteinas, usa informacion evolutiva para comparar aminoácidos. Con ellos puntua que tan probable o improbable es esa transformación.
Margaret Dayhoff fue quien desarrolló las matrices PAM para aminoácidos. Los datos de las matrices fueron tomados con datos experimentales.

![Matriz de sustitución](https://github.com/wisaku/Bioinformatica-UNQ/blob/master/TP5_AlineamientYBlast/practica/extra/pam1.png)


Tecnicas y programas de alineamiento

| Local  |  Global   |
|--------|--------|
|Mejor alineamiento a lo largo de 2 secuencias | Mejor alineamiento del segmento más largo entre 2 secuencias|
|Smith Waterman| Needleman Wunsch |
| Búsquedas de sub-secuencias o regiones | Tienen la misma organización secuencial?|
| Permite localizar segmentos o dominios comunes| sirve para proteinas|


Clustal usa NW

BLAST es un algoritmo de busqueda de similitud secuencial.

AHCNIRVS
AICINRCK

