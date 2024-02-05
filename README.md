# Reglas de estilo utilizada en el proyecto

## Hoja de estilo de la pagina principal: style.css

*{

  margin:0;

  padding: 0;

  font-family:Verdana, Geneva, Tahoma, sans-serif;

}

Da margen y padding de 0 a todo el documento, además de darle la fuente de Verdana.

.container{

  display: grid;

  height: auto;

  width: 90%;

  margin: 0 auto;

  grid-template-rows: 110px 600px 500px 200px;

  position: relative;

}

Se le da propiedad de grid para poder dimensionar las filas. Se le da un ancho de 90% de la pantalla y se le quita las márgenes, se le coloco posición sea relativa al contenedor que envuelve a la regla de estilo.

 header{

  display: flex;

  justify-content: space-between;

  width: 100%;

  height: 110px;

  grid-column: 1;

  grid-row: 1;

  background-color:#F2163E;

}

Se utilizo display:flex para que lo que contenia el header se ordenaran de forma horizontal.  justify-content: space-between da un espaciado a lo que contenía el header, con grid column y row se le dijo al programa que tomara la primera fila y la primera columna y se le dio un color de fondo con background.

.cont{

  width: 100%;

  display: flex;

  justify-content: space-between;

  align-items: center;

  }

Contiene el menú de navegación el cual todos sus items se alinean horizontalmente con flex. Da un espacio entre ellos con space-between y los alinea centralmente de manera vertical.

.catalogo{

  width: 100%;

  grid-column: 1;

  grid-row: 2;

}

Da un ancho de 100% es decir que ocupe todo el contenedor de manera horizontal. con grid column y row dice que empiece de la fila 2 y columna 1.

.tres-productos{

  width: 100%;

  height: 500px;

  grid-column: 1;

  grid-row: 3;

}

El contenedor tres-productos se le da una ancho de 100% para que ocupe todo el contenedor de manera horizontal, se le dio un alto de 500 px y con grid column y row se dice que empiece en la columna 1 fila 3.

.logo{

  width: 230px;

  height: 100px;

}

El logo tendrá un ancho de 230px y un alto de 100px.

nav ul{

  display: flex;

  list-style: none;

  text-align: center;

  margin: 15px 15px;

  font-size: 20px;

  font-weight: bold;

}

A una lista dentro de nav se realizo con flex el ordenamiento horizontal de los elementos dentro de ella, se le quito los estilos, se alinearon central los elementos, el tamaño de letra se coloco a 20px y que la letra en negrita. Se le colocaron márgenes de 15px.

nav ul li{

  margin: 0;

  padding: 0 30px;

  }

A cada elemento li se le dio margen 0 y padding lateral de 30px.

nav ul li a{

  text-decoration: none;

  color:white;

  display: block;

  margin: 0;

  padding: 0;

}

A los elementos "a" se les quito la decoración del texto, se colocaron las letras de color blanco y que se desplegaran en forma de bloque ósea en columna, las márgenes y el padding se colocaron a 0.

nav ul li :hover{

  border: 2px solid;

  border-color: #73060F;

  background-color: #73060F; 

  color:aquamarine

}

Con hover podemos activar un elemento al pasar el puntero del mouse sobre el. Aquí cuando se activa el elemento li aparece un borde de 2px cambiando de color las letras y el fondo.

nav ul li:active{

  padding: 2px;

}

Cuando esta activa "li" su padding aumenta haciéndola ver mas grande.

.catalogo-foto{

   width: 100%;

  height:600px;

}

Da un ancho de 100% para que ocupe todo el contenedor y un alto de 600px.

.producto-prin{

  width: 250px;

  height: 250px;

  border-radius: 10px;

  background-color: #F2163E;

}

Da al producto principal un tamaño de 250x250px. Al border se le da un redondeo de 10px y se coloca de color de fondo un rosado.

h1{

  text-align: center;

  font-size: 40px;

  padding: 30px;

  color: black;

}

Al titulo lo centran y le dan un tamaño de 40px, un padding de30px y que las letras sean de color negro.

.pro-relevantes{

  display: flex;

  justify-content: space-evenly;

}

