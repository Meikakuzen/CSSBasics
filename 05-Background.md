# Background

- Con cover abarca el 100% del contenedor.
- Para que esté centrado: background-position: center. Puedo decirle center-top
- Attachment: local, scroll, fixed
- Para todo esto esta el atajo background:
    - url(img)
    - no-repeat
    - fixed
    - center
    - cover NO lo incluye, hay que hacerlo manualmente
~~~css
div{
    background: red;
    background: linear-gradient(90deg, green, yellow);
    background-image: ('./wallpaper.jpg');
    background-repeat no-repeat;
    background-size: cover;
    background-position: center center;
    background-attachment: fixed; /*Se queda fija*/
    /*object-fit: cover evita la distorsion de la imagen*/
    /*object-position: center center*/
}

~~~
## BLEND MODE

- Para combinar imagenes puedo usar blend-mode. Puedo añadirle un color después de las url(opcional)
- Tiene varias opciones: multiply, screen, overlay, darken, lighten, color-dodge, saturation, ,color, luminosity, hue
    - multiply es el más popular
~~~css
div{
    width: 100vh;
    height: 100vh;

    background: url('./img.jpg'), url('img2.jpg'), yellow;
    background-size: cover;
    background-position: center;
    background-blend-mode: multiply;
}
~~~

## Filters

~~~css
img{
    filter: grayscale(80%);
    filter: blur(5px); /*difumina*/
    filter: sepia(80%);
    filter: saturate(80%);
    filter: opacity(20%); /*Mas cercano al cero más transparente*/
    filter: hue-rotate(180deg); /*rota los colores*/
    filter: invert(70%);
    filter: drop-shadow(20px 10px 5px #00000) /*x y difuminado color*/
}
~~~
- backdrop-filter lo aplicará solo al fondo con cualquiera de los filtros