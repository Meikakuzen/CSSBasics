# Unidades de color

- Con palabra clave: red, brown, etc. No personalizable
- Hexadecimal: #F0F0F0
- RGB, red, green, blue. Valores de 0 a 255: rgb(255,255,255)
- HSL, un código de color, saturación y brillo: hsl(125, 85%, 20%)
- Degradado: solo background: linear-gradient; Primer valor: de donde va a ser ese degradado (180deg de arriba a abajo)
    - Segundo valor: el color. Se pueden añadir varios
    - Tercer valor: hacia dónde
    - radial-gradient es circular
~~~css
div{
    background: linear-gradient(90deg, blue, green)
}
~~~
## Transparencia

- Hexadecimal: añade dos digitos más, 50 = 50% de transparencia
- RGBA: Añade el porcentaje de transparencia
- HSL: Añade el porcentaje
- opacity: 0.7. Más cercano al 1 es menos transparente
~~~css
div{
    background-color: transparent;
    background-color: #0000050;
    background-color: rgba(0,0,0,0.51);
    background-color: hsla(124,30%, 50%, 20%);
    opacity: 0.2
}
~~~