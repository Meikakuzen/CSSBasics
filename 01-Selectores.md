# Selectores


~~~css
/*Por etiqueta*/

h1{
    font-color: red
}

/*Por id*/

#miParrafo{
    font-size: 32px
}

/*Por clases (el más recomendable)*/

.texto-naranja{
    color: orange
}

/*Agrupar selectores. Puedo agrupar diferentes selectores, clases, id, etc*/

h1,p,a{
    color: blue
}

h1, .elemento1, #elementoId{
    font-size: 32px
}

/*Selectores descendientes. Párrafo dentro de contenedor*/

#contenedor p{
    font-weight: bold
}

#contenedor ul li a{
    color: yellow
}

/*Más simple*/

#contenedor a{
    color: yellow
}

/*Selector hijo. h1 dentro del hijo div del container*/

#contenedor > div h1{
    font-size: 32px
}

/*Selectores hermanos (al mismo nivel). Hay hermano general y el hermano adyacente (colo al que está al lado)*/
/*Todos los hermanos span de h1*/

#articulo h1 ~ span{
    color: white
} 

/*hermano adyacente (al lado)*/

#articulo h1 + span{
    color: red
}

/*Pseudoclases*/

a:hover{
    color:green
}

a:visited{
    color: violet
}

/*Pseudoclases avanzadas*/
/*Al primer elemento*/

p:first-child{
    color: blue
}

/*Al ultimo elemento*/

p:last-child{

}

/*Al elemento que le especifique, 3 en este caso*/

p:nth-child(3){
    color: brown
}

/*Contando desde el final, el penúltimo en este caso*/

p:nth-last-child(2){
    color: red
}

/*los elementos pares*/

p:nth-child(even){
    color: yellow
}

/*Los elementos impares*/

p:nth-child(odd){
    color: red
}

/*Elementos n*/

p:nth-child(3n){
    color: black
}

/*Pseudo-elementos before y after. Siempre hay que declarar el content*/
/*Util para iconos y otras cosas*/

span::before{
    content:'-',
    font-size: 32px
}

/*Selectores por atributo*/

p[type="number"]{
    color: blue
}

/*Que contengan una palabra*/

a[href*="udemy"]{
    color: violet
}

/*Que empiece por una palabra*/

a[href^="http"]{
    color: red
}

/*Que terminen por una palabra*/

a[href$=".com"]{
    color: yellow
}

