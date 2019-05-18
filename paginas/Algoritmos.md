
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
https://amtdb.org/records/
2. 
>Dloop_rCRS_Mitomap_H2a2
accgctatgtatttcgtacattactgccagccaccatgaatattgtacggtaccataaatacttgaccacctgtagtacataaaaacccaatccacatcaaaaccccctccccatgcttacaagcaagtacagcaatcaaccctcaactatcacacatcaactgcaactccaaagccacccctcacccactaggataccaacaaacctacccacccttaacagtacatagtacataaagccatttaccgtacatagcacattacagtcaaatcccttctcgtccccatggatgacccccctcagataggggtcccttgaccaccatcctccgtgaaatcaatatcccgcacaagagtgctactctcctcgctccgggcccataacacttgggggtagctaaagtgaactgtatccgacatctggttcctacttcagggtcataaagcctaaatagcccacacgttccccttaaataagacatcacgatggatcacaggtctatcaccctattaaccactcacgggagctctccatgcatttggtattttcgtctggggggtatgcacgcgatagcattgcgagacgctggagccggagcaccctatgtcgcagtatctgtctttgattcctgcctcatcctattatttatcgcacctacgttcaatattacaggcgaacatacttactaaagtgtgttaattaattaatgcttgtaggacataataataacaattgaatgtctgcacagccActttccacacagacatcataacaaaaaatttccaccaaaccccccctCCCCCgcttctggccacagcacttaaacacatctctgccaaaccccaaaaacaaagaaccctaacaccagcctaaccagatttcaaattttatcttttggcggtatgcacttttaacagtcaccccccaactaacacattattttcccctcccactcccatactactaatctcatcaatacaacccccgcccatcctacccagcacacacacaccgctgctaaccccataccccgaaccaaccaaaccccaaagacaccccccacagtttatgtagcttacctcctcaaagcaatacactgaaaatgtttagacgggctcacatcacccc
	


### Ejercicio
Vamos a realizar un alineamiento de varias secuencias mitocondriales. [Datos mitocondriales](https://docs.google.com/spreadsheets/d/1ajSiBLri_EdqfFWWOInqOYX3KH7KtOf-oTykd0f-58s/edit?usp=sharing)

Link para descargar las secuencias con las que haremos el árbol  
Ahora vamos a descargar las secuencias a alinear  


sed 's/^/>/' BaseCol1,2 | sed 's/\t/\n/'

### Linux Edición de Archivos   
> Aprenderás a editar archivos y visualizar el contenido de archivos.   
> Aprenderás a copiar, mover y renombrar archivos en el sistema de directorios.  

`$ nano`  
`$ head`  
`$ cat`  
`$ cp`  
`$ mv`   
Wild character  `*`  

`ls *`  


[documento colaborativo ](https://etherpad.net/p/compbio)  

