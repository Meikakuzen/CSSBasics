# BEM

- Block Element Modifier

- Significa que debo tener elementos bloque, items y modificadores

- Trabajo con clases
- BEM dice que cuando es un elemento bloque se trabaje como una clase
- Para los items me voy a referir como block__item, (block=contenedor padre)
- Los modificadores se usan con un guión block-modificador
- No estoy amarrando el box_btn al box. box es el bloque, y box_btn el elemento
- Con el modificador añado la clase .box y .box--green al elemento html

~~~css
.box{
    width: 300px;
    height: 200px;

}

.box__btn{
    padding: 8px;
    background-color: red
}

/*modificador*/

.box--green{
    color: green
}

~~~
- BEM ayuda a reutilizar código y estructurar mejor el código
- Para proyectos grandes es recomendable