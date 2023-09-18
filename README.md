# Practice makes perfect
He aquí el repo del  RETO#4 
En cada uno de los archivos está cada uno de los puntos del reto #4
## 1.Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
Primero tuve que identificar los números pertenecientes al codigo ASCII (sí, cuando lo escribí, en mi cabeza sonó aski) de cada una de las vocales en minúscua, para la a:97, para la e:101, para la i:105, para la o:111 y para la u:117. Con ayuda de una estructura if-elif dar una condición con cada uno de estos números.
```pseudocode
print("Ingrese un numero entero")
numerito = float(input("Su número: "))
if numerito == 97:
    print("El número que ingresó corresponde a la vocal 'a' en el código ASCII")
elif numerito == 101:
    print("El número que ingresó corresponde a la vocal 'e' en el código ASCII")
elif numerito == 105:
    print("El número que ingresó corresponde a la vocal 'i' en el código ASCII")
elif numerito == 111:
    print("El número que ingresó corresponde a la vocal 'o' en el código ASCII")
elif numerito == 117:
    print("El número que ingresó corresponde a la vocal 'u' en el código ASCII")
else:
    print("El número que ingresó no corresponde a alguna vocal minúscula en código ASCII")
```
## 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no
Con cadena de longitud 1 entendí que era una cadena de un solo carácter. Con la función ord (que da el codigo ASCII de un carácter) definí una variable y despues con una operación modulo igualada a 0 cree una condición en una estructura if-else.
```pseudocode
la_cadenita = (input("Ingrese una letra: "))
codigo = ord(la_cadenita)
if codigo % 2 == 0:
    print("El código ASCII de primera letra de la cadena es par")
else:
    print("El codigo ASCII de la primera letra de la cadena es impar")
```
## 3.Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no
Parae ste punto con ayuda de una estructura if-else cree la condición cuando el caracter es igual a algún digito (0,1,2,3,4,5,6,7,8,9)
```pseudocode
el_susodicho = (input("Ingrese un carácter: "))
if el_susodicho == "0" or el_susodicho == "1" or el_susodicho == "2" or el_susodicho == "3" or el_susodicho == "4" or el_susodicho == "5" or el_susodicho == "6" or el_susodicho == "7" or el_susodicho == "8" or el_susodicho == "9":
    print("El carácter ingresado corresponde a un dígito")
else:
    print("El carácter ingresado no corresponde a un dígito")
```
# 4.Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero
Para este codigo solo fue necesario una estructura if-elif-else en la que se daban las dos condiciones, si el número era mayor que cero, si era menor y si no, era cero.
```pseudocode
a=float( input("Ingrese un número real: "))
if a > 0:
    print(f"El número {a} es positivo")
elif a < 0:
    print(f"El número {a} es negativo")
else:
    print(f"El número {a} es el número neutro para la suma")
```
# 5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
Lo primero fue buscar la ecuación de la circunferencia (que obviamente me la sabía y solo la busqué para estar segura) y ajustarla a las variables del código, además de que en vez de un = debía poner un <=-
Y con eso y una estructura if-else crear una condición cuando se cumple la igualdad de la ecuación.
```pseudocode
#Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
radio = float(input("Ingrese el radio de un círculo: "))
centro_x = float(input("Ingrese la coordenada en x del centro del círculo: "))
centro_y = float(input("Ingrese la coordenada en y del centro del cículo:  "))
el_punto_x = float(input("Ingrese la coordenada en x del punto: "))
el_punto_y = float(input("Ingrese la coordenada en y del punto: "))
if ((el_punto_x - centro_x)**2) + ((el_punto_y - centro_y)**2) <= (radio**2):#Ecuación de la circunferencia 
    print(f"El punto ({el_punto_x};{el_punto_y}) pertenece al interior del círculo de centro ({centro_x};{centro_y}) y radio {radio}")
else:
    print(f"El punto ({el_punto_x};{el_punto_y}) NO pertenece al interior del círculo de centro ({centro_x};{centro_y}) y radio {radio}")
```
# 6.Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
Para poder contruir un triagunlo es necesario que se cumpla para cualquiera de sus lados que un lado siempre va a ser menor que la suma de los otros dos. Teniendo eso en cuenta, con una condición if-else y un conector and creé la condición.
```pseudocode
lado_a = float(input("Ingrese la longitud del lado 'a': "))
lado_b = float(input("Ingrese la longitud del lado 'b': "))
lado_c = float(input("Ingrese la longitud del lado 'c': "))
if lado_b < (lado_c +lado_a) and lado_c < (lado_b +lado_a) and lado_a < (lado_c +lado_b):
    print("Es posible crear un triangulo a parir de las longitudes ingresadas")
else:
    print("NO es posible crear un triangulo a parir de las longitudes ingresadas")
```
