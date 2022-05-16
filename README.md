# Cultura-Urbana-Sass

Optimizaciones SEO:

Index
Meta tags base, los cuales se repetiran y tendran una modificacion minima en en resto de las paginas

<meta name="Keywords" content="buzos de hombre, buzos de mujer, ropa de hombre, ropa de mujer, ropa de moda, remerones, remeras 2022">

<meta name="Description" content="Tienda urbana, cultura urbana tienda, ropa a la moda, ropa callejera" >

<meta name="title" content="Tienda Cultura Urbana">

Resto de las paginas:

Cambio de titulos relacionados con sus respectivas paginas
Cambios en el meta name title para tener relacion con la pagina
Cambios en el meta name description para tener relacion con la pagina
Agregado de keywords en relacion a las paginas

<!-- Sale-->
<meta name="Keywords" content="productos en oferta, producto con descuentos, productos mas vendidos">

<meta name="Description" content="productos en sale cultura urbana, remate de accesorios, temporada 2022, descuentos" >

<!-- Productos-->
<meta name="Keywords" content="remerones, sudaderas, bermudas, camperas, buzos, ver buzos, ver remeras, ver sudaderas, ver camperas, ropa mujer, ropa hombre ">

<meta name="Description" content="productos cultura urbana, busca tu estilo, temporada 2022, proxima temporada en octubre" >

<!-- Politica de devolucion-->
<meta name="Keywords" content="devolucion de dinero, devolucion de prendas, politicas de devolucion, arreglo de envios">

<meta name="Description" content="productos para devolver, devolucion de dinero, devolucion de prenda" >

<!-- Contacto-->
<meta name="Keywords" content="contacto pagina, contacto para ventas, contacto para consultas, consulta, mayoristas, minoristas">

<meta name="Description" content="contacto de la pagina, ayuda, devolucion, contactame, contactar" >

Uso de SASS

Mixins:
Use @mixin para aplicar flex rapidamente, ya que lo uso en varias parte de la estructura de mi pagina

@mixin flexible ($dis, $direction, $just, $align, $text){
    display: $dis;
    flex-direction: $direction;
    justify-content: $just;
    align-items: $align;
    text-align: $text;
}

Mapas
Use mapas para los headings en especial los h4-h5 para textos simples.
$headings: (
h4: smaller,
h5: smaller,
h6: smaller 
);

Extend
Use extend para setear mi clase card con configuraciones basicas de display e imagen.

.ucard{
    @extend .card;
    

    img {
        @extend .avatar;
    }
}