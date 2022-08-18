# Transiciones

- El primer argumento es a que propiedad se le aplica. La segunda, cuánto va a durar. La tercer es la velocidad de la transición, la cuarta el delay
~~~css
.elemento-transicion{
    background: red; 
    transition-property: background;
    transition-duration: 1s;
    transition-timing-function: linear; /*velocidad lineal, hay otros valores como ease, ease-in, ease-out, ease-in-out, etc*/
    transition-delay: 1s;
    /*atajo*/
    transition: background 1s linear 1s 7 /*puedo usar transition: all para todas las propiedades*/
}

.elemento-transicion:hover{
    background: orange
}
~~~