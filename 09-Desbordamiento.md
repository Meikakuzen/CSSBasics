# Desbordamiento

- Overflow tiene varios valores. hidden para ocultar el desbordamiento. Scroll crea la barra de scroll
- Auto es la mejor opción
- text-overflow: ellipsis crea unos puntos suspensivos para ocultar el resto del texto 
~~~css
div{
    overflow: auto;
    text-overflow: ellipsis   
}
~~~
# Despliegue de textos
- Con column-count despliega el texto en columnas
- Column-gap mide la separación entre columnas
~~~css

div{
    column-count: 3;
    column-gap: 20px;
    column-rule: 2px solid red /*linea divisoria de las columnas*/

}
~~~
