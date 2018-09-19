#Listas simples

~~~
Variables listas.
a=[1,"hola",3.4,"adios",True]
lista=[1.73, 1.68, 1.71, 1.89, 1.79]
matriz=[[1.73, 1.68, 1.71, 1.89, 1.79],[65.4, 59.2, 63.45, 88.56 ,68.7]]
~~~
~~~
Mediante type podemos conocer el tipo de variable.
print(type(a))
<class 'list'>

Imprimos los valores de la variable lista a
print(a[0])
print(a[1])
print(a[-1])
print(a[0:2])

Resultados:
1
hola
True
[1, 'hola']

---------------------------------------------------
Valores de la variable lista matriz llamada matriz.

print(matriz)
print(matriz[0][0])# primer elemento de la primera fila
print(matriz[0][0:3]) # elementos de 0 a 2(elemento 1, 2 y 3) de la primera fila
print(matriz[1][0]) #  primer elemento de la segunda fila
print(matriz[1][-1]) # último elemento de la segunda fila
print(matriz[0]) # primera fila completa
print(matriz[1]) # segunda fila completa
print(matriz) # matriz completa
print(matriz[0:2])# matriz completa

Resultados:
[[1.73, 1.68, 1.71, 1.89, 1.79], [65.4, 59.2, 63.45, 88.56, 68.7]]
1.73
[1.73, 1.68, 1.71]
65.4
68.7
[1.73, 1.68, 1.71, 1.89, 1.79]
[65.4, 59.2, 63.45, 88.56, 68.7]
[[1.73, 1.68, 1.71, 1.89, 1.79], [65.4, 59.2, 63.45, 88.56, 68.7]]
[[1.73, 1.68, 1.71, 1.89, 1.79], [65.4, 59.2, 63.45, 88.56, 68.7]]
---------------------------------------------------
Las frases y palabras son en realidad listas de letras.
palabra="HolaMundo"
palabra[0]
'H'
palabra[:3]
'Hol'
palabra[3:]
'aMundo'
palabra[-1]
'o'
palabra[:-3]
'HolaMu'
palabra[-5:-2]
'Mun'
palabra[-5:]
'Mundo'
~~~
<pre>
#####Las operaciones más habituales que se realizan en Python son las siguientes:
lista[i]: Devuelve el elemento que está en la posición i de la lista.
lista.pop(i): Devuelve el elemento en la posición i de una lista y luego lo borra.
lista.append(elemento): Añade elemento al final de la lista.
lista.insert(i, elemento): Inserta elemento en la posición i.
lista.extend(lista2): Fusiona lista con lista2.
lista.remove(elemento): Elimina la primera vez que aparece elemento.
lista[3]=”otro dato”   actualiza el dato en la posición 3.

nombre="hola.html"
nombre2=nombre.split(".")
print(nombre2)
nom=nombre2[0]
ext=nombre2[1]
print(nom,ext)

Resultado:
['hola', 'html']
hola html
</pre>

# Tuplas
~~~
Son lo mismo que las listas pero se encierran entre paréntesis y no se pueden modificar.
t=(1,2,3,4)
print(type(t))
<class 'tuple'>
Convertir lista a tupla
listx = [5, 10, 7, 4, 15, 3]
print(listx)
tuplex = tuple(listx)
print(tuplex)
~~~















