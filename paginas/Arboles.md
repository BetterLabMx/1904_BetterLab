# Árboles filogenéticos
En esta sección vamos a construir un árbol filogenético que contenga a tu secuencia y otras secuencias de ADNmt. Finalmente lo visualizaremos junto con algunos metadatos.  

## Aŕbol filogenético.  
1. Antes de construir el árbol debemos alinear nuestro archivo fasta que preparamos previamente. Súbelo al 
[Alineador mafft](https://www.ebi.ac.uk/Tools/msa/mafft/) y obtén un alineamiento.  

2. Toma ese alineamiento y llévalo a este servidor para obtener un árbol filogenético.  
[Creador de árboles](http://www.phylogeny.fr/simple_phylogeny.cgi) 
¿Qué observaste?  

3. Descarga el formato newick y guárdalo en tu carpeta BetterLab, es lo que utilizaremos en la siguiente sección.  

## Metadatos  
Los metadatos son datos sobre los datos usualmente vienen en una tabla de excel. Por ejemplo la latitud y la longitud del muestreo son metadatos que vienen en el archivo BaseMitocondrial que descargaste. Hay una serie de consejos sobre buenas prácticas de toma de metadatos. En cuanto a los datos, las buenas prácticas nos dicen que siempre conservemos los datos originales.    

### [Microreact  ](https://microreact.org/)  un visualizador de datos y metadatos  

Microreact es una plataforma de visualización de datos que está especializada en epidemiología genómica. En particular Microreact ayuda a explorar árboles filogenéticos conectándolos con mapas señalando los lugares dónde ocurrieron las infecciones.  

Nosotros utilizaremos esta plataforma primero para ver los lugares y años donde nacimos todos nosotros!   

####   Ejercicio primera parte
Llena con tus datos la [Hoja de cáculo de google drive ](https://docs.google.com/spreadsheets/d/1IyFEEVDgBtfRb9rUEX9JePTl7ARiHAxyR3n1RKtk_OQ/edit?usp=sharing)
  
Para agregar las coordenadas de tu lugar de nacimiento:
1) Abre [Google Maps  ](https://www.google.com.mx/maps)  
2) Busca tu lugar de nacimiento  
3) Da click derecho sobre el lugar del que quieres extraer las coordenadas. Debe aparecer un cuadrito en la parte inferior del mapa    (Si no aparece utiliza click derecho -> ¿Qué hay aquí?)
4) Pulsa sobre las coordenadas que están abajo del cuadro  
5) Copia y pega la latitud y longitud en las columnas de la hoja de cálculo que abriste en el paso   

### Recuerda que cuando se llena la hoja de cálculo se deben seguir las buenas prácticas de colecta de metadatos.

####   Ejercicio segunda parte
a) Abre [Microreact  ](https://microreact.org/)  
b) Inicia sesión utilizando tu cuenta de gmail  
c) Da click en Upload  
d) Ve a la hoja de cálculo y copia el link que está en 'File->Publish' o 'Archivo->Publicar'  
e) Pega el link donde pide un archivo .csv  
f) da click en continue (without tree)  
g) Ingresa el título de tu proyecto de visualización  
h) Visualiza tus resultados!  

### Visualización simultánea de árboles y mapas
Ahora regresa a la página principal de microrreact.  
Selecciona el proyecto 'Zika virus in the Americas', discute con tu compañero de al lado y escriban sus respuestas en el documento colaborativo.  
¿En dónde se tuvo el primer registro de este virus?  
¿Cuál fue el primer lugar de América en el que se detectó zika?  
¿En qué año fue la epidemia que se describe en este artículo?  
¿Cuál es el ancestro más cercano a los virus de la epidemia?  
¿Cuántos sitios de microencefalia en Brasil reportaron?
¿Cuáles virus tienen el genoma más grande y más chico?

## Metadatos con tus secuencias mitocondriales.  
Ahora vamos a crear una visualización de microreact que incluya tanto las coordenadas de latitud y longitud donde se tomó la muestra de DNAmt como el árbol filogenético de las secuencias. Para ello crea una hoja de cálculo de google docs, que contenga la base de datos que ya descargaste y además tu secuencia con tus metadatos.   

