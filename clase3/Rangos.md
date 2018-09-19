#Rangos

~~~
#Tipo range(m, n, p)

# m: el valor inicial. A partir de donde arranca la secuencia, pero si no pones n o el valor final(que se explica a continuación), entonces este valor m se tomará como el final y el valor inicial será 0.
Ejem:range(5) será -->[0, 1, 2, 3, 4] , no incluye el 5. Para poder visualizar los valores de un rango, es mejor convertirlos en lista y de esa forma usar el print.
print(list(range(5)))será -->[0, 1, 2, 3, 4]

Si pones print(list(range(-5))) te saldrá [  ]  o sea, lista vacía, o sea, en el formato en el que usas solo el valor de inicio m  sin los demás parámetros(n y p), es para trabajar con enteros positivos solamente.


# n: el valor final (que no se alcanza nunca pues  alcanza es a n-1). Si es por ejemplo n= 5, llegará hasta 4 y 4 es el final de la secuencia. Si no pones n,el final será igual al valor m o inicial, y el inicial tomará el valor de 0, o sea, queda en el formato range(m) sin los demás parámetros. Si pones m y n sin el parámetro p, queda en el formato range(m,n), y por tanto p por defecto siempre será 1.

Ejemplos:
print(list(range(0,5))) -->[0, 1, 2, 3, 4]
print(list(range(-5,0))) --> [-5, -4, -3, -2, -1]
Funcionarán todas aquellas secuncias que se mueven hacia la derecha solamente, pues al no poner el parámetro p, por defecto dicho parámetro tomará el valor 1 positivo, y por tanto se sumará al valor de un rango para que pueda moverse al siguiente valor.
Pero si haces por ejemplo:
print(list(range(0,-5))) --> te saldrá [ ] o sea, lista vacía, pues si le sumas a 0 el 1 por defecto del valor de la p, va empezar a crecer hacia la dirección contraria a valor final que es -5(realmente es -4), y en vez de mandar error, te devuelve una lista vacía.



# p: el paso (la cantidad que se avanza cada vez). Trabaja sumando al inicio hasta alcanzar el final, aconsejo que  siempre se sume la p al valor inicial y se vea si avanza hacia la dirección del valor final y sabrás si estás colocando el signo del paso de forma correcta. Puede ser negativo o positivo. Si no lo pones,  por defecto será 1 positivo.

Ejemplos:
valores=list(range(-5, 6,2))
print(valores)
[-5, -3, -1, 1, 3, 5]
Observa , que el paso, es positivo, y al restar al valor inicial -5+2=-3, va hacia la dirección del final(que es 6, o mejor dicho 6-1=5) , o sea, va hacia la derecha, que es la dirección correcta.

valores=list(range(-5, -10,-1))
print(valores)
[-5, -6, -7, -8, -9]
Vemos que al sumar al valor incial -5 el valor -1: -5-1=-6  va hacia la dirección correcta de -10, por eso el paso -1 es correcto.


Ojo como asignas los valores de un rango a una lista, veamos:

a=[range(5)]
print(a) --> [range(0, 5)]   o sea, te devuelve una lista con un solo elemento, dicho elemento es un rango.
Si haces:
print(a[1])--> saldrá error, pues te dirá que solo hay un solo elemento, y por tanto el índice que acepta es el 0, el del primer elemento,no hay un segundo elemento.
Si haces:
print(a[0]) --> range(0, 5)  te devuelve el valor que es un rango.
Si quieres entrar a ver los valores del único valor de la lista , o sea los valores dentro del rango:
print(a[0:1])-->[0]  recuerda que inicia en 0 y termina en n-1, o sea, 1-1=0, por tanto inicia en 0 y termina en 0, es 0.
print(a[0:2])-->[0,1]
print(a[0:5])-->[0, 1, 2, 3,4]
print(a[1:2])-->[1]
print(a[2:3])-->[2]
print(a[3:4])-->[3]
...

Ahora bien, ¿qué pasa si son dos rangos?
a=[range(5),range(5,11)]
print(a)-->[range(0, 5), range(5, 11)] te devuelve una lista con dos elementos, y para ver dentro de ellos:

print(a[0][0:3])-->range(0, 3)  devuelve un rango que es un subrango del primero rango y que va desde 0 a 3.
print(a[0][4:5])-->range(4, 5) devuelve un rango que es un subrango del primero rango y que va desde 4 a 5.
print(a[1][0:3])-->range(5, 8) devuelve un rango que es un subrango del segundo rango y que va desde 5 a 8, pues el índice 0 apunta al primer elemento del segundo rango que es 5, y el ìndice 3 apunta al 4 elemento del segundo rango que es 8.


Ahora bien, no queremos elementos que sean rangos dentro de nuestras listas, lo que queremos son los elementos que producen los rangos, no los rangos en sí (los objetos rangos), para eso trabajo así:

a=list(range(5))
print(a)--> [0, 1, 2, 3, 4]  ahora si, me ha devuelto una lista (pues son valores dentro de corchetes) de elementos, no rangos.

~~~















