# Consulta 1(Estructura)

for $item in //Item  
where $item/@categoria \= "Hardware" and number($item/AnioLanzamiento) \< 1985  
return   
\<resultado\>  
Titulo: {$item/Nombre/text()} \-   
Año: {$item/AnioLanzamiento/text()}  
\</resultado\>

# Consulta 2(Estructura)

for $item in //Item  
where number($item/EstadoConservacion) \= 5  
return   
\<resultado\>  
Titulo: {$item/Nombre/text()}  
Precio: {$item/ValorEstimado/text()}  
Lanzamiento: {$item/AnioLanzamiento/text()}  
\</resultado\>

# Consulta 3(Estructura)