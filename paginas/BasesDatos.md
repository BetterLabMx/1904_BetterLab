# Sesión 5 Datos genómicos y Bioinformática   

## 5.1 ¿Qué es la bioinformática?  
Bioinformática es un conjunto de técnicas y algoritmos computacionales aplicadas a datos biológicos. Es una nueva área de estudio que combina biología molecular con ciencias computacionales. Un reto mayor que la bioinformática enfrenta es organizar la gran cantidad de información obtenida gracias a las nuevas tecnologías de secuenciación. Veamos ¿qué es la bioinformática? en esta [presentación](https://docs.google.com/presentation/d/1YVe0m1G_4EgnF9--HmRjnNluNHYqXNrpozsXTktSNgc/edit?usp=sharing)    

### La información Biológica se almacena en grandes bases de datos.  
Las bases de datos que almacenan información biológica pueden ser públicas o privadas. En ellas, los usuarios acumulan información de los organismos, esta información es usualmente procesada por algún paquete de análisis asociado a ella.  

#### [The National Center for Biotechnology Information NCBI](https://www.ncbi.nlm.nih.gov/)  
NCBI es una de las grandes bases de datos biológicas contiene información de una extensa variedad de organismos incluyendo genes, genomas, proteinas, clasificación taxonómica, etc.  

Ejemplo:
Selecciona Nucleotide como base de datos y realiza la siguiente búsqueda. ¿Qué obtienes?  
"mitochondrial" [title]AND "D-loop"[title] NOT "segment"[title] AND "homo" [organism]  

Obtén la secuencia de un D-loop mitocondrial y anótala en el documento colaborativo.   
¿Es idéntica a tu ensamblado?. ¿Qué diferencias ves? Anóta tu conclusión en el documento colaborativo.  

## 5.2 La terminal de linux  
Para visualizar nuestro electroferograma necesitamos iniciar el visualizador desde una terminal de linux. Por ello, a continuacion estudiaremos un poco de bash, el lenguaje de linux. 

> En esta lección aprenderás a moverte en el sistema de directorios:  
> - Conocer tu ubicación en el sistema de directorios (pwd)  
> - Conocer el contenido del directorio en el que te encuentras.   
> -Cambiarte de directorio.  

`cd `Cambio de directorio.    
`ls` Listado del contenido del directorio.    
`pwd`"Path to working directory" Muestra la ubicación del directorio.    

Para conocer más sobre la terminal de linux te recomendamos <a href="https://swcarpentry.github.io/shell-novice-es/"> Software Carpentry </a>

Para mover archivos utilizamos el comando move, y para copiarlos el comando copy.  
`mv`
`cp`

Para crear archivos utilizaremos el editor nano.  
