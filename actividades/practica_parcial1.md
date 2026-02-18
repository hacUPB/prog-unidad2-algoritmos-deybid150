**ejercicios**
1. En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.

datos de entrada

|nombre|tipo|descripcion|
|------|----|-----------|
|PM|PF|Peso maximo de despegue|
|PV|PF|Peso de la aeronave en vacio|
|EW|PF|Carga añadida incluyendo los pasajeros|
|PF|PF|Peso del combustible|

Datos intermedios

|nombre|tipo|descripcion|
|------|----|-----------|
|SPS|PF|suma de los pesos|
|RP|PF|Resta entre el total y el maximo|

Datos de salida

|nombre|tipo|descripcion|
|------|----|-----------|
|ESTADO|BLN |Determina si el avion es apto para salir o no|
|PR|PF|Nos dice cuanto peso esta el avion por encima o por debajo del limite|


2. **Control de combustible en pruebas**
    
    Durante un ensayo en banco de un motor a reacción, se mide el nivel de combustible cada minuto y se detiene el registro cuando el combustible baja del 10%. Mostrar el tiempo total de operación antes de llegar a ese punto.

datos de entrada

|nombre|tipo|descripcion|
|------|----|-----------|
|CT|PF|Combustible total precargado|
|NC|PF|nivel del combustible|

Datos de salida

|nombre|tipo|descripcion|
|------|----|-----------|
|i|int|Tiempo transcurrido|


**pseudocodigo**
`````
inicio
    i = 0
    leer CT
    L = CT/10
    mientras CT > L
        
        leer CT
        i += 1

    fin mientras
        
    mostrar i "minutos transcurridos desde el inicio"

``````

fin

6. **Control de temperatura en cabina**
    
    Un sistema mide cada 5 minutos la temperatura en cabina durante una hora. Si en algún momento se detecta una temperatura mayor a 27°C o menor a 18°C, debe indicar que se active el sistema de climatización.

    **pseudocodigo**
`````
Inicio
    i = 0
    for i hasta 12
        leer T
        si 18 < T > 27
            Pasar
        sino 
            mostrar "activar ac"
        i += 1
    fin for
final