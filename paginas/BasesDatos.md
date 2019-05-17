# Sesión 5 Datos genómicos y Bioinformática   

## 5.1 ¿Qué es la bioinformática?  
Bioinformática es un conjunto de técnicas y algoritmos computacionales aplicadas a datos biológicos. Es una nueva área de estudio que combina biología molecular con ciencias computacionales. Un reto mayor que la bioinformática enfrenta es organizar la gran cantidad de información obtenida gracias a las nuevas tecnologías de secuenciación. Veamos ¿qué es la bioinformática? en esta [presentación](https://docs.google.com/presentation/d/1YVe0m1G_4EgnF9--HmRjnNluNHYqXNrpozsXTktSNgc/edit?usp=sharing)    

### La información Biológica se almacena en grandes bases de datos.  
Las bases de datos que almacenan información biológica pueden ser públicas o privadas. En ellas, los usuarios acumulan información de los organismos. Esta información es usualmente procesada por algún paquete de análisis para proporcionar una visualización.  

#### [The National Center for Biotechnology Information NCBI](https://www.ncbi.nlm.nih.gov/)  
NCBI es una de las grandes bases de datos biológicas contiene información de una extensa variedad de organismos incluyendo genes, genomas, proteinas, clasificación taxonómica, etc.  

Ejemplo de búsqueda en NCBI:
1. Búsqueda individual
   Ve a la página de NCBI y escribe mithocondrial en el buscador  
   ¿Qué resultados te salen?  
   
2. Búsqueda con modificadores AND y NOT   
 De hecho NCBI agrupa varias bases de datos, vamos a explorar taxonomy y nucleotide. Selecciona Nucleotide como base de datos y realiza la siguiente búsqueda.   
   
`"mitochondrial" [title]AND "D-loop"[title] NOT "segment"[title] AND "homo" [organism]  `    
  
¿Qué obtienes?  

### El formato fasta  
En bioinformática los formatos de los archivos son importantes para su posterior tratamiento. Nosotros necesitaremos el formato fasta para posteriores análisis. Por ello haremos un ejercicio para que te familiarices con él. Este formato consiste en una línea con el símbolo '>' antes del nombre identificador de la secuencia, y después un salto de línea y la secuencia como tal.  
  
Ejercicio  
  
De los resultados que visualizaste en tu segunda búsqueda, obtén la secuencia fasta de un D-loop mitocondrial y anótala en el documento colaborativo. Para ello debes hacer click en algún resultado de tu interés y después seleccionar FASTA en la parte superior izquierda.  

Descarga tu secuencia de tu correo y colócala en el Escritorio. ¿Es la secuencia de NCBI idéntica a la tuya?, ¿Qué diferencias ves? Anota tu conclusión en el documento colaborativo.  

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