En la sección de productos relevantes se colocó que los elementos dentro de esta sección estuvieran alineados horizontalmente usando "flex" y se le dio un espaciado con  justify-content: space-evenly.

.p1{

  text-align: center;

  color: black;

  }

A los párrafos "p1" se le coloco que el parrafo  se centrar y la letra sea de color negro.

footer{

  width: 100%;

  height: 200px;

  grid-column: 1;

  grid-row: 4;

  background-color:#F2163E;

  display: flex;

  justify-content: center;

}

se le dio tamaño de100% de ancho por 200px de alto, el footer ocupa la primera columna y la 4 fila. Se le dio un color rosado de fondo, los items dentro del footer van a estar alineados horizontalmente y van a estar centrados por el flex y por justify-content respectivamente.

### @media

.container{

​    text-align: center;

​    align-items: center;

​    justify-content: center;

​    grid-template-rows: 200px 200px 910px 500px;

​    flex-direction: column;

​    width: 350px;  

​    margin: 0 auto;

  }

En el container principal se alinean centralmente el texto a la parte central en eje Y, y los elementos  justify-content centran los elementos. Se le dio el tamaño a las a las filas y se organizan en columnas con un ancho de 350px.

nav ul{

​    position: relative;

​    width: 350px;

​    height: 300px;

​    background: coral;

​    top: 150px;

​    left: -100%;

​    display: none;

​    z-index: 1;

​    text-align: center;

​    transition: all 0.5s;

​    padding-top: 15px;

​      }

Se le da una posicion relativa a "ul" para que mas adelante con top y left se le de la posición respecto al contenedor donde se ubica, se le dio un fondo color coral, se hizo invisible con el fin de que se haga un hover mas adelante y aparezca. El z-index es para colocar una imagen sobre otra y se vea la que este encima. transition hace que haya una transición menos abrupta entre un estado del elemento y otro.

  #check:checked ~  ul{

​    left:0px;

​    display: block;

  }

Cuando el check este activo el elemento "ul" tomara la posición de 0px a la izquierda y se mostrara en bloque su contenido.

footer{

​    text-align: center;

​    align-items: center;

​    justify-content: center;

​    height: 510px;

​    flex-direction: column; 

  }

En el footer los texto se alinearon y los items también de manera central, se le dio un tamaño de 510px con una dirección en columna.



## Hoja de estilo del catálogo: style2.css

*{

  margin:0;

  padding: 0;

  font-family:Verdana, Geneva, Tahoma, sans-serif;

  }

Da margen y padding de 0 a todo el documento, además de darle la fuente de Verdana.

.container{

  display: grid;

  height: auto;

  width: 100vw;

  margin: 0 auto;

  border-color: black; 

  grid-template-rows: 70px 750px 800px 800px 800px 200px;

  }

Al haber declarado grid al comienzo,  se asigna el tamaño de las filas, se le dio un color negro al borde y un máximo de pantalla.

.cont-foto1:hover .foto-peque1{

  background-image: url('/../images/foto1.png');

  position: relative;

  width: 550px;

  height: 500px;

  top:80px;

  left:240px;

  }

se llama a una imagen, se le coloca posición relativa con un top de 80px y un left de 240px.

y sus dimensiones las cuales son 550x500px.

nav ul{

​    position: relative;

​    width: 350;

​    height: 300px;

​    background: coral;

​    top: 23px;

​    left: -160%;

​    display: block;

​    z-index: 1;

​    text-align: center;

​    transition: all 0.5s;

​    overflow-y: scroll;

​    scroll-behavior: smooth;    

  }

Se le asigna una posición relativa de top:23px y left -160px.  el z-index hace que la imagen se coloque encima de las otras que estén abajo. Se alineó el texto centrado. la transition durará 0.5s. scroll es para que hubiera una barra lateral con la cual se pueda hacer scroll.

.descripcion-pro{

​    padding-top: 10%;

​    grid-column-start: 1;

​    grid-column-end: 3;

​    padding: 0px;

​    text-align: justify;

  }

En la descripción de los productos se le dio un padding-top de 10%. El contenedor va a ocupar la fila 3 y columna 1. Tendrá un padding de 0 y el párrafo estará justificado.