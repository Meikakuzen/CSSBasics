# Animaciones

~~~css
div{
    animation-name: changeColor;
    animation-duration: 5s;
    animation-timing-function: ease;
    animation-delay: 1s;
    animation-iteration-count: 1; /*numero de iteraciones*/
    animation-direction: normal; /*con alternate va de principio a fin y de vuelta al principio*/
    animation-fill-mode: forwards; /*se queda con el final de la animación, backguard vuelve al inicio antes de la animación*/
    animation-play-state: running; /*en paused no se realiza la animación*/
    /*atajo*/
    animation: nombre duración timing-function dirección play-state;
    animation: changeColor 5s linear infinite alternate running
}

@keyframes changeColor{
    0%{
        background: blue
    }

    50%{
        background: orange
    }

    80%{
        background: black
    }
}