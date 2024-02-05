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







