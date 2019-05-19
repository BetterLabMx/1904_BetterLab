
# Algoritmos en biología  
Un algoritmo es un proceso con un número de pasos finito que tiene un principio y un final. Por ejemplo cambiar una llanta es un algoritmo. En Biología se aplican algoritmos matemáticos y computacionales para estudiar las variaciones de secuencias. En esta sesión estudiaremos cómo alinear secuencias, cómo calcular distancias entre ellas, y finalmente cómo visualizar estos resultados en un árbol filogenético.      

## Distancia entre dos secuencias  
La distancia más simple entre dos secuencias es un 0 si tienen la misma base o un 1 si no la tienen. Mira el siguiente ejemplo 
![dis1](https://github.com/nselem/cbhonduras/blob/master/imagenes/distanciaH1.png)  
¿Qué pasa aquí?  
![dis2](https://github.com/nselem/cbhonduras/blob/master/imagenes/dist2.png)  

Cuál es la distancia de Hamming entre la secuencia 1 y las demás secuencias?? 

>seq1  
CAGGACCACACA  
>seq2  
CAGGACCACACA  
>seq3  
CACGACCACACA  
>seq4  
CGGACCACACA  
¿Qué distancia te gustaría que fuera?  

## Algoritmos de alineamiento    
Como podemos ver, eventos evolutivos como las deleciones e inserciones crean la necesidad de alinear secuencias para poder obtener un mejor estimado de sus distancias evlutivas.  

### Ejemplo 1    
>seq1  CAGGACCACACA   
>seq3  CA-GACCACACA   

### Ejemplo 2
Vamos a utilizar una versión [mafft](https://www.ebi.ac.uk/Tools/msa/mafft/) en línea para hacer un alineamiento ambas secuencias de ANDmt.  

1. Toma tu secuencia consenso y pégala en el espacio correspondiente del alineador.  
2. Ahora pega esta secuencia de referencia de DNAmt humano y alínealas.  
DloopH2a2  
accgctatgtatttcgtacattactgccagccaccatgaatattgtacggtaccataaatacttgaccacctgtagtacataaaaacccaatccacatcaaaaccccctccccatgcttacaagcaagtacagcaatcaaccctcaactatcacacatcaactgcaactccaaagccacccctcacccactaggataccaacaaacctacccacccttaacagtacatagtacataaagccatttaccgtacatagcacattacagtcaaatcccttctcgtccccatggatgacccccctcagataggggtcccttgaccaccatcctccgtgaaatcaatatcccgcacaagagtgctactctcctcgctccgggcccataacacttgggggtagctaaagtgaactgtatccgacatctggttcctacttcagggtcataaagcctaaatagcccacacgttccccttaaataagacatcacgatggatcacaggtctatcaccctattaaccactcacgggagctctccatgcatttggtattttcgtctggggggtatgcacgcgatagcattgcgagacgctggagccggagcaccctatgtcgcagtatctgtctttgattcctgcctcatcctattatttatcgcacctacgttcaatattacaggcgaacatacttactaaagtgtgttaattaattaatgcttgtaggacataataataacaattgaatgtctgcacagccActttccacacagacatcataacaaaaaatttccaccaaaccccccctCCCCCgcttctggccacagcacttaaacacatctctgccaaaccccaaaaacaaagaaccctaacaccagcctaaccagatttcaaattttatcttttggcggtatgcacttttaacagtcaccccccaactaacacattattttcccctcccactcccatactactaatctcatcaatacaacccccgcccatcctacccagcacacacacaccgctgctaaccccataccccgaaccaaccaaaccccaaagacaccccccacagtttatgtagcttacctcctcaaagcaatacactgaaaatgtttagacgggctcacatcacccc
	

### Linux Manipulación de Archivos 
En esta sección prepararemos un archivo que contendrá varias secuencias de DNAmt en formato fasta. En este archivo agregaremos nuestra secuencia consenso y posteriormente alinearemos todas las secuencias. Para tener las secuencias en formato fasta necesitamos aprender un poco más del uso de la terminal.  
  
> En esta sección aprenderás a  
> Editar archivos y visualizar el contenido de archivos.   
> Copiar, mover y renombrar archivos en el sistema de directorios.  

Para ello necesitarás los siguientes comandos:  
`$ nano`	Editor de texto  
`$ head`  Permite visualizar las primeras líneas de un texto  
`$ cp`	Copia un archivo  
`$ mv`   Mueve o renombra un archivo  
`$ sed`  Permite editar un archivo sin abrirlo  
`$ cut`	Recorta columnas    

#### Ejemplo 1 Creación de un archivo de dos coulmnas con secuencias de DNAmt
1. Descarga los [Datos mitocondriales](https://docs.google.com/spreadsheets/d/1ajSiBLri_EdqfFWWOInqOYX3KH7KtOf-oTykd0f-58s/edit?usp=sharing) que contienen una variedad de haplotipos y que preparamos para ti. Este archivo tiene varias columnas, la primera es el identificador de la secuencia, la segunda la secuencia, la tercera el haplotipo y después la latitud y longitud de donde este haplotipo es característico. Para el formato fasta que necesita el alineador sólo ocuparemos las dos primeras columnas. Los otros metadatos no serán necesarios por el momento. Así pues vamos a modificar este archivo mediante el uso de la terminal.  
  
  
2. Abre tu terminal, verifica en que directorio estás y ve al directorio BetterLab  
`$ pwd`  
`$  cd Desktop/BetterLab`    
  
3. Copia a BetterLab el archivo BaseMitocondrial que acabas de descargar. Este archivo está ubicado en Downloads.  
`$ cp /home/usuario/Downloads/Base<autocompletar> BaseMitocondrial .`    
  
4. Ahora vamos a visualizar las primeras líneas del archivo con el comando `head`  
`$ head -n3 BaseMitocondrial`  
El modificador -n3 nos dice que vamos a ver únicamente las tres primeras líneas del archivo. ¿Está en formato fasta? Si no está, ¿qué le falta?  

5. Recortaremos las dos primeras columnas del archivo para acercarnos al formato fasta. Linux lo hace por nosotros con el comando `cut`  
`cut -f1,2 BaseMitocondrial`

6. Verifica que el archivo BaseMitocondrial haya quedado recortado. ¿Qué pasó? 
No se recortó porque sólo visualizamos en la pantalla como quedaría si lo recortáramos. Para guardar este archivo tenemos que utilizar el comando _redireccionar_ que en linux está representado por el símbolo ">"  
`cut -f1,2 BaseMitocondrial> Base_Col1_2`  
Ahora sí creamos un nuevo archivo. ¿Cómo se llama este nuevo archivo?
  
#### Ejercicio Visualiza las primeras líneas del último archivo creado.  
Verifica con `ls -tr` cuál es el último archivo creado y después visualiza sus primeras tres líneas.  ¿Qué comandos necesitas?  


#### Ejemplo 2 Concatenar comandos con pipe  
Ya tienes un archivo con dos columnas, una el identificador y la otra la secuencia. Para el formato fasta necesitamos que la línea empiece con ">". Por ello debemos sustituir todos los inicios de línea con ">"  
  
El comando para sustituir fragmentos de palabras es  
`sed 's/>Fragmento a sustituir>/<Fragmento a incluir en lugar de>/ <Nombre del archivo>`    

En este caso deseamos incluir ">" y deshacernos de "^" que es el caracter especial de linux para el inicio de línea.  
  
1. Sustituyamos el inicio de línea por el mayor que.  
`$ sed 's/^/>/' Base_Col1_2`   
¿Se modificó el archivo? ¿Qué tendrias que hacer para guardar los cambios?  
`$ sed 's/^/>/' Base_Col1_2 > BaseMit_c12.fasta1`   

2. Ahora nos falta sustituir el tabulador o "\t" por el salto de línea o "\n".  
`$ sed 's/\t/\n/' BaseMit_c12.fasta1 > BaseMit_c12.fasta2`  

Donde finalmente queda nuestro archivo fasta en BaseMit_c12.fasta2.
  
Ahora bien utilizando el "pipe" o concatenador de comandos en linux podríamos habernos guardado mucho tiempo ya que pipe concatena la salida de un comando como la entrada del siguiente.  ¿Qué te resulta de ejecutar el siguiente comando?  
  
`$ sed 's/^/>/' Base_Col1_2 | sed 's/\t/\n/'`  
  
#### Ejemplo 3 Crea tu propio script en la terminal  
Ahora vas a aprender a crear tu script.  

utiliza nano para crear el archivo `creaFastaMitocondrial.sh` 

1. `nano creaFastaMitocondrial.sh`  

2. Escribe la siguiente instrucción dentro de tu archivo `creaFastaMitocondrial.sh`  
`sed 's/^/>/' $1 | sed 's/\t/\n/' >$1-fasta  `  
Aquí $1 tomará el valor del primer parámetro que le pases al script. Tal como hacía finchtv.  

3. Ejecúta creaFastaMitocondrial.sh  
Después de salir de nano teclea  
`bash creaFastaMitocondrial.sh Base_Col1_2  `  
¿Se creo algún nuevo archivo? ¿Qué contiene?  

Listo has creado tu primer script que podrías ejecutarlo sobre muchos archivos distintos. 

4. Para finalmente tener un archivo limpio de errores. Abre el archivo .fasta en nano y bórrale las tres primeras líneas que no corresponden a secuencias sino a los encabezados de la hoja.  

Este archivo es un fasta se secuencias que utilizaremos en la siguiente sesión para crear un árbol filogenético.  
