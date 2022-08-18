# CSSGRID
- Para columnas grid-template-columns
- Para filas grid-template-rows
----
- Primero debo indicar display: grid en el contenedor padre
- Segundo indicar el numero de columnas y filas con su tamño correspondiente
- Unamanera podría ser esta
~~~css
.container{
    width: 100%;
    display: grid;
    grid-template-columns: 200px 200px 200px;
    grid-template-rows: 300px 300px 300px ;
}
~~~

- Hay una unidad más viable que es la fracción.

~~~css
.container{
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 2fr 2fr 2fr 2fr ;
}
~~~

- Puedo usar una forma abreviada con filas y columnas
~~~css
.container{
    grid-template: 1fr 2fr 1fr /  1fr 3fr 3fr 2fr

}
~~~
- Establecer separación
~~~css
.container{
    
    grid-template: 1fr 2fr 1fr /  1fr 3fr 3fr 2fr;
    grid-gap: 20px
}

~~~
- Puedo usar funciones como repeat para establecer las filas y columnas 
~~~css

.container{
    grid-template: repeat(3, 1fr) / repeat(4,1fr)
}
~~~
- Puedo salir del repeat para crear una columna distinta
~~~css

.container{
    grid-template-columns: repeat(3,200px) 2fr 100px
}
~~~
- Puedo establecer valores minimo y máximo
~~~css
.container{
    grid-template-columns: minmax(150px, 300px)
}
~~~
## Posicionar elementos
- El grid dispone de números (del 1 al 2, del 2 al 3, etc) tanto para filas como para columnas
- Puedo usar la posición de inicio y final para colocar el elemento
~~~css
.grid .item{
    grid-column-start: 2; 
    grid-column-end: 4;
    grid-row-start: 2;
    grid-row-end: 3;
    /*atajo*/
    grid-column: 2 / -1; /*-1 es el final*/
    grid-row: 3 / 4;
}
~~~
- También está grid-area que agrupa grid-column y grid-row
----
## Grid Areas
- Me permite crear una plantilla
~~~css
.container{
    grid-template-areas: "header    header      header"
                         "contenido contenido   asside" 
                         "contenido contenido   asside"
                         "widget1   widget2     asside"
                         "footer    footer      footer"  
}

.item{
    grid-area: header
}

~~~
## Alineación de elementos

- Alineación horizontal se hace con justify-items. End, start, center, auto, stretch (ocupa todo el contenido)
- Alineación vertical se hace con align-items.
- Se puede alinear un elemento en concreto con justify-self y align-self
~~~css
.item-seleccionado{
    justify-self: center;
    align-self: center
}
~~~

### Alineación multilinea

- Justify-content también sirve aquí. Center, start, space-around, space-between, space-evenly
- Align-content para la alineación vertical. Start, end, space-around

### Centrar con grid

- display:grid, justify-content: center, align-content: center 
- En flexbox sería display: flex, justify-content: center, align-items: center

## Orden de elementos
- Si todos los elementos tienen orden 0 ( su valor inicial ) al elemento que le ponga 1 lo situará al final, o -1 para ser el primero
- Con order puedo darles la ubicación en el orden que yo quiera
~~~css
.grid .item2{
    order: 1
}
~~~

