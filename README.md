# bda-modulo-1-evaluacion-final-Ani-sabina

## Funcion agegregar producto:
He creado una funcion que agrega productos a mi inventario.
para poder agregar productos necesita saber el nombre, precio y cantidad que son los argumentos de la funcion.
mi funcion presupone que el producto que le voy a dar es falso (que no existe) creando una variable que diga producto_existe es igual a falso (tipo booleana)
mi funcion va a revisar los productos dentro del inventario con un bucle for
dentro del bucle for se pregunta: es el nombre del producto igual al nombre del producto que le estoy dando?
si es verdad, pasaran 2 cosas: una sera que la variable del producto existe (que al inicio era falso), ahora será verdadera (que si que existe un producto con ese nombre) y va al apartado cantidad del producto que ahora será la suma de la cantidad del producto mas la nueva cantidad

la ultima parte del codigo lo que hace es preguntarse si ¿el producto existe es falso? y si sigue siendo falso ya que se lo hemos dicho al inicio, lo que hace es ejecutar el append, que será añadir el producto nuevo, y para eso necesito tener todos los argumentos de mi inventario.
si el producto existe es verdadero no ejecutara el append

## Funcion ver inventario:
He creado una funcion para poder ver el inventario por pantalla.
inicio creando un bucle for para que recorra por mi inventario, recorre cada diccionario guardado.
una vez que el diccionarios le pido que lo imprima con la funcion print.
le pido a print que me muestre las claves que escribo manualmente y los valores del diccionario, para que se muestre los valores le al producto que me muestre el valor de las claves nombre, precio y cantidad.

### Funcion buscar producto:
he creado una funcion para poder buscar en el inventario si esta el producto y en caso de estar que salga por pantalla los detalles del producto buscado.
primero creo un bucle for que recorrera dentro del inventario producto por producto.
con el if le digo al programa que si el producto nombre es igual al nombre que he solicitado me haga un print con los valores.

#### Funcion actualizar stock:
He creado una funcion para actualizar el stock de mi inventario.
primero pongo que por defecto el producto = Falso (no existe).
creo un bucle for para recorrer el inventario y al preguntar por el nombre si lo encuentra ahora producto existe es True, al ser verdadero pasa otra cosa que es actualizar el inventario por eso la cantidad actual del producto es igual a la cantidad mas la nueva cantidad registrada.
por ultimo la funcion pregunta si el producto es falso y al ser falso como se indica al inicio procede a imprimir por pantalla el mensaje de Este producto no existe entre comillas porque quiero que salga ese mensaje tal cual.

##### Funcion eliminar producto:
