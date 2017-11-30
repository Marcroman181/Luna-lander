# Luna-lander
## Pràctica html i css del luna lander

[Link del rawgit del luna lander](https://rawgit.com/Marcroman181/Luna-lander/master/lunalander.html)

[Link del rawgit de la pàgina d'instruccions](https://rawgit.com/Marcroman181/Luna-lander/master/instruccions.html)

**Este repositorio contiene una branch con todo el codigo minimificado**

### Documentació

**Cambios realizados respecto al proyecto inicial:**

 -He cambiado el indicador de fuel puesto que este era un GIF y no era posible implementarlo. Por lo tanto el indicador de fuel lo he     realizado con 2 divs.
 -He cambiado el menú, puesto que este estaba compuesto por imagenes. Entonces, el menú esta hecho mediante un div. 

**HTML:**

El HTML tiene la siguiente estructura:

La pantalla està compuesta por varios contenedores principales:
  
  -El contenedor de la izquierda contiene los tres indicadores del juego: El de altura compuesto por dos divs uno dentro del otro, y       el de velocidad y altura compuesto por un div con un fondo y dentro una imagen que nos indica el valor del indicador.
    
  -El contenedor de la derecha que contiene tres subcontenedores. El primero contiene los cuatro botones que vamos a usar para             interaciconar con las opciones del jueog, el segundo contiene el botón de reiniciar y el último el botón para acelerar el cohete. 
    
  -Dos contenedores en el centro para centrar la nave y el fuego.
    
  -Un contenedor en la parte inferior de la pantalla que contiene la luna. 
  
  -Por último, tenemos un contenedor que contiene todos los menús que van a aparecer en la pantalla. Este contenedor nos és útil porque   nos va a permitir que cuando activemos el menú no podamos interaccionar con el juego, es decir, va a ser un contenedor transparente     que ocupará toda la pantalla. Hay dos menús, el de configuración del juego para cambiar la dificultad y el de instrucciones.
  
  -Además, tenemos un contenedor llamado dropdown que contiene el menú desplegable para la pantalla vertical. Para ello, hemos puesto un   contenedor con un botón y de fondo una imagen. Dentro de este contenedor, hay otro contenedor que se hace visible cuando estamos         encima del contenedor dropdown y enseña todos los botones.
  

**CSS horizontal:**

Siguiendo la estructura del html:
  
  -Contenedor de la derecha: Este contenedor està fijado a la parte derecha con un tamaño porcentual a la pantalla, y dentro hay los       tres contenedores colocados con posición absoluta y un tamaño porcentual respecto al anterior. Los botones ocupan un valor               porcentual a la altura del div y están colocado con un display. inline-block i float right. El botón de play estará sin visibilidad     mientras el de pausa esté y viceversa. Las imagenes de reiniciar y botón de motor simplemente están posicionadas con un float right     y dimensionadas porcentualmente. Además, para añadir efectos al pulsar, se cambia de tamaño al pasar por encima con hover y scale, y     con active le damos un color de fondo para destacar cuando pulsamos. 
    
  -El contenedor de la izquierda: Este contenedor es parecido al anteior. El contenedor de fuel contiene otro contenedor dentro que       simula una barra. El contenedor de altura y velocidad contienen un fondo que no se repiten y una imagen posicionada adecuadamente       dentro que seria el indicador. Por otra parte, he añadido unas dimensiones mínimas al contenedor para que la imagen de fondo no se       corte.
    
  -Los contenedores para la nave simplemente están centrados respecto al body y estan dimensionados porcentualmente.
    
  -El contenedor inferior: Éste simplemente está posicionado en la parte inferior y centra la imagen que hay en su interior, la luna.     Además, se dimensiona adecuadamente. 
    
  -El contenedor de menús ocupa toda la pantalla y es transparente, además su z-index debe ser superior al resto para evitar la           interacción con los botones. Cuando no haya ningún meno su visibilidad es none. 
    
  -En el horizontal no hay dropdown, así que no está visible.
    

**CSS vertical:**
    
Siguiendo la estructura del html:
  
  -Contenedor de la derecha: Este contenedor no existe en el vertical, por lo tanto no está visible.
    
  -El contenedor de la izquierda: Este contenedor es igual que en el horizontal. Su única diferencia es a la hora de dimensionar las       imagenes que hay dentro, puesto que he considerado que era mejor dejar su tamaño fijo.
    
  -Los contenedores para la nave, para la luna y para los menús son iguales.
    
  -El contenedor dropdown va a contener un fondon que sea una imagen y estará posicionada y dimensionada adecuadamanete. Cuando se pase   por encima del botón se desplegara un contenedor que contiene los botones dimensionados y con un margen. Además, estos botones al       igual que en el horizontal se harán más grandes al pasar por encima y cambiarán el color de fondo al activarse.
