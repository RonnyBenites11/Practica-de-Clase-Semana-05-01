# Conceptos importantes CSS
## Selectores
- Indiuca a que elemento o elementos html se le aplicaran los estilos
- selector etiqueta
```css
<!-- /* SELECTOR DE ETIQUETA */ -->
h1{
    color:red;
}
<!-- /* selector descendencia */ -->
nav ul li{
    color:blue;
}
```
## Herencia
- Ciertas propiedades el padre esta heredando a sus hijos


## Cascada
- Lo que viene despues sobre escribe lo de antes css
## Especificidad
- Valor que adquieren los selectores y determinan que reglas CSS prevalece.
## Familias tipograficas
- existen tres tipos de fromas en como acceder a tipos de letras una de ellas es mediante la etiqueta link directamnete en el html , la otra mediante cdd con el @import y la otra descarganbdo la tipografia directamnete  ael proyecto
``` html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&family=Playwrite+NG+Modern:wght@100..400&display=swap" rel="stylesheet">

```
``` css
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&family=Playwrite+NG+Modern:wght@100..400&display=swap');
    font-family: "Playwrite NG Modern", cursive;

```
## Tamaños de fuentes
- px es la unidad de medida universal todas las demas se basan en ella
- em hace referencia a el contenedor en el cual esta alogada es decir si en el contenedor especificamos que el font sixe es 30px y en la etiqueta quie esta dentro colocamos que el fontsixe es de 1em el valor seria 30px en ese caso si colocamos 2em el valor seria de 60px, en caso de no colocar el valor font-size en el contenedor el valor por defecto e 1em es igual a 16px
```css
.contenedor{
    font-size: 30px;

}
h1{
    font-size : 2em; el valor seria 60px
}
´´´
- en el caso de rem al igual que el em el vañlor por defecto es 16px en caso de que su contenedor no este definido el font-size el contenedor directo del rem es html
´´´css
html{
    font-size: 20px;
}
h1{
    font-size : 2rem; el valor del em es igual a 20 px y como definimos que es 2 rem seria igual a 40px
}
´´´
- vw (Viewport Width): Esta unidad representa un porcentaje del ancho del viewport. 1 vw es igual al 1% del ancho total de la ventana del navegador. Por ejemplo, si el ancho del viewport es de 1000 píxeles, 1 vw equivaldría a 10 píxeles.
-vh (Viewport Height): Esta unidad representa un porcentaje de la altura del viewport. 1 vh es igual al 1% de la altura total de la ventana del navegador. Por ejemplo, si la altura del viewport es de 800 píxeles, 1 vh equivaldría a 8 píxeles.