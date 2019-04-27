# Descubriendo tu información genética  
![BetterLab Logo](images/BetterLab.png)   

      
    
## Informacion General  
Bienvenido a aprender sobre tu información genética. En este taller adquirirás nociones de biología tanto experimental como computacional. Te presentamos tres herramientas de trabajo, este sitio web, un documento colaborativo así como el resúmen del curso.  

Esta será la página web del taller, donde encontrarás el temario y los protocolos del curso. Iremos agregando información sobre las sesiones de trabajo.  

Además utilizaremos un [documento colaborativo](https://etherpad.net/p/190419_BetterLab) donde podemos anotar dudas de los participantes y compartir información todos al mismo tiempo. Los documentos colaborativos ayudan a llevar un registro del trabajo comunitario y te permiten tener una herrammienta de consulta en el futuro. 

En este [resumen]( https://github.com/BetterLabMx/1904_BetterLab/blob/master/paginas/Resumen.pdf) puedes encontrar los protocolos y la información que utilizaremos taller. 
  
## Calendario   
  
<table>
    <tr>
             <td>Sábado 27       </td> <td>           Domingo 28                 </td>
  </tr>  
      <tr>
      <td> Sesión 1 (10:00-10:50) Introducción teórica a la Biología Molecular.   </td>  
      <td>  Sesión 3 (10:00-11:00) Introducción teórico-práctica a la reacción de PCR</td>
  </tr>
      <tr><td>Coffee Break</td><td>Coffee Break</td>    </tr>
    <tr>
          <td>Sesión 2 (11:00-14:00) Extracción de DNA</td>
          <td>Sesión 4 (11:20-14:00) Termociclado y electroforesis </td></tr>  
    <tr><td>Sábado 4</td><td>Domingo 5 </td></tr>
    <tr>
          <td> Sesión 5 (10:00-11:45) Genómica y Bioinformática          </td>
      <td>Sesión 7 (10:00-11:45) <a href="paginas/genomica/genomica.md"> Arboles y metadatos</a></td>
    </tr>
    <tr><td>Coffee Break</td><td>Coffee Break</td>    </tr>
    <tr>
          <td> Sesión 6 (12:00-14:00 am) Introducción y <a href="https://swcarpentry.github.io/shell-novice-es/"> bash </a> 
        </td>    <td>Sesión 8 (12:00-14:00 pm) Proyectos y exposición </td>
    </tr>
</table>  


## Temario detallado  
<table> 
<tr>
      <td><b> Sesión 1 </b> <br>
            1 <a href="https://github.com/BetterLabMx/1904_BetterLab/blob/master/paginas/GenomaMitocondrial.md">Introducción a la Biología Molecular.</a> <br>
      1.1 Fundamentos del uso del ADN mitocondrial 
      para identificación humana y ancestría.<br>
      1.2 Conociendo el genoma mitocondrial.<br>
      1.3 Legislación de la genética humana.<br>
      </td>
     <td><b> Sesión 2 </b> <br>
     2.1 Extracción de DNA y  conservación <br>
     2.2 Visualización del ADN genómico Tarde libre<br>
           </td></tr>
      <tr>
     <td><b> Sesión 3 </b> <br>
      3.1 Realizando PCR<br>
      3.2 Preparando Mix PCR<br> 
           </td>
      <td><b> Sesión 4 </b> <br>
      4.1 Amplificando la región mitocondrial <br>
      4.2 Visualizando por electroforesis la región mitocondrial <br>
      </td>
</tr>      
<td><b>Sesión 5</b><br> 
    5.1 Visualización de fragmentos <br> 
    5.2  Recepción de los datos de secuenciación <br> 
      </td>
<td><b>Sesión 6</b><br> 
    6.1  Alineamientos y  filogénias <br> 
    6.2  Interpretación de la secuenciación <br> 
      </td>
<tr>
<td><b>Sesión 7</b><br> 
      7.1 Encontrando la ancestría usando haplogrupos <br> 
      </td>
<td><b>Sesión 8</b><br> 
      8.1 Software de antropología genómica. <br> 
      8.2 Marcadores biomédicos y genética forense<br> 
      </td>
      </tr>
</table>    
___  
  
## Instalaciones y requerimientos previos  
<h2 id="setup">Setup</h2>  

<p>
  Para participar en este taller necesitas acceso al siguiente software. Además necesitarás acceso a un navegador como chrome o firefox.   
  </p>
<p>
  Aqui hay una referencia de posibles problemas durante la instalación.  
  <a href = "https://github.com/carpentries/workshop-template/wiki/Configuration-Problems-and-Solutions">Wiki de problemas de instalación y sus soluciones. </a>.
</p>

<div id="shell">  
  <h3>El Bash Shell</h3>  
  <p>  
    Bash es un intérprete de comandosque te da poder de hacer tareas simples rápidamente.  
  </p>  

  <div class="row">  
    <div class="col-md-4">  
      <h4 id="shell-windows">Windows</h4>  
      <a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>  
      <ol>  
        <li>Baja para windows <a href="https://git-for-windows.github.io/">el instalador de git </a>.</li>  
        <li>Corre el instalador y sigue los siguientes pasos:  
          <ol>  
            <li>Click en "Next".</li>  
            <li>Click en "Next".</li>    
            <li>  
              <strong>  
               Manten el "Use Git from the Windows Command Prompt" seleccioinado y  click en "Next".  
              </strong>  
                Si se te olvida hacer esto algunos programas que necesitarás no funcionaran correctamente.  
                Si esto te pasa regrésate al paso anterior del instalador y selecciona la opción correcta.  
            </li>  
            <li>Click en "Next".</li>
            <li>  
              <strong>  
                Mantén "Checkout Windows-style, commit Unix-style line endings" seleccionado y click en "Next".
              </strong>
            </li>
            <li>  
              <strong>  
                Mantén "Use Windows' default console window" seleccionado y click en "Next".  
              </strong>  
            </li>  
            <li>Click en "Install".</li>
            <li>Click en "Finish".</li>  
          </ol>  
        </li>  
        <li>  
          si tu variable de ambiente "HOME" no está lista (o no sabes qué es esto):
          <ol>
            <li>Abre el prompt (Abre el menu start, escribe <code>cmd</code> y presiona enter [Enter])</li>
            <li>
              Escribe la siguiente línea en la ventana del promt exactamente como se  muestra:  
              <p><code>setx HOME "%USERPROFILE%"</code></p>  
            </li>  
            <li>Presiona [Enter], debes de ver <code>SUCCESS: Specified value was saved.</code></li>
            <li>Para salir del prompr escribe <code>exit</code> y presiona enter [Enter]</li>
          </ol>
        </li>
      </ol>
      <p>Esto te dará ambos Git y Bash en el programa Git Bash.</p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">macOS</h4>
      <p>
        El shell por default en todas las versiones de macOS es Bash, asi que no debes instalar nada.  Podrás accesar a Bash desde la Terminal
        (que se encuentra en        <code>/Applications/Utilities</code>).
        Para la instalación de Git aqui tenemos un <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
        for an example on how to open the Terminal.
        Tal vez quieras mantener la Terminal en tu dock para este taller.  
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        El shell es usualmente Bash, pero si tu máquina es diferente puedes abrir una terminal y escribir <code>bash</code>.  
        No se necesita intalar nada
      </p>
    </div>
  </div>
</div> 
