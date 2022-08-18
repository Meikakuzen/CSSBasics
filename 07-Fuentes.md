# Fuentes

- Lo más básico es font-family. Se le da varias opciones

~~~css
h1{
    font-family: 'Verdana', 'Helvetica', sans-serif
}
~~~

- Pueden descargarse e incluirse con @font-face

~~~css
h1{
    @font-face{
        font-family: `Train One' ;
        src: url(/Fuentes/TrainOne-Regular.ttf)
    }
}
~~~