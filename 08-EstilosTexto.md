# Estilos texto


- Letter-spacing me permite determinar el espacio entre cada letra. Con word-spacing es lo mismo pero con las palabras
- Line-height permite determinar el interlineado
- La sangría es con text-indent
- El borde de texto se trabaja con text-fill y text-stroke. No losoportan todos los navegadores
- Text-align para alinear el texto
- Transfromar a minusculas, mayúsculas o capitalize
- El pseudo-elemento first-line y first-letter me permite trabajar con la primera linea o primera letra respectivamente
~~~css
p{
    letter-spacing: 2px;
    word-spacing: 3px;
    line-height: 20px;
    text-indent: 8px;
    text-align: center;   /*O justify, end*/
    text-transform: lowercase
}

p::first-line{
    color: red
}
~~~
- Para quebrar palabras a final de linea se usa overflow-wrap con valores anywhere o break-word (actuan igual)
- word-breack: breack-all romperá todas las palabras
- hyphens: auto (la más usada) coloca un guión y quiebra la palabra
~~~css
p{
    overflow-wrap: anywhere;
    hyphens: auto
}
