# ParcialHerramientasComputacionales

## 1. ¿Qué problema es ?

es un problema que requiere de la creación de un software por medio de la escritura de código para resolver, facilitar y optimizar el funcionamiento del problema planteado en el enunciado, esto gracias a el uso de estructuras matemáticas para simular el comportamiento de la venta de productos en una tienda 

## 2. ¿Qué modelo computacional lo resuelve?

este problema es resuelto gracias a un modelo computacional matemático que realiza el calculo, que simula el comportamiento de la venta en una tienda como se puede aprecial en la linea de codigo.
```python
s = "Python syntax highlighting"

   precio = precio + ((producto[compra[0]][1]-producto[compra[0]][1]*(50/100))*int(compra[1])) 
   lista.append(producto[compra[0]][0])
   
   precio = precio + ((producto[compra[0]][1]-producto[compra[0]][1]*(20/100))*int(compra[1]))
   lista.append(producto[compra[0]][0])

```


## 3. ¿Qué recibe el algoritmo de entrada? y ¿Cuál sería su salida? 
_Entrada:_
```python
s = "Python syntax highlighting"

cedula = str(input("Digite su cédula: "))
rol = str(input("¿Es estudiante o maestro? "))   
##En esta parte lo que entra es el dato de la cédula y posteriormente el rol del usuario

        
compra = str(input()).split()
## en esta parte se pide el dato del nombre del producto que se va a comprar y la cantidad de este

SioNo = str(input("¿Desea comprar algo más? "))
##En esta parte se pide el dato de si el usuari desea comprar otro producto o desea finlaizar la compra
```
_Salida:_
```python
s = "Python syntax highlighting"

   print("El ",rol, "con cedula ", cedula,", ", "Debe pagar ",precio,"por el producto ", end = ' ')

    for x in lista:

        print(x, end=' ')

    print(" ")
    ## esta parte del codigo lo que hace es arrojar como dato final un texto que integra el rol del usuario, su cédula, cuanto debe pagar y una 
    ##lista con los codigos de los productos seleccionados

```

## 4. ¿Cómo lo calcula?
```python
s = "Python syntax highlighting"

   producto = {
    "JugoHit" : ["210",2500],
     "Cafe"    : ["200",1500],
     "Gaseosa" : ["129", 3000],
     "Te"      : ["180",1800],
     "Perro"   : ["300",3000],
     "Hambueguersa" : ["320",5000],
     "Pizza"   : ["330",4000]
}
##Se define el deccionario "producto" que es donde almasenamos los productos disponibles y su respectivo codigo y precio

def tienda():

    cedula = str(input("Digite su cédula: "))
    rol = str(input("¿Es estudiante o maestro? "))
    ## Aquí pedimos por teclado los datos de cédula y rol que son parte de la entrada del problema

    print("¿que producto desea comprar? y ¿Que cantidad?, digite el nombre y la cantidad")
    print("los productos disponibles son: ")
    
    
    for i in producto: 

        print(i, "" , producto[i][1] )
    ##Este for sirve para imprimir los nombres de todos los productos seguidos de sus precios
    
    
    op = True

    precio = 0

    lista = []
    ##Definimos las varialbes: "op" que es un booleano que almaena True, precio que es una esecie de contador para al final imprimir el precio final por loque se declara 
    ##con el valor 0 al inicio, y por ultimo "lista" que es donde guardaremos los codigos de los productos que compro para ser impresos al final.

    while op == True:
    ##El while lo usamos para que el ciente pueda registrartantos productos como quiera, hasta que op sea False, en dicho caso se calcelara el ciclo
        compra = str(input()).split()
        ##Recive el nombre del producto y la cantidad, estos datos se almacenan en una lista
        
        
        if compra[0] in producto:

            if rol == "estudiante" or rol == "Estudiante":

                precio = precio + ((producto[compra[0]][1]-producto[compra[0]][1]*(50/100))*int(compra[1])) 
                lista.append(producto[compra[0]][0])
            else:

                precio = precio + ((producto[compra[0]][1]-producto[compra[0]][1]*(20/100))*int(compra[1]))
                lista.append(producto[compra[0]][0])

        
        else:

            print("No se encuentra el producto")

        ## esta cdena de if's lo primero que hace es comprobar si el producto que el cliente desea comprar esta en el diccionrio "producto", si no esta 
        ##printea el mensaje "No se encuentra el producto", pero de lo contrario si si esta,revisa que rol fue digitado anteriormente y dependiendo de eso 
        ##realiza el calculo respectivo al precio del producto con su respectivo descuento y agrega el codigo del producto a "lista" para luego ser impresa
        
        SioNo = str(input("¿Desea comprar algo más? "))
        ##imprime le pregunta "¿Desea comprar algo más? " y guarda su respuesta
        if SioNo == "Si" or SioNo == "si":

            op = True
        
        else:

            op = False
        ##Si la respuesta guardada en "SioNo" es si, "op" es True ,de lo contrario si es no entonces "op" es False y el ciclo while se rompera dejando de 
        ##registrar mas productos
    print("El ",rol, "con cedula ", cedula,", ", "Debe pagar ",precio,"por el producto ", end = ' ')

    for x in lista:

        print(x, end=' ')

    print(" ")
    ##En esta parte ya para finalizar se imprime el mensaje respectiovo con los valores de las variables "rol", "cedula", y "precio" seguido de los 
    ##coódigos de los productos registrados
```


## Contenido del repositorio
El repositorio solo contiene 3 archivos uno es este que estas lellendo y los otros 2 son un archivo de word con la redaccion de los fallos ue se nos presetaron y su respectia solucion y el otro es el codigo como tal.