### Identificación de haplogrupos mitocondriales   
Un haplogrupo es definido por las variaciones del ADN mitocondrial (ADNmt) humano. La determinación de haplogrupo se realiza utilizando los resultados obtenidos por secuenciación. En la figura 5 se muestran ejemplos de haplogrupos incluyendo el metadato que registra de dónde proviene.  
![Figura5](Figura5.png)   
Figura 5.- En este mapa se muestran los haplogrupos identificados por letras y las regiones de donde provienen.  


## Retos e ideas para tu propio proyecto  
Aquí te presentamos una secuencia misteriosa, ¿Puedes determinar a qué haplotipo pertenece?    
   
>Secuencia_misteriosa  
AATTTTATTTTTTAACCTAACTCCCCTACTAAGTGTACCCCCCCTTTCCCCCCCAGGGGGGGTATACTAT  
GCATAATCGTGCATACATTTATATACCACATATATTATGGTACCGGTAATATATACTATATATGTACTAA  
ACCCATTATATGTATACGGGCATTAATCTATATTCCACATTTCTCCCAATGTCCATTCTATGCATGATCC  
AGGACACACTCATTCACCCTCCCCATAGACAGTTCCAAACCACTACCAAGTCACCTAACTATGAATGGTT  
ACAGGACATAAATCTCACTCTCATGTTCTTCCCCCAACAAGTCACCTAACTATGAATGGTTACAGGACAT  
ACATTTAACTACCATGTTCTAACCCATTTGGTTATGCTCGCCGTATCAGATGGATTTATTGATCGTCCAC  
CTCACGAGAGATCAGCAACCCCTGCTTGTAATGTACTTCATGACCAGTCTCAGGCCCATTCTTTCCCCCT  
ACACCCCTCGCCCTACTTGCCTTCCACCGTACCTCTGGTTCCTCGGTCAGGCACATCCCATGCATAACTC  
CTGAACTTTCTCACTTTTCACGAAGTCATCTGTGGATTATCTTCCCCTCTTTAGTCCGTGATCGCGGCAT  
CTTCTCTCTTCTATTGCTGTTGGTTCCTTCTCTTTTTGGGGCTTCTTCACAGGTTACCCTTCACAGTGCG  
GGTGCGGAGTGCTATTCAAGTGAAGCCTGGACTACACCTGCGTTGCGTCCTATCCTAGTCCTCTCGTGTC  
CCTCGATGAGACGGTTTGCGTGTATGGGGAATCATCTTGACACTGATGCACTTTGGATCGCATTTGGTTA    
TGGTTCTTCCACCCCCCCCGGTAAATGGTGCTATTTAGTGAATGCTTGTCGGACATATTTTTATCAATTT    
TCACTTCCTCTATTTTCTTCACAAAACTAGGAAATTCACCACAATTTTTTCTTTGTTATTTTTTAATTTT  
TTTTTTATTTTTTAAAAACATTTTTTAAAAAACTAAATTACATACAAACTACCGCATAAAATCCCTCAAA  
CTATACAAACGTTTATCGTATAATATATATACATTATTGTTTATTCTATCATTATTAGAGAAACTCCACT  
ACCAAAACCATCATTAAAACAAAAATTTACATGCCACTTAACTCCCCTCACAAACAATCGTTATTTATAT  
TGTTAATTAGCAAACACAAAACCTGCCTTCTACCACTATAAA  
  
Esta es una base de datos de [DNAmt antiguo](https://amtdb.org/records/), a cuál de ellas te pareces más.  
  
Busca otras paginas de análisis de DNAmt. ¿Qué logras aprender de tu secuencia?  

Esta es una base de datos de [Haplogrupos](https://www.mitomap.org/foswiki/bin/view/MITOMASTER/WebHome).


Este es un artículo de [Haplogrupos en mesoamericanos nativos](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3446984/#pone.0044666). 

Otra página de [mitomap](https://www.mitomap.org/MITOMAP)



