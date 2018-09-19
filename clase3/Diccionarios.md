#Diccionarios

~~~
c={"Saludos":"Hola",1:"Manzana",2:"Naranja","Panamá":507,"España":3}

c[2]--> 'Naranja'

c["Panamá"]--> 507

El algoritmo que usa Python internamente para buscar un elemento en un diccionario es muy distinto que el que utiliza para buscar en listas.

Para buscar en las listas, se utiliza un algoritmos de comparación que tarda cada vez más a medida que la lista se hace más larga. En cambio, para buscar en diccionarios se utiliza un algoritmo llamado hash, que se basa en realizar un cálculo numérico sobre la clave del elemento, y tiene una propiedad muy interesante: sin importar cuántos elementos tenga el diccionario, el tiempo de búsqueda es siempre aproximadamente igual.

Este algoritmo de hash es también la razón por la cual las claves de los diccionarios deben ser inmutables, ya que la operación hecha sobre las claves debe dar siempre el mismo resultado, y si se utilizara una variable mutable esto no sería posible.

No es posible obtener porciones de un diccionario usando [:], ya que al no tener un orden determinado para los elementos, no sería posible tomarlos en orden.

Un diccionario es una colección no ordenada de objetos. Es por eso que para identificar un valor cualquiera dentro de él, especificamos una clave (a diferencia de las listas y tuplas, cuyos elementos se identifican por su posición). Las claves suelen ser números enteros o cadenas, aunque cualquier otro objeto inmutable puede actuar como una clave. Los valores, por el contrario, pueden ser de cualquier tipo, incluso otros diccionarios.
Para crear un diccionario se emplean llaves ({}), y sus pares clave-valor se separan por comas. A su vez, intercalamos la clave del valor con dos puntos (:).

Otras formas de crear diccionarios
Haciendo uso directo de la clase dict Python ofrece algunos métodos para crear diccionarios de formas alternativas (cuyo uso, por cierto, es poco usual).
Si se pasan argumentos por nombre a dict(), constituirán las claves del nuevo diccionario como cadenas.
>>> d = dict(Python=1991, C=1972, Java=1996)
>>> d
{'Python': 1991, 'C': 1972, 'Java': 1996}
https://recursospython.com/guias-y-manuales/diccionarios/
http://www.w3big.com/es/python/python-dictionary.html


~~~















