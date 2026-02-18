**ejercicio**

un acuario necesita determinar cuantos litros o galones de agua caben en un acuario, pero solo dispone de una cinta metrica.

**datos de entrada**

unidad: unidad de medida de agua

largo: largo del tanque en cm

ancho: ancho del tanque en cm

alto: alto del tanque en cm

**datos de salida**

vol_lit: volumen en litros

vol_gal: volumen en galones


**Pseudocodigo**

````
inicio
    mostrar: "por favor ingrese las medidas del tanque"
    leer largo, ancho, alto
    mostrar: "ingrese L para litros y G para galones"
    leer unidad

    Vol = largo*ancho*alto

        Val_lit = vol/1000

        si unidad = "G"

            Val_gal = Val_lit*0.26
            
            mostrar: Val_gal

        si no
            mostrar: Val_lit
````
**ejercicio 2**

Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

**datos de entrada**
|nombre|descripcion|
|------|-----------|
|CL|cantidad de lapices|

**datos de salida**
|nombre|descripcion|
|------|-----------|
|T|Precio total|

**Pseudocodigo**

`````
inicio
    mostrar: "cantidad de lapices a comprar"
    leer CL
    si CL >= 1000
        T = CL*85
        Mostrar: T"$"
    Si no
        T = CL*90
        Mostrar: T"$"
    fin si
fin

``````

**ejercicio 3**

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

**datos de entrada**
|nombre|tipo|descripcion|
|------|----|-----------|
|C|PF|Valor de la compra|

**datos intermedios**
|nombre|tipo|descripcion|
|------|----|-----------|
|