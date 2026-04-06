# bda-modulo-1-evaluacion-final-Ani-sabina

# 2.1 Funcion agegregar producto:
- He creado una funcion que agrega productos a mi inventario.
para poder agregar productos necesita saber el nombre, precio y cantidad que son los argumentos de la funcion.
- Mi funcion presupone que el producto que le voy a dar es falso (que no existe) creando una variable que diga producto_existe es igual a falso (tipo booleana)
mi funcion va a revisar los productos dentro del inventario con un bucle for
dentro del bucle for se pregunta: es el nombre del producto igual al nombre del producto que le estoy dando?
si es verdad, pasaran 2 cosas: una sera que la variable del producto existe (que al inicio era falso), ahora será verdadera (que si que existe un producto con ese nombre) y va al apartado cantidad del producto que ahora será la suma de la cantidad del producto mas la nueva cantidad.

- La ultima parte del codigo lo que hace es preguntarse si ¿el producto existe es falso? y si sigue siendo falso ya que se lo hemos dicho al inicio, lo que hace es ejecutar el append, que será añadir el producto nuevo, y para eso necesito tener todos los argumentos de mi inventario.

- si el producto existe es verdadero no ejecutara el append

# 2.2 Funcion ver inventario:
- He creado una funcion para poder ver el inventario por pantalla.
inicio creando un bucle for para que recorra por mi inventario, recorre cada diccionario guardado.
- Una vez que el diccionarios le pido que lo imprima con la funcion print.
le pido a print que me muestre las claves que escribo manualmente y los valores del diccionario, para que se muestre los valores le al producto que me muestre el valor de las claves nombre, precio y cantidad.

# 2.3 Funcion buscar producto:
- He creado una funcion para poder buscar en el inventario si esta el producto y en caso de estar que salga por pantalla los detalles del producto buscado.
primero creo un bucle for que recorrera dentro del inventario producto por producto.
- Con el if le digo al programa que si el producto nombre es igual al nombre que he solicitado me haga un print con los valores.

# 2.4 Funcion actualizar stock:
- He creado una funcion para actualizar el stock de mi inventario.
primero pongo que por defecto el producto = Falso (no existe).
- Creo un bucle for para recorrer el inventario y al preguntar por el nombre si lo encuentra ahora producto existe es True, al ser verdadero pasa otra cosa que es actualizar el inventario por eso la cantidad actual del producto es igual a la cantidad mas la nueva cantidad registrada.
- Por ultimo la funcion pregunta si el producto es falso y al ser falso como se indica al inicio procede a imprimir por pantalla el mensaje de Este producto no existe entre comillas porque quiero que salga ese mensaje tal cual.

# 2.5 Funcion eliminar producto:
-He creado una funcion para poder eliminar un producto del inventario si este este esta repetido.
- He empezando creando una variable para que el programa comience creyendo que el producto que vamos a buscar no existe.
- A continuacion realizo un bucle for para que recorra por el inventario lo que le pide el if, que es si el nombre del producto es igual al nombre que esta dando la usuaria, entonces la informacion de producto existe cambia a verdad y lo que hara será eliminarlo del inventario con el remove, entre parentensis esta el producto que es donde a recorrido el bucle for dento de inventario.

- Por ultimo con otro if el programa tambien pregunta si el producto exite es falso como se señala al inicio entonces pedimos que salga por pantalla el mensaje de "este producto no existe".

# 2.6 Funcion valor total:
- he creado una funcion para calcular el valor total del inventario y para eso, primero he creado una variable donde va a ir almacenado la multiplicacion que haga el blue for al pasasr por el precio y la cantidad del producto del inventario.
- Una vez tengo almacenado la multiplicacion del primer producto como bucle for sigue iterando sobre los demas productos lo que hago es sumar el nuevo valor del producto al total que lleva registrada valor total, que se ira sumando en cada iteracion.
- Para finalizar he creado un print fuera del bucle para que me imprima por pantalla el valor total.

# 2.7 Funcion realizar compra:
- Defino la funcion para poder realizar una compra.
- Lo siguiente que hago es crear 3 variables para usarlas dentro de mi funcion, que son:
    - seguir_comprando = True (con esto lo que pretendo es controlar el cucle, mientras sea verdad seguira comprando)
    - carrito = lo creo como lista para que el cliente pueda ir añadiendo lo que compre ahi
    - total_compra = creo esta variable para poder guardar ahi toda la suma de la compra
-creo el blucle while en que le digo al buble que siga saliendo si seguir_comprando sea igual a true, mientras eso sea verdad nel bucle nos mostrara el inventario (he usado el mismo codigo ya creado anteriormente para poder ver el inventario).
- dentro de la variable selecciona la prenda esta el input donde se le da 2 opciones al cliente, que seleccione el producto o que finalice la compra. Le pongo el .lower para que todo lo que escriba sea en minisculas ya que las prendas estan en minusculas.
- A continuacion le pongo una condicion al bucle while con el if, donde se interpreta como "si en el input de selecciona prenda pone finalizar" se cambia la variable seguir comprando a falso y esto hace que el bucle pare.
- A continuacion aparece el else con la finalidad de que nuestro codigo reaccione diferente cuando encuentre el producto del cliente, para esto empezamos con un indicador si econtramos el producto, con el bucle flor recorre todos los productos del inventario y con el if compara el nombre del producto en el inventario con lo que escribe el cliente,
- En este caso con el booleano señalado indicamos al codigo que el articulo seleccionado existe con el True.
- A continuacion anidamos otro if para indicar que ocurre si hay existencias de la prenda y para eso señalamos que dentro de la clave cantidad debe tener una cantidad mayor que 0, si es uan cantidad mayor a 0 ocurriran 4 cosas:
    - con el append añadimos la prenda seleccionada a la variable carrito ya creada al inicio del todo
    - tambien restara el producto seleccionado, con esto conseguimos actualizar el stock, ponemos -1, porque en ningun momento del codigo preguntamos al cliente cuantas unidades de producto quiere, entonces irá descontando de 1 en 1, si quiere otra vez el mismo producto tendra que seleccionarlo otra vez
    - contiara con mostrarnos en pantalla la prenda seleccionada
    - y para finalizar sumara el precio del producto al total
- dentro de este if tambien añadimos la condicional else para el caso que el producto cumpla con la condicion que sea mayor a 0, mostrando el mensaje "sin stock"
- Continuamos con el segundo if del for donde despues de recorrer todo el inventario si no se encontro ninguna coincidencia avisamo al cliente cone print de "producto no encontrado"
- para finalizar Mostramos al cliente cuánto debe pagar en total con el return carrito, total_compra devuelve la lista de productos comprados y el total.
