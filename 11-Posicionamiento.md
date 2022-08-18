# Posicionamiento

- Estático, relativo, absoluto, fijo y pegajoso
- El posicionamiento es lo que me permite darle un libre albedrio a los elementos y poder ubicarlos dónde yo quiera

## Static y relative

- El posicionamiento estático es el que dispone de forma natural los elementos. 
- el posicionamiento relativo permite mover ese elemento en base a la posición en la que está

~~~css
div{
    position: relative;
    top: 100px
}
~~~

## Absolute
- La manera de usarlo es dentro de un contenedor padre con position:relative

- de esta manera lo ubicará en el extremo izquierdo del contenedor padre
~~~css
div{
    position: absolute;
    left:0
}
~~~

## Fixed
- Es como el hijo rebelde. Siempre va a estar en el lugar que yo le especifique, por mucho que haga scroll o lo que sea, siempre estará ahi.
- Se queda fijo en el lugar que le de

## Sticky

- Es pegajoso respecto al padre. es como el fixed pero relativo al padre


## Float
- Si yo le digo float: left se va a ubicar a la izqueirda y los elementos que tenga adyacentes se acoplarán