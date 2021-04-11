# BIOMOLÉCULAS

## TRABAJO PRACTICO 1

### **RETO I**
#### ¿Podrías buscar un ejemplo de macromoléculas que almacenen información sobre la ‘identidad’ de un organismo dado?

Un ejemplo de macromoléculas es el ácido núcleico (ADN)

### **RETO II**
####Proponé una forma de expresar la información contenida de la estructura primaria de las proteínas usando tipo de datos de los lenguajes de programación que conocés.
Una forma de expresar la información contenida  de la estructura primaria de las proteinas puede ser un "String".

### ***RETO III***
####¿ En qué tipo de datos podrías expresar la información de la estructura terciaria proteica?
Para poder contener los datos que expresa la informacion de la estructura terciaria proteica (coordenadas y elemento) creo que una lista de objetos seria la mejor opción.

### **RETO IV** 
####Rosalind Franklin es una científica muy relevante, que tuvo menos reconocimiento del merecido. ¿Cuáles fueron sus contribuciones en este campo? ¿Qué nos cuenta su historia acerca del mundo de la ciencia?

- Rosalind Franklin logro obtener imagenes con ADN lo suficientemente nitidas que permitian ver y explicar la estructura de un ADN. Sus resultados sugerían una estructura helicoidal con 2,3 o 4 cadenas y con los grupos fosfatos hacia el exterior.
- Esta historia aparte de marcar un quiebre en la forma de entender y interpretar la estructura de un ADN, pone de manifiesto el maltrato y el intento de desprestigio que existia y que existe sobre las mujeres en ciencia. 


### **RETO V**
####Proponé en pseudocódigo un programa que prediga la estructura secundaria que adpotará cada residuo (aminoácido) de la secuencia proteica dada, especificandola con H (si es una hélice), B (si es una hoja beta plegada) y L (si es un bucle o loop).

##### &diams; PREGUNTA DISPARADORA: ¿Qué inputs tendra tu programa? ¿De qué modo se te ocurre configurar el output?

Como inputs en principio va a tener la estructura primaria. Pero a su vez va a usar una base de datos donde nos indique que tan probable sea en una secuencia exista una hélice, una beta plegada o un bucle.
El output sera un string con las siglas indicadas que representaran la secuencia secundaria.

```
fun predecirSecuenciaPrimariaASecundaria(secuenciaAPredecir: String){
	/*
		PROPOSITO: predice la secuencia secundaria que adopta cada residuo de 
		la secuencia proteica "secuenciaAPredecir"
		RETORNA: un String que representa la estructura secundaria predecida.
		OBSERVACIÓN: especificando con H (si es una hélice), B (si es una hoja beta plegada) y L (si es un bucle o loop).
	*/
	var secuenciaProcesada = secuenciaAPredecir
	estructuraSecundariaMejorRepresentadaHastaAhora = ""
	while(noEsVacia(secuenciaProcesada)){
		porcionYEstructura = porcionYEstructuraSecundariaConMejorProbabilidad(secuenciaProcesada)
		secuenciaProcesada = secuenciaProcesada.quitarLosPrimerosElementosDeLaLista(porcionYEstructura.porcion.size())
		 estructuraSecundariaMejorRepresentadaHastaAhora = estructuraSecundariaMejorRepresentadaHastaAhora + porcionYEstructura.estructura
	
	}	
	return estructuraSecundariaMejorRepresentadaHastaAhora
	
}

fun porcionYEstructuraSecundariaConMejorProbabilidad(estructuraPrimaria: String){
		/*
		PROPOSITO: obtener la porcion de estructura primaria y elemento secundario que 
		mejor probabilidad exista 
		RETORNA: una Equivalencia 
		OBSERVACIÓN: especificando con H (si es una hélice), B (si es una hoja beta plegada) 
		y L (si es un bucle o loop).
	*/
	var mejorProbabilidadHastaAhora = 0
	var estructura = ""
	secuenciaPrimariaConMasProbabilidad = ""
	estructuraPrimaria.forEach{ elemento -> 
		estructura = estructura + elemento
		val predisposicion = probabilidadConLaEstructura(estructura) 
		// toma la estructura y la busca en la base de datos, devuelve la estructura 
		// secundaria con mayor probabilidad Predisposicion
		if(predisposicion.probabilidad > mejorProbabilidadHastaAhora){
			mejorProbabilidadHastaAhora = predisposicion.probabilidad
			estructuraSecundaria = predisposicion.estructura
			secuenciaPrimariaConMasProbabilidad = predisposicion.secuencia
		}
	}
	return Equivalencia(secuenciaPrimariaConMasProbabilidad, estructuraSecundaria)

}


data class Equivalencia(val porcion: String, val estructura:String)

data class Predisposicion(val secuencia, val probabilidad: String, val estructura:String)
```

#### **PARA PENSAR:** ¿Cuantas proteínas puede sintentizar un organismo? ¿De qué depende la cantidad y la caracterista de las proteínas que puede sinitetizar un organismo?

- La catidad y el tipo de proteinas que puede sintetizar un organismo varia, pero podrian ser millones.

- Depende de la complejidad de dicho organismo, un organismo simple va a sintentizar menos proteinas que uno mas complejo

### **RETRO VI**
#### ¿Qué hace distintos a los individuos de una especie? Propone una forma de corroborar tu respuesta realizando un diagrama de un posible método computacional para dicho fin.

